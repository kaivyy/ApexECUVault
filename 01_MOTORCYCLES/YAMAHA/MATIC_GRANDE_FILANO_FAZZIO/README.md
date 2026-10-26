# MATIC GRANDE FILANO FAZZIO - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/YAMAHA/MATIC_GRANDE_FILANO_FAZZIO`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `9 files` (7 binary dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MATIC_GRANDE_FILANO_FAZZIO` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2018–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `GRANDE_B8A0.bin` | **2022–2026** | 27.0 KB | `2cdade228ac30d2096f248eb314cae73` | Factory Binary Firmware Dump |
| `GRANDE_B8A1-40.bin` | **2022–2026** | 27.0 KB | `788c98fd2280b1b2daa0c4184c244216` | Factory Binary Firmware Dump |
| `GRANDE_B8A1.bin` | **2022–2026** | 27.0 KB | `eee65a0d8e12393078930a8405685020` | Factory Binary Firmware Dump |
| `GRANDE_B8B0.bin` | **2018–2024** | 27.0 KB | `b5ae5b01d21999e05f8fe74242fff56f` | Factory Binary Firmware Dump |
| `GRANDE_B8B0_31.bin` | **2018–2024** | 27.0 KB | `b5ae5b01d21999e05f8fe74242fff56f` | Factory Binary Firmware Dump |
| `GRANDE_B8B0_THAI.bin` | **2018–2024** | 27.0 KB | `b5ae5b01d21999e05f8fe74242fff56f` | Factory Binary Firmware Dump |
| `GRANDE_B8B1_41.bin` | **2018–2024** | 27.0 KB | `d5013e9e8047da2846f1b3947b0ec252` | Factory Binary Firmware Dump |
| `YAMAHA_B8A-H594A-00_Yamaha_Grand_Filano_Hybrid_(B8A0_B8B0).xdf` | **2022–2026** | 6.5 KB | `b66aa6c85862b4d492163f2b0619cc20` | TunerPro Binary Definition Map |
| `YAMAHA_BEJ-H594A-00_Yamaha_Fazzio_125_Hybrid_(BEJ0).xdf` | **2022–2026** | 6.5 KB | `b64df53f154da843a91173a8a9bd18d7` | TunerPro Binary Definition Map |

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
