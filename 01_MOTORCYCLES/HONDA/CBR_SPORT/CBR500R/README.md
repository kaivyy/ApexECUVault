# CBR500R - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/CBR_SPORT/CBR500R`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `9 files` (7 binary dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CBR500R` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2013–2023

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `38770-MGZ-A03.bin` | **2013–2023** | 256.0 KB | `f6a6d9cebc04702d2b2b6ea9e79285fb` | Factory Binary Firmware Dump |
| `38770-MGZ-C02.bin` | **2013–2023** | 256.0 KB | `40e29ed018bf30a2f0d4c67a6111cbd4` | Factory Binary Firmware Dump |
| `38770-MGZ-C03.bin` | **2013–2023** | 256.0 KB | `f6ecaefc0067babc704fa442e54d7184` | Factory Binary Firmware Dump |
| `38770-MGZ-D02.bin` | **2013–2023** | 256.0 KB | `541fbc35987007aa9834cd070d71cab6` | Factory Binary Firmware Dump |
| `38770-MGZ.xdf` | **2013–2023** | 26.9 KB | `e35c3132febb369200d7a54bbe120e87` | TunerPro Binary Definition Map |
| `38770-MJW-AQ1.bin` | **2013–2023** | 256.0 KB | `5b69fdd34ab97f0546e87b12a2613242` | Factory Binary Firmware Dump |
| `38770-MJW-DR1.bin` | **2013–2023** | 256.0 KB | `1827b58adfcdb7cf7fb89a4b07ebae41` | Factory Binary Firmware Dump |
| `38770-MJW-T11.bin` | **2013–2023** | 256.0 KB | `16d661c881f6d4694eedb0aab93cfab3` | Factory Binary Firmware Dump |
| `38770-MJW.xdf` | **2013–2023** | 71.7 KB | `8e5d477d5a174cc1f394ccbadb209698` | TunerPro Binary Definition Map |

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
