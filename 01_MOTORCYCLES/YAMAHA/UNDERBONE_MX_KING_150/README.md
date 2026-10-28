# UNDERBONE_MX_KING_150 - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/YAMAHA/UNDERBONE_MX_KING_150`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `9 files` (3 binary dumps, 6 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `UNDERBONE_MX_KING_150` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2015–2023

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `GENERATIONAL_B5V-H591A-00_Yamaha_Exciter_155_VVA___Sniper_155_V3_SmartKey_2021_2025.xdf` | **2021–2025** | 2.5 KB | `bd57c17363976768f3ea699ca8d8dbd1` | TunerPro Binary Definition Map |
| `GENERATIONAL_B5V-H591A-10_Yamaha_Exciter_155_VVA___Sniper_155_V3_Standard_Key_2021_2025.xdf` | **2021–2025** | 2.5 KB | `f1f508dc7e501e6d939f2adf1d9e768d` | TunerPro Binary Definition Map |
| `GENERATIONAL_BNV-H591A-01_Yamaha_Sniper_155_V4_VVA_SmartKey_2023_2025.xdf` | **2023–2025** | 2.5 KB | `21a149f69e3590fee5a62abf56d8618d` | TunerPro Binary Definition Map |
| `MX_KING_2PV1.bin` | **2015–2023** | 27.0 KB | `a705f0587831fe9525ce4872b64cdc95` | Factory Binary Firmware Dump |
| `MX_KING_B5V0.bin` | **2015–2023** | 27.0 KB | `81449ab4c9756c72adbe6a646fa49d0c` | Factory Binary Firmware Dump |
| `MX_KING_BKV1.bin` | **2015–2023** | 27.0 KB | `cbf24c22b2ad23c6923247b7dbfbd53f` | Factory Binary Firmware Dump |
| `YAMAHA_2PV-H591A-00_Yamaha_MX_King_150_V1_(2PV0).xdf` | **2015–2023** | 6.5 KB | `53734ac043c55586c373eb282464ad6f` | TunerPro Binary Definition Map |
| `YAMAHA_B5V-H591A-00_Yamaha_MX_King_150_V2_LED_(B5V0).xdf` | **2015–2023** | 6.5 KB | `0235d7e17b94f00105b57e81b3a7666b` | TunerPro Binary Definition Map |
| `YAMAHA_BKV-H591A-10_Yamaha_MX_King_150_(BKV1).xdf` | **2015–2023** | 6.5 KB | `a43267663c315a96a4c625e7c707583a` | TunerPro Binary Definition Map |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance, Low/High Octane Timing, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow & Boost Management**: Peta Target Boost Pressure, Wastegate Duty Cycle (WGDC), MAF/MAP Scaling, dan Throttle Response Curves.
- **Safety Limits & Thresholds**: Rev Limiter (Hard/Soft Cut), Top Speed Limiter (Vmax), Overboost Fuel Cut, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
