# ImperialUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/N63 S63/Generic/ImperialUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `27 files` (0 binary dumps, 27 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ImperialUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2015–2026

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `H4C99274B_4acf-010_050_004.ImperialUnits.xdf` | **2015–2026** | 776.1 KB | `91c10396e5f3d36666fa03e8ecb801aa` | TunerPro Binary Definition Map |
| `H4C993A3B_4acf-020_120_003.ImperialUnits.xdf` | **2015–2026** | 849.8 KB | `08d8422efcb8c5f271f9dbebf78c2b5b` | TunerPro Binary Definition Map |
| `H4C99695B_4acf-030_110_005.ImperialUnits.xdf` | **2015–2026** | 869.8 KB | `25fddb499627da9e17e8ed9578a05d1b` | TunerPro Binary Definition Map |
| `H4C996B5B_4acf-030_120_005.ImperialUnits.xdf` | **2015–2026** | 869.8 KB | `25fddb499627da9e17e8ed9578a05d1b` | TunerPro Binary Definition Map |
| `H4C996H5B_4acf-030_150_005.ImperialUnits.xdf` | **2015–2026** | 869.8 KB | `256c76f20f14161265fb9e100d22a82d` | TunerPro Binary Definition Map |
| `H4C996K5B_4acf-030_160_005.ImperialUnits.xdf` | **2015–2026** | 869.8 KB | `0388317d4c006e506e6511e79be78129` | TunerPro Binary Definition Map |
| `H4C996K6B_4acf-030_160_006.ImperialUnits.xdf` | **2015–2026** | 869.8 KB | `0388317d4c006e506e6511e79be78129` | TunerPro Binary Definition Map |
| `H4C996P5B_4acf-030_170_005.ImperialUnits.xdf` | **2015–2026** | 869.8 KB | `adb71f781419d0e978dd3a4b6bce72f7` | TunerPro Binary Definition Map |
| `H4C996R5B_4acf-030_180_073.ImperialUnits.xdf` | **2015–2026** | 869.8 KB | `56875b213a4b6778f0f196dafd0f218f` | TunerPro Binary Definition Map |
| `H4C9L8A5B_4acf-040_110_005.ImperialUnits.xdf` | **2015–2026** | 890.4 KB | `059e5eb52bd039c6a5818df1f8c5a7e5` | TunerPro Binary Definition Map |
| `H4C9L8E6B_4acf-040_120_006.ImperialUnits.xdf` | **2015–2026** | 890.4 KB | `03fca25f9b55fb32be45d727b84a1fe9` | TunerPro Binary Definition Map |
| `H4C9L8J5B_4acf-040_130_005.ImperialUnits.xdf` | **2015–2026** | 890.4 KB | `63a2197db431afe50acdb88867bda36d` | TunerPro Binary Definition Map |
| `H4C9L8N5B_4acf-040_150_005.ImperialUnits.xdf` | **2015–2026** | 890.4 KB | `c4694d114a54449584bb085d96bc73aa` | TunerPro Binary Definition Map |
| `V4C9F4K6B_4963-040_170_006.ImperialUnits.xdf` | **2015–2026** | 870.1 KB | `01dc4599860daede89d8d01772a9049d` | TunerPro Binary Definition Map |
| `V4C9F4N6B_4963-040_180_006.ImperialUnits.xdf` | **2015–2026** | 870.1 KB | `c5dd6a0faa7cc3d8812cd1d76b2e599d` | TunerPro Binary Definition Map |
| `V4C9H6H6B_4963-060_130_006.ImperialUnits.xdf` | **2015–2026** | 904.2 KB | `0c90c32fb976339dcc6b884d60635eab` | TunerPro Binary Definition Map |
| `V4C9H6N7B_4963-060_150_007.ImperialUnits.xdf` | **2015–2026** | 904.2 KB | `063668d0771ce0fe1b9205360e3e70e7` | TunerPro Binary Definition Map |
| `V4C9H6S8B_4963-060_170_008.ImperialUnits.xdf` | **2015–2026** | 904.2 KB | `761906db30f7f39754346978582b2427` | TunerPro Binary Definition Map |
| `V4C9J717B_4963-070_030_007.ImperialUnits.xdf` | **2015–2026** | 913.8 KB | `baef6ef026d8aa0b03448535075058c9` | TunerPro Binary Definition Map |
| `V4C9J796B_4963-070_060_006.ImperialUnits.xdf` | **2015–2026** | 913.8 KB | `1d1b1c7acc3e856df5a54be9aa2a8930` | TunerPro Binary Definition Map |
| `V4C9J7A5B_4963-070_070_005.ImperialUnits.xdf` | **2015–2026** | 913.8 KB | `26c13c1f3354ae896391d9fd2aa17979` | TunerPro Binary Definition Map |
| `V4C9J7N6B_4963-070_080_006.ImperialUnits.xdf` | **2015–2026** | 913.8 KB | `4d8caf6ab17346d2e7f3388b8b3fd11c` | TunerPro Binary Definition Map |
| `V4C9J7S8B_4963-070_100_008.ImperialUnits.xdf` | **2015–2026** | 913.8 KB | `7742301a7659625495ba62c7e68b7e2e` | TunerPro Binary Definition Map |
| `V4C9J7V5B_4963-070_120_005.ImperialUnits.xdf` | **2015–2026** | 913.8 KB | `71a27684374e103feab9782e6fce0e4f` | TunerPro Binary Definition Map |
| `V4C9J7W5B_4963-070_130_005.ImperialUnits.xdf` | **2015–2026** | 913.8 KB | `71a27684374e103feab9782e6fce0e4f` | TunerPro Binary Definition Map |
| `V4C9L8N6B_4963-080_060_006.ImperialUnits.xdf` | **2015–2026** | 901.5 KB | `996e83a3e2c2603270cf19bfcb101c53` | TunerPro Binary Definition Map |
| `V4C9L8S9B_4963-080_080_009.ImperialUnits.xdf` | **2015–2026** | 901.5 KB | `97d855f711cd427595a294adefd8dba7` | TunerPro Binary Definition Map |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro yang tersedia, struktur kalibrasi mencakup parameter esensial:
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
