# v7.3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.3`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `26 files` (0 binary dumps, 26 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.3` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `R0C9J8B2B_3081-080_017_002_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9J8D2B_3081-080_021_002_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9J8I2B_3081-080_029_002_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9J8I3B_3081-080_029_003_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9J8I4B_3081-080_029_004_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9J962B_3081-090_010_002_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9J9E3B_3081-090_020_003_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9J9E4B_3081-090_020_004_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9JA05B_3081-090_025_005_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9JA15B_3081-090_030_005_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9JC05B_3081-090_050_005_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9JD06B_3081-090_060_006_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R0C9JE15B_3081-090_080_005_v7.3.xdf` | `.XDF` | `2,819,235` bytes | TunerPro Binary Definition Map |
| `R1C9I562B_3076-050_006_002_v7.3.xdf` | `.XDF` | `2,724,085` bytes | TunerPro Binary Definition Map |
| `R1C9J8B2B_3076-080_017_002_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9J8B3B_3076-080_017_003_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9J8I2B_3076-080_029_002_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9J8I7B_3076-080_029_007_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9J962B_3076-090_010_002_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9J9E3B_3076-090_020_003_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9J9E5B_3076-090_020_005_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9J9E7B_3076-090_020_007_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9JA05B_3076-090_025_005_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9JC05B_3076-090_050_005_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9JD06B_3076-090_060_006_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |
| `R1C9JE15B_3076-090_080_005_v7.3.xdf` | `.XDF` | `2,819,182` bytes | TunerPro Binary Definition Map |

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
