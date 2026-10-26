# Mitsubishi Destinator / DST Concept (2025-2026) Platform Technical Dossier

## 1. Overview & Platform Architecture
The **Mitsubishi Destinator** (derived from the production version of the Mitsubishi DST Concept unveiled in late 2024 / 2025 for ASEAN and emerging markets) is a 3-row, 7-seater compact monocoque SUV positioned between the Xforce and the Pajero Sport.
It shares the modular ASEAN platform and electrical architecture with the **Mitsubishi Xforce (2023-2026)** and **Xpander Cross HEV (e:MOTION)**.

### Engine & Transmission Configurations:
* **Engine**: 1.5L 4-Cylinder DOHC 16-valve MIVEC (Naturally Aspirated `4A91` / Turbocharged `4B40` or hybrid e:MOTION system).
* **Transmission**: High-efficiency Lineartronic-type Continuously Variable Transmission (CVT) with manual step-shift simulation.
* **Drive Modes**: Normal, Wet, Gravel, Mud (integrated Electronic Stability & AYC - Active Yaw Control).

---

## 2. ECU Hardware Specifications
* **ECU Supplier**: Melco (Mitsubishi Electric Corporation) Gen3 CAN Platform.
* **Microcontroller (MCU)**:
  - Renesas SuperH SH72543 (2MB Flash, 128KB RAM, 200MHz 32-bit RISC) or
  - Melco MH8115F (2.5MB Flash embedded memory).
* **Communication Interface**: High-Speed CAN-Bus (ISO 11898-2) @ 500 kbps (CAN Diagnostic ID: Request `0x7E0`, Response `0x7E8`).
* **Factory Part Number Series**: `1860E0xx` / `1860Fxxx`.

---

## 3. Bench Read, Bootloader & Flashing Protocols
Unlike older Mitsubishi vehicles (which use Tactrix OpenPort 2.0 with standard OpenEcu / EcuFlash K-Line bootloader), the 2025-2026 Melco Gen3 CAN ECUs implement strict OEM cryptographic security:
1. **Commercial Flashing Support**:
   - **PCMFlash**: Module 31 (*Mitsubishi K-Line/CAN-Bus*) or Module 82 (*Melco MH8115F SH72543 CAN Boot*).
   - **BitBox**: *Mitsubishi Melco Gen3 CAN* (Bench / OBD read via UDS ISO 14229).
   - **Alientech KESS3 / CMDFlash**: Boot/Bench Tricore / Renesas SuperH plugin.
2. **Seed/Key Security Exchange**:
   - UDS Diagnostic Session Control (`0x10 0x03` - Extended Diagnostic Session).
   - Security Access (`0x27 0x01` - Request Seed, `0x27 0x02` - Send Key calculated via OEM AES-128 / proprietary polynomial hashing).
3. **Public Repository / Open-Source Binary Status**:
   - Factory raw binary dumps (`.bin` / `.hex`) of brand-new 2025/2026 pre-production vehicles are **not released on public open-source Git repositories** due to OEM proprietary intellectual property and cryptographic locks.
   - Per strict anti-fabrication standards, **ZERO synthetic binaries** are created. Calibration tuning definitions and reverse-engineering work map directly to the Melco Gen3 platform shared with the Xforce:
     `02_CARS/MITSUBISHI/XFORCE_4A91_CVT/GENERATIONAL_1860E035_Mitsubishi_Xforce_1.5_MIVEC_CVT_(2023-2026).xdf`.

---

## 4. Key Calibration Map Structure & Offsets
When a physical dump is obtained via bench tool, the calibration maps correspond to the following structure:
* **Volumetric Efficiency (VE) & Speed Density**: 16x16 3D Table (RPM vs MAP kPa).
* **Fuel Target Lambda (Open-Loop / Closed-Loop Switch)**: 12x12 Table (Load vs RPM).
* **Ignition Timing Advance Base (Main Spark)**: 18x18 3D Table (°BTDC vs Load vs RPM).
* **MIVEC VVT Advance (Intake & Exhaust Cam Phasing)**: 14x14 3D Table.
* **DBW Throttle Request (Drive-by-Wire)**: Target Throttle Plate Opening vs Accelerator Pedal Angle (%).
* **CVT Torque Reduction / Protection Limits**: Maximum allowed engine torque during CVT lock-up and ratio shift.
