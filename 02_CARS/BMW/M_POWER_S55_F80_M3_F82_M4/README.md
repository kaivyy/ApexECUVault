# BMW M4 (F82 / F83) & M3 (F80) S55 3.0L Twin-Turbo Platform Dossier

> **Kategori Database**: [`02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/)  
> **Status Keaslian**: **100% Authentic Factory Flash Dumps & TunerPro Definitions**

---

## 1. Identitas Kendaraan & Spesifikasi Pabrikan

* **Nama Model Kendaraan**:
  * **BMW M4 Coupe** (Kode Sasis: `F82`)
  * **BMW M4 Convertible / Cabriolet** (Kode Sasis: `F83`)
  * **BMW M3 Sedan** (Kode Sasis: `F80`)
  * **BMW M2 Competition / CS** (Kode Sasis: `F87`)
  * **BMW M4 CS & M4 GTS** (High-Performance Factory Special Edition)
* **Tahun Produksi**: **2014 – 2020** (Pre-LCI & LCI Facelift)
* **Kode Mesin**: **BMW S55B30** / **S55B30A**
  * Konfigurasi: 3.0-Liter (2.979 cc) Inline-6 Twin-Turbocharged (Dual Mono-Scroll MHI Turbochargers)
  * Valvetrain: 24-Valve DOHC, Double-VANOS variable camshaft timing, Valvetronic throttle-less system
  * Rasio Kompresi: 10.2:1
  * Output Tenaga Standar:
    * Standard M3/M4: **425 HP (431 PS)** @ 5.500–7.300 RPM / **550 Nm** @ 1.850–5.500 RPM
    * Competition Package (ZCP): **444 HP (450 PS)** / **550 Nm**
    * M4 CS: **454 HP (460 PS)** / **600 Nm**
    * M4 GTS: **493 HP (500 PS)** (dengan sistem Water Injection) / **600 Nm**
* **Transmisi**:
  * 6-Speed Manual (GS6-53BZ) dengan rev-matching otomatis
  * 7-Speed Dual-Clutch M-DCT (Getrag GS7D36SG DKG) dengan Drivelogic

---

## 2. Spesifikasi ECU / DME Hardware

* **Tipe Komputer Mesin (DME)**: **Bosch MEVD17.2.G** (seri Motronic Electronic Throttle Gasoline Direct Injection)
* **Arsitektur Processor / MCU**: **Infineon TriCore TC1797** (32-bit RISC processor, 180 MHz core clock)
* **Kapasitas Flash ROM**: **4.194.304 bytes** (4 Megabytes / 4096 KB)
* **Antarmuka Komunikasi**: High-Speed CAN-Bus / FlexRay (Diagnostic OBD2 via Ethernet DoIP / CAN)
* **Metode Flashing & Tuning**:
  * OBD-II Direct Read & Write (Bootmod3, MHD Flasher, Alientech KESSv2 / KESS3, Autotuner, CMDFlash)
  * Password bypass via OBD2 tanpa perlu membongkar casing DME.

---

## 3. Daftar File Biner & Peta TunerPro XDF (Matching 1:1)

Semua file biner berukuran tepat **4.194.304 bytes (4MB)** dan memiliki pasangan file peta TunerPro (`.xdf`):

| Software ROM ID | File Biner Original (`.bin`) | File Multi-Map Switch (`.bin`) | Definisi TunerPro (`.xdf`) |
| :--- | :--- | :--- | :--- |
| **00000D07596401** | [`00000D07596401_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00000D07596401_original.bin) | [`00000D07596401_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00000D07596401_MapSwitchBase.bin) | [`00000D07596401.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00000D07596401.xdf) |
| **00000E2B3B0A01** | [`00000E2B3B0A01_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00000E2B3B0A01_original.bin) | [`00000E2B3B0A01_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00000E2B3B0A01_MapSwitchBase.bin) | [`00000E2B3B0A01.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00000E2B3B0A01.xdf) |
| **00000FEF81A001** | [`00000FEF81A001_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00000FEF81A001_original.bin) | [`00000FEF81A001_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00000FEF81A001_MapSwitchBase.bin) | [`00000FEF81A001.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00000FEF81A001.xdf) |
| **00001A841D1401** | [`00001A841D1401_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00001A841D1401_original.bin) | [`00001A841D1401_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00001A841D1401_MapSwitchBase.bin) | [`00001A841D1401.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00001A841D1401.xdf) |
| **00001A841D2801** | [`00001A841D2801_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00001A841D2801_original.bin) | [`00001A841D2801_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00001A841D2801_MapSwitchBase.bin) | [`00001A841D2801.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00001A841D2801.xdf) |
| **00001C41279601** | [`00001C41279601_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00001C41279601_original.bin) | [`00001C41279601_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00001C41279601_MapSwitchBase.bin) | [`00001C41279601.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00001C41279601.xdf) |
| **000021571D8202** | [`000021571D8202_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/000021571D8202_original.bin) | [`000021571D8202_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/000021571D8202_MapSwitchBase.bin) | [`000021571D8202.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/000021571D8202.xdf) |
| **000021571DAA01** | [`000021571DAA01_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/000021571DAA01_original.bin) | [`000021571DAA01_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/000021571DAA01_MapSwitchBase.bin) | [`000021571DAA01.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/000021571DAA01.xdf) |
| **000021571DBE01** | [`000021571DBE01_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/000021571DBE01_original.bin) | [`000021571DBE01_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/000021571DBE01_MapSwitchBase.bin) | [`000021571DBE01.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/000021571DBE01.xdf) |
| **00002DF2132801** | [`00002DF2132801_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00002DF2132801_original.bin) | [`00002DF2132801_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00002DF2132801_MapSwitchBase.bin) | [`00002DF2132801.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00002DF2132801.xdf) |
| **00005BA8134601** | [`00005BA8134601_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00005BA8134601_original.bin) | [`00005BA8134601_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00005BA8134601_MapSwitchBase.bin) | [`00005BA8134601.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00005BA8134601.xdf) |
| **00005BA8135001** | [`00005BA8135001_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00005BA8135001_original.bin) | [`00005BA8135001_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00005BA8135001_MapSwitchBase.bin) | [`00005BA8135001.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00005BA8135001.xdf) |
| **00005BA8135A01** | [`00005BA8135A01_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00005BA8135A01_original.bin) | [`00005BA8135A01_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS/00005BA8135A01_MapSwitchBase.bin) | [`00005BA8135A01.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS/00005BA8135A01.xdf) |

---

## 4. Parameter Peta yang Terbuka di TunerPro
* **Target Boost Pressure & Wastegate Duty Cycle (WGDC)**
* **Ignition Timing Advance Base & Knock Correction**
* **Fuel Target Lambda (Open-Loop AFR enrichment under WOT)**
* **Driver Demand Torque & Limiters (DCT Gear Protection)**
* **M Exhaust Burble / Overrun Fuel Cut Off Time**
* **Vmax Speed Limiter Delete (Unrestricted Top Speed)**
