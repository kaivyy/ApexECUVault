# BMW M4 (G82 / G83) & M3 (G80) S58 3.0L Twin-Turbo Platform Dossier

> **Kategori Database**: [`02_CARS/BMW/M_POWER_S58_G80_M3_M4/`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/)  
> **Status Keaslian**: **100% Authentic Factory Flash Dumps & TunerPro Definitions**

---

## 1. Identitas Kendaraan & Spesifikasi Pabrikan

* **Nama Model Kendaraan**:
  * **BMW M4 Coupe** (Kode Sasis: `G82`)
  * **BMW M4 Convertible / Cabriolet** (Kode Sasis: `G83`)
  * **BMW M3 Sedan** (Kode Sasis: `G80`)
  * **BMW M3 Touring** (Kode Sasis: `G81`)
  * **BMW M2 Coupe** (Kode Sasis: `G87`)
  * **BMW M4 Competition & M4 CSL** (Club Sport Light / Limited Edition)
  * **BMW X3 M / X4 M** (Kode Sasis: `F97` / `F98`)
* **Tahun Produksi**: **2020 – 2026** (Generasi Terbaru)
* **Kode Mesin**: **BMW S58B30T0**
  * Konfigurasi: 3.0-Liter (2.993 cc) Inline-6 Twin-Turbocharged (Mono-scroll twin turbocharges dengan cylinder head 3D-printed core)
  * Valvetrain: 24-Valve DOHC, Double-VANOS variable valve timing, Valvetronic variable valve lift
  * Rasio Kompresi: 9.3:1
  * Sistem Injeksi Bahan Bakar: High-Precision Direct Injection dengan tekanan hingga 350 bar
  * Output Tenaga Standar:
    * M3 / M4 Standard: **473 HP (480 PS)** @ 6.250 RPM / **550 Nm** @ 2.650–6.130 RPM
    * M3 / M4 Competition (RWD / M xDrive): **503 HP (510 PS)** / **650 Nm** @ 2.750–5.500 RPM
    * M4 CS (2024–2025): **543 HP (550 PS)** / **650 Nm**
    * M4 CSL (2022–2023): **543 HP (550 PS)** @ 6.250 RPM / **650 Nm**
* **Transmisi**:
  * 6-Speed Manual (GS6-53BZ)
  * 8-Speed M Steptronic Automatic dengan Drivelogic (transmisi ZF 8HP76)

---

## 2. Spesifikasi ECU / DME Hardware

* **Tipe Komputer Mesin (DME)**: **Bosch MG1CS024**
* **Arsitektur Processor / MCU**: **Infineon AURIX TC397 / TC3xx Family** (32-bit TriCore multi-core processor 300MHz, ASIL-D safety compliant)
* **Kapasitas Flash ROM**: **8.388.608 bytes** (Tepat 8 Megabytes / 8192 KB)
* **Antarmuka Komunikasi**: High-Speed Automotive CAN-FD & FlexRay (DoIP Ethernet)
* **Status Proteksi & Flashing**:
  * Unit produksi sebelum Juli 2020: Dapat di-flash via OBD-II (MHD, BM3, MG Flasher).
  * Unit produksi setelah Juli 2020 (Post-06/2020): Dilindungi hardware security lock. Membutuhkan prosedur *Bench Unlock* (Femto custom bootloader patch) sebelum OBD write dapat dibuka.

---

## 3. Daftar File Biner & Peta TunerPro XDF (Matching 1:1)

Semua file biner berukuran tepat **8.388.608 bytes (8MB)** dan memiliki pasangan file peta TunerPro (`.xdf`):

| Software ROM ID | File Biner Original (`.bin`) | File Multi-Map Switch (`.bin`) | Definisi TunerPro (`.xdf`) |
| :--- | :--- | :--- | :--- |
| **00005C640A6405** | [`00005C640A6405_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C640A6405_00005C640A6405_original.bin) | [`00005C640A6405_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C640A6405_00005C640A6405_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C640A6405.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C640A6405.xdf) |
| **00005C640A8205** | [`00005C640A8205_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C640A8205_00005C640A8205_original.bin) | [`00005C640A8205_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C640A8205_00005C640A8205_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C640A8205.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C640A8205.xdf) |
| **00005C640A8C05** | [`00005C640A8C05_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C640A8C05_00005C640A8C05_original.bin) | [`00005C640A8C05_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C640A8C05_00005C640A8C05_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C640A8C05.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C640A8C05.xdf) |
| **00005C64143206** | [`00005C64143206_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64143206_00005C64143206_original.bin) | [`00005C64143206_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64143206_00005C64143206_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C64143206.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C64143206.xdf) |
| **00005C64143C05** | [`00005C64143C05_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64143C05_00005C64143C05_original.bin) | [`00005C64143C05_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64143C05_00005C64143C05_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C64143C05.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C64143C05.xdf) |
| **00005C64144606** | [`00005C64144606_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64144606_00005C64144606_original.bin) | [`00005C64144606_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64144606_00005C64144606_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C64144606.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C64144606.xdf) |
| **00005C64145007** | [`00005C64145007_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64145007_00005C64145007_original.bin) | [`00005C64145007_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64145007_00005C64145007_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C64145007.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C64145007.xdf) |
| **00005C64145A05** | [`00005C64145A05_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64145A05_00005C64145A05_original.bin) | [`00005C64145A05_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64145A05_00005C64145A05_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C64145A05.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C64145A05.xdf) |
| **00005C64146E06** | [`00005C64146E06_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64146E06_00005C64146E06_original.bin) | [`00005C64146E06_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64146E06_00005C64146E06_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C64146E06.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C64146E06.xdf) |
| **00005C64148205** | [`00005C64148205_original.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64148205_00005C64148205_original.bin) | [`00005C64148205_MapSwitchBase.bin`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/00005C64148205_00005C64148205_MapSwitchBase.bin) | [`TUNERPRO_XDFS/00005C64148205.xdf`](file:///root/ecu_master_database/02_CARS/BMW/M_POWER_S58_G80_M3_M4/TUNERPRO_XDFS/00005C64148205.xdf) |

---

## 4. Parameter Peta yang Terbuka di TunerPro (S58 MG1CS024)
* **Boost Control**: Target Absolute Pressure (hPa/bar), WGDC Base Feedforward, Boost Limit ceiling.
* **Ignition Timing**: Optimal Engine Torque Spark Advance, Minimum Timing for Anti-Lag/Burble, Knock Retard Recovery.
* **Direct Fuel Injection**: Lambda Target Map (Closed-loop 1.0 stoichiometric transition to rich WOT enrichment), Rail Pressure Request (hingga 350 bar).
* **Torque Calculation Model**: Indicated Engine Torque, Maximum Clutch/Transmission Torque Thresholds (ZF 8HP76 torque limiter bypass).
* **Exhaust Flap Control & Burble Config**: WOT active valve angle, duration of pops & bangs overrun fuel injection.
