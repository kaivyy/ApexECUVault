# Ferrari 360 Modena & 360 Challenge (ME7.3H4) Platform Dossier

> **Kategori Database**: [`02_CARS/FERRARI/FERRARI_360_MODENA_CHALLENGE_ME73/`](file:///root/ecu_master_database/02_CARS/FERRARI/FERRARI_360_MODENA_CHALLENGE_ME73/)  
> **Status Keaslian**: **100% Authentic Factory Flash Dumps** (Origin: `360trev/ME7RomTool_Ferrari`)

---

## 1. Identitas Kendaraan & Spesifikasi Pabrikan

* **Nama Model Kendaraan**:
  * **Ferrari 360 Modena** (Coupe)
  * **Ferrari 360 Spider** (Convertible)
  * **Ferrari 360 Challenge** (Factory Race Car)
  * **Ferrari 360 Challenge Stradale** (Lightweight Special Edition)
* **Tahun Produksi**: **1999 – 2005**
* **Kode Mesin**: **Ferrari Tipo F131** (3.6-Liter 90° V8 Flat-Plane Crankshaft)
  * Konfigurasi: 3.586 cc Naturally Aspirated V8, 5 katup per silinder (40 katup total), Dry Sump Lubrication
  * Redline: 8.500 RPM
  * Tenaga Maksimal:
    * Standard 360 Modena: **400 PS (395 HP)** @ 8.500 RPM / **373 Nm** @ 4.750 RPM
    * Challenge Stradale: **425 PS (419 HP)** @ 8.500 RPM
* **Transmisi**:
  * 6-Speed Manual gated shifter
  * 6-Speed F1 Electrohydraulic Paddle-Shift Automated Manual

---

## 2. Arsitektur ECU / DME Dual-Bank Master/Slave

Ferrari 360 menggunakan konfigurasi **Dual ECU independen**:
* **Bank Kiri (Silinder 1–4)**: Bosch Motronic ME7.3H4 ECU
* **Bank Kanan (Silinder 5–8)**: Bosch Motronic ME7.3H4 ECU
* **Nomor Part Bosch**: `0 261 204 841` (Ferrari Part No. `185403` / `180700`)
* **Processor**: Siemens / Infineon C167CR (16-bit RISC Automotive MCU)
* **Kapasitas Flash**: **524.288 bytes** (512 KB per bank)
* **Protokol Diagnostik & Flashing**: K-Line ISO 9141-2 / ME7 Boot Mode (K-TAG, Galletto, MPPS, ME7RomTool)

---

## 3. Daftar File Biner Asli di Database

| Nama File | Ukuran | SHA-256 Hash | Keterangan |
| :--- | :---: | :--- | :--- |
| [`Ferrari 360 Challenge.bin`](file:///root/ecu_master_database/02_CARS/FERRARI/FERRARI_360_MODENA_CHALLENGE_ME73/Ferrari%20360%20Challenge.bin) | 524.288 bytes (512 KB) | `c5efa59d5edb...` | Dump biner asli pabrikan Ferrari 360 Challenge Race Car (Bosch 0261204841) |
| [`LEFT_Eddie_2004_360Spider_EU.bin`](file:///root/ecu_master_database/02_CARS/FERRARI/FERRARI_360_MODENA_CHALLENGE_ME73/LEFT_Eddie_2004_360Spider_EU.bin) | 524.288 bytes (512 KB) | `c6a986f3fb9a...` | Dump biner asli pabrikan 2004 Ferrari 360 Spider EU (Bank Kiri / Left Bank) |

---

## 4. Parameter Utama Karakteristik Tuning Ferrari ME7.3H4
* **Variable Intake Plenum Geometry**: Kontrol katup resonansi intake manifold ganda pada 5.500 RPM.
* **Exhaust Bypass Valve**: Pengaturan pembukaan katup knalpot sport di RPM tinggi.
* **Ignition Advance & Knock Detection**: Peta pengapian sensitif per-silinder untuk flat-plane crank V8.
* **Rev Limiter (NMAX)**: Pengaturan batas putaran mesin hingga 8.700–9.000 RPM.
