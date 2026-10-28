# XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/NISSAN_INFINITI/XDFS`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `13 files` (0 binary dumps, 13 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `B13RT.xdf` | **2000–2024** | 55.7 KB | `a0006e906bbe90d014633bbbc039d198` | TunerPro Binary Definition Map |
| `Infinity_M30_90_92.xdf` | **1990–1992** | 34.8 KB | `b1630ec489830f7defbad263058e335a` | TunerPro Binary Definition Map |
| `Q45.xdf` | **2000–2024** | 70.6 KB | `99e8aea351928ae6cf6cc999ae18800e` | TunerPro Binary Definition Map |
| `Q4516bit.xdf` | **2000–2024** | 69.4 KB | `ac1473035ba48b95b3eaf3f95b04f943` | TunerPro Binary Definition Map |
| `RB20det.xdf` | **2000–2024** | 63.2 KB | `e38a481986a9f7d257cca8258c61220c` | TunerPro Binary Definition Map |
| `S13RT.xdf` | **2000–2024** | 122.4 KB | `571f97764da3c17de15dd706858f65ce` | TunerPro Binary Definition Map |
| `U13-93-94-Altima-240sx.xdf` | **2000–2024** | 127.8 KB | `459739ee5fef532adf6f4f4cc29db51b` | TunerPro Binary Definition Map |
| `U13-96-240sx-Altima.xdf` | **2000–2024** | 95.9 KB | `b18f48fcf94d8887f749f2e6a9c3ec1b` | TunerPro Binary Definition Map |
| `Z31.xdf` | **2000–2024** | 30.3 KB | `291de52e361518ebe13f52c2c436e364` | TunerPro Binary Definition Map |
| `Z32.xdf` | **2000–2024** | 61.0 KB | `cbdd92027f7e92e65503f7e2192cd567` | TunerPro Binary Definition Map |
| `Z32_512.xdf` | **2000–2024** | 71.3 KB | `295232210b9c374fa0b5daf3a2727fe1` | TunerPro Binary Definition Map |
| `ca18det_v2.xdf` | **2000–2024** | 37.8 KB | `4ffe18a32986a82712e9e8f1c6fec6f3` | TunerPro Binary Definition Map |
| `sr20ve.xdf` | **2000–2024** | 69.9 KB | `fd60ec05379a1ddb4e8bbb13fbd5f2a9` | TunerPro Binary Definition Map |

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
