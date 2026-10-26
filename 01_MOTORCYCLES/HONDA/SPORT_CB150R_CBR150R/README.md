# SPORT CB150R CBR150R - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/SPORT_CB150R_CBR150R`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `29 files` (3 binary dumps, 26 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SPORT_CB150R_CBR150R` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `38770-KPP-602.bin` | `.BIN` | `57,344` bytes | Honda Motorcycle Keihin ECU ROM `38770-KPP` |
| `38770-KPP-N02.bin` | `.BIN` | `57,344` bytes | Honda Motorcycle Keihin ECU ROM `38770-KPP` |
| `38770-KPP-T03.bin` | `.BIN` | `57,344` bytes | Honda Motorcycle Keihin ECU ROM `38770-KPP` |
| `GENERATIONAL_38770-K15-P01_Honda_All_New_CB150R_Streetfire_Gen_4_Inverted_Fork_(2021-2026).xdf` | `.XDF` | `5,585` bytes | Honda Motorcycle Keihin ECU ROM `38770-K15` |
| `GENERATIONAL_38770-K3B-N01_Honda_CB150X_Adventure_Touring_(2021-2026).xdf` | `.XDF` | `5,572` bytes | Honda Motorcycle Keihin ECU ROM `38770-K3B` |
| `GENERATIONAL_38770-K45-G01_Honda_CBR150R_Gen_3_Facelift_LED_(2016-2018).xdf` | `.XDF` | `5,555` bytes | Honda Motorcycle Keihin ECU ROM `38770-K45` |
| `GENERATIONAL_38770-K45-N01_Honda_CBR150R_Gen_2_Lokal_Dual_Eyes_(2014-2016).xdf` | `.XDF` | `5,547` bytes | Honda Motorcycle Keihin ECU ROM `38770-K45` |
| `GENERATIONAL_38770-K45-N41_Honda_CBR150R_Gen_4_Facelift_ABS_&_Emergency_Stop_(2018-2020).xdf` | `.XDF` | `5,575` bytes | Honda Motorcycle Keihin ECU ROM `38770-K45` |
| `GENERATIONAL_38770-K45-R01_Honda_All_New_CBR150R_Gen_5_Inverted_Fork_SFF-BP_(2021-2026).xdf` | `.XDF` | `5,599` bytes | Honda Motorcycle Keihin ECU ROM `38770-K45` |
| `HONDA_38770-K0A-A01_CB300R_Neo_Sports_Cafe_(2018-2024).xdf` | `.XDF` | `16,713` bytes | Honda Motorcycle Keihin ECU ROM `38770-K0A` |
| `HONDA_38770-K0A-R11_CB300R_Neo_Sports_Cafe_(2018-2024).xdf` | `.XDF` | `16,713` bytes | Honda Motorcycle Keihin ECU ROM `38770-K0A` |
| `HONDA_38770-K15-601_CB150R_Streetfire.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K15` |
| `HONDA_38770-K15-888_CB150R_Streetfire.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K15` |
| `HONDA_38770-K15-903_CB150R_Streetfire.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K15` |
| `HONDA_38770-K15-921_CB150R_Streetfire.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K15` |
| `HONDA_38770-K18-902_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K18` |
| `HONDA_38770-K18-941_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K18` |
| `HONDA_38770-K18-961_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K18` |
| `HONDA_38770-K33-D02_CBR300R___CB300F_(2014-2020).xdf` | `.XDF` | `16,715` bytes | Honda Motorcycle Keihin ECU ROM `38770-K33` |
| `HONDA_38770-K33-D22_CBR300R___CB300F_(2014-2020).xdf` | `.XDF` | `16,715` bytes | Honda Motorcycle Keihin ECU ROM `38770-K33` |
| `HONDA_38770-K33-N03_CBR300R___CB300F_(2014-2020).xdf` | `.XDF` | `16,715` bytes | Honda Motorcycle Keihin ECU ROM `38770-K33` |
| `HONDA_38770-K45-N01_CBR150R_LED_(2016-2024).xdf` | `.XDF` | `16,702` bytes | Honda Motorcycle Keihin ECU ROM `38770-K45` |
| `HONDA_38770-K45-N42_CBR150R_LED_(2016-2024).xdf` | `.XDF` | `16,702` bytes | Honda Motorcycle Keihin ECU ROM `38770-K45` |
| `HONDA_38770-K45-NA1_CBR150R_LED_(2016-2024).xdf` | `.XDF` | `16,702` bytes | Honda Motorcycle Keihin ECU ROM `38770-K45` |
| `HONDA_38770-K94-T02_CBR150R_(Indonesia).xdf` | `.XDF` | `16,698` bytes | Honda Motorcycle Keihin ECU ROM `38770-K94` |
| `HONDA_38770-K98-E02_CB150R_Neo_Sports_Cafe_(2017-2024).xdf` | `.XDF` | `16,713` bytes | Honda Motorcycle Keihin ECU ROM `38770-K98` |
| `HONDA_38770-KPP-602_CBR150R_(2011-2015).xdf` | `.XDF` | `16,694` bytes | Honda Motorcycle Keihin ECU ROM `38770-KPP` |
| `HONDA_38770-KPP-N02_CBR150R_(2011-2015).xdf` | `.XDF` | `16,694` bytes | Honda Motorcycle Keihin ECU ROM `38770-KPP` |
| `HONDA_38770-KPP-T03_CBR150R_(2011-2015).xdf` | `.XDF` | `16,694` bytes | Honda Motorcycle Keihin ECU ROM `38770-KPP` |

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
