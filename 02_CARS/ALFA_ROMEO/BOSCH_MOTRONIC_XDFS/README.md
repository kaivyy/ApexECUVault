# BOSCH MOTRONIC XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/ALFA_ROMEO/BOSCH_MOTRONIC_XDFS`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `29 files` (0 binary dumps, 29 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `BOSCH_MOTRONIC_XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `145_1.4_16V_TS_0261204481_1037358388.xdf` | `.XDF` | `459,610` bytes | Bosch Motronic Hardware ID `0261204481` |
| `145_1.6_16V_TS_0261200695_1267358244.xdf` | `.XDF` | `379` bytes | Bosch Motronic Hardware ID `0261200695` |
| `145_1.7_16V_0261203354_1267358146.xdf` | `.XDF` | `124,326` bytes | Bosch Motronic Hardware ID `0261203354` |
| `145_1.7_16V_0261203849_358699.xdf` | `.XDF` | `127,918` bytes | Bosch Motronic Hardware ID `0261203849` |
| `145_2.0_16V_TS_0261204478_1037358492.xdf` | `.XDF` | `172,604` bytes | Bosch Motronic Hardware ID `0261204478` |
| `155_1.7_TS_0261200536_1267357669.xdf` | `.XDF` | `174,531` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_1.8_16V_TS_0261203846_1267358560.xdf` | `.XDF` | `148,958` bytes | Bosch Motronic Hardware ID `0261203846` |
| `155_1.8_16V_TS_0261204168_355197.xdf` | `.XDF` | `172,482` bytes | Bosch Motronic Hardware ID `0261204168` |
| `155_1.8_TS_0261200536_1267356588.xdf` | `.XDF` | `187,477` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_1.8_TS_0261200536_1267357151.xdf` | `.XDF` | `187,488` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_1.8_TS_0261200536_1267357963.xdf` | `.XDF` | `178,714` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_2.0_16V_TS_0261203862_355410.xdf` | `.XDF` | `159,408` bytes | Bosch Motronic Hardware ID `0261203862` |
| `155_2.0_16V_TS_0261203993_355908.xdf` | `.XDF` | `159,450` bytes | Bosch Motronic Hardware ID `0261203993` |
| `155_2.0_TS_0261200536_1267357094.xdf` | `.XDF` | `187,510` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_2.0_TS_0261200536_1267357151.xdf` | `.XDF` | `187,488` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_2.0_TS_0261200536_1267357669.xdf` | `.XDF` | `174,531` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_2.5_V6_0261200537_1267356596.xdf` | `.XDF` | `108,630` bytes | Bosch Motronic Hardware ID `0261200537` |
| `155_2.5_V6_0261203829_1267358578.xdf` | `.XDF` | `131,243` bytes | Bosch Motronic Hardware ID `0261203829` |
| `164_2.0_TS_0261200108_1267355452.xdf` | `.XDF` | `221,766` bytes | Bosch Motronic Hardware ID `0261200108` |
| `164_2.0_TS_0261200108_1267355604.xdf` | `.XDF` | `221,818` bytes | Bosch Motronic Hardware ID `0261200108` |
| `164_2.0_TS_0261200108_1267356191.xdf` | `.XDF` | `221,851` bytes | Bosch Motronic Hardware ID `0261200108` |
| `164_3.0_12V_0261200117_1267355710.xdf` | `.XDF` | `218,444` bytes | Bosch Motronic Hardware ID `0261200117` |
| `164_3.0_12V_0261200117_1267356096.xdf` | `.XDF` | `217,659` bytes | Bosch Motronic Hardware ID `0261200117` |
| `164_3.0_12V_0261200117_1267356310.xdf` | `.XDF` | `217,659` bytes | Bosch Motronic Hardware ID `0261200117` |
| `75_3.0_12V_0261200141_1267356097.xdf` | `.XDF` | `211,491` bytes | Bosch Motronic Hardware ID `0261200141` |
| `GTV_2.0_16V_TS_0261203671_355934.xdf` | `.XDF` | `159,425` bytes | Bosch Motronic Hardware ID `0261203671` |
| `GTV_2.0_V6_TURBO_0261203869_1267358696.xdf` | `.XDF` | `145,136` bytes | Bosch Motronic Hardware ID `0261203869` |
| `GTV_2.0_V6_TURBO_0261203883_1037358648.xdf` | `.XDF` | `145,594` bytes | Bosch Motronic Hardware ID `0261203883` |
| `SZ_3.0_12V_0261200141_1267355737.xdf` | `.XDF` | `211,675` bytes | Bosch Motronic Hardware ID `0261200141` |

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
