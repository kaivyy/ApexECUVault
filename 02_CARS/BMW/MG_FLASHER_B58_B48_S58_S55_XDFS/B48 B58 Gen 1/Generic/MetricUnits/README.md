# MetricUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Generic/MetricUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `35 files` (0 binary dumps, 35 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MetricUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `R0C9J8B2B_3081-080_017_002.MetricUnits.xdf` | `.XDF` | `995,552` bytes | TunerPro Binary Definition Map |
| `R0C9J8D2B_3081-080_021_002.MetricUnits.xdf` | `.XDF` | `995,552` bytes | TunerPro Binary Definition Map |
| `R0C9J8I2B_3081-080_029_002.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9J8I3B_3081-080_029_003.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9J8I4B_3081-080_029_004.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9J962B_3081-090_010_002.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9J9E3B_3081-090_020_003.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9J9E4B_3081-090_020_004.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9JA05B_3081-090_025_005.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9JA15B_3081-090_030_005.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9JC05B_3081-090_050_005.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9JD06B_3081-090_060_006.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0C9JE15B_3081-090_080_005.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0R96015B_7706-000_007_005.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0R96025B_7706-000_008_005.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R0R9A005B_7706-000_011_005.MetricUnits.xdf` | `.XDF` | `995,551` bytes | TunerPro Binary Definition Map |
| `R1C9I562B_3076-050_006_002.MetricUnits.xdf` | `.XDF` | `925,250` bytes | TunerPro Binary Definition Map |
| `R1C9J772B_3076-070_009_002.MetricUnits.xdf` | `.XDF` | `983,240` bytes | TunerPro Binary Definition Map |
| `R1C9J8B2B_3076-080_017_002.MetricUnits.xdf` | `.XDF` | `994,992` bytes | TunerPro Binary Definition Map |
| `R1C9J8B3B_3076-080_017_003.MetricUnits.xdf` | `.XDF` | `994,992` bytes | TunerPro Binary Definition Map |
| `R1C9J8D3B_3076-080_018_003.MetricUnits.xdf` | `.XDF` | `994,992` bytes | TunerPro Binary Definition Map |
| `R1C9J8G3B_3428-000_001_001.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9J8I2B_3076-080_029_002.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9J8I7B_3076-080_029_007.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9J962B_3076-090_010_002.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9J9E3B_3076-090_020_003.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9J9E5B_3076-090_020_005.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9J9E7B_3076-090_020_007.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9JA05B_3076-090_025_005.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9JC05B_3076-090_050_005.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9JD06B_3076-090_060_006.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1C9JE15B_3076-090_080_005.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1R95005B_7972-000_005_005.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `R1R96015B_7972-000_007_005.MetricUnits.xdf` | `.XDF` | `994,991` bytes | TunerPro Binary Definition Map |
| `V0C9J6J2B_3125-065_027_002.MetricUnits.xdf` | `.XDF` | `843,412` bytes | TunerPro Binary Definition Map |

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
