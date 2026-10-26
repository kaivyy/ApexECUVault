# XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/LS_V8_P01_P59/XDFS`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `35 files` (0 binary dumps, 35 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `12202088 - 2001 512k.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12202088` |
| `12208322 - 2001 512k.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12208322` |
| `12209203 - 2002 512k V1.xdf` | `.XDF` | `602,221` bytes | General Motors Operating System ID `12209203` |
| `12212156 - 2002 512k V1.xdf` | `.XDF` | `602,206` bytes | General Motors Operating System ID `12212156` |
| `12216125_TCS.xdf` | `.XDF` | `695` bytes | General Motors Operating System ID `12216125` |
| `12587603 - 2004 1mb.xdf` | `.XDF` | `801,440` bytes | General Motors Operating System ID `12587603` |
| `12592433-imperial.xdf` | `.XDF` | `619,252` bytes | General Motors Operating System ID `12592433` |
| `12592433-metric.xdf` | `.XDF` | `611,995` bytes | General Motors Operating System ID `12592433` |
| `No Password - OS12212156 - 2002 512kB PCM - v5_old.xdf` | `.XDF` | `1,272,938` bytes | General Motors Operating System ID `12212156` |
| `No Password - Operating System 12202088 - 512Kb PCM - 2001 model year.xdf` | `.XDF` | `620,841` bytes | General Motors Operating System ID `12202088` |
| `No Password - Operating System 12208322 - 512Kb PCM - 2001 model year.xdf` | `.XDF` | `620,841` bytes | General Motors Operating System ID `12208322` |
| `No Password - Operating System 12209203 - 512Kb PCM - 2002 model year.xdf` | `.XDF` | `618,128` bytes | General Motors Operating System ID `12209203` |
| `No Password - Operating System 12216125 - 512Kb PCM - 2002 model year - 5.3L Flex Fuel and 8.1L engines.xdf` | `.XDF` | `643,408` bytes | General Motors Operating System ID `12216125` |
| `No Password - Operating System 12221588 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | `.XDF` | `623,195` bytes | General Motors Operating System ID `12221588` |
| `No Password - Operating System 12225074 - 512Kb PCM - 2001 to 2004 Holden model years.xdf` | `.XDF` | `618,194` bytes | General Motors Operating System ID `12225074` |
| `No Password - Operating System 12587603 - 1Mb PCM - 2004 model year.xdf` | `.XDF` | `631,750` bytes | General Motors Operating System ID `12587603` |
| `No Password - Operating System 12593358 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | `.XDF` | `623,195` bytes | General Motors Operating System ID `12593358` |
| `No Password - XDF for Operating System 12202088 - 2001 512Kb PCM - Version 5.xdf` | `.XDF` | `632,026` bytes | General Motors Operating System ID `12202088` |
| `No Password - XDF for Operating System 12208322 - 2001 512Kb PCM - Version 5.xdf` | `.XDF` | `632,026` bytes | General Motors Operating System ID `12208322` |
| `No Password - __Operating System 12212156 - 512Kb PCM - 2002 model year.xdf` | `.XDF` | `618,112` bytes | General Motors Operating System ID `12212156` |
| `OS12212156 - 2002 512kB PCM - v5_old.xdf` | `.XDF` | `1,273,255` bytes | General Motors Operating System ID `12212156` |
| `OS12212156 - 2002 512kB PCM - v6 - no password.xdf` | `.XDF` | `1,687,463` bytes | General Motors Operating System ID `12212156` |
| `Operating System 12202088 - 512Kb PCM - 2001 model year.xdf` | `.XDF` | `621,149` bytes | General Motors Operating System ID `12202088` |
| `Operating System 12208322 - 512Kb PCM - 2001 model year.xdf` | `.XDF` | `621,149` bytes | General Motors Operating System ID `12208322` |
| `Operating System 12209203 - 512Kb PCM - 2002 model year.xdf` | `.XDF` | `618,436` bytes | General Motors Operating System ID `12209203` |
| `Operating System 12216125 - 512Kb PCM - 2002 model year - 5.3L Flex Fuel and 8.1L engines.xdf` | `.XDF` | `643,716` bytes | General Motors Operating System ID `12216125` |
| `Operating System 12221588 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | `.XDF` | `623,503` bytes | General Motors Operating System ID `12221588` |
| `Operating System 12225074 - 512Kb PCM - 2001 to 2004 Holden model years.xdf` | `.XDF` | `618,502` bytes | General Motors Operating System ID `12225074` |
| `Operating System 12587603 - 1Mb PCM - 2004 model year.xdf` | `.XDF` | `632,058` bytes | General Motors Operating System ID `12587603` |
| `Operating System 12593358 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | `.XDF` | `623,503` bytes | General Motors Operating System ID `12593358` |
| `P01_512Kb_Experimental-Need_Testing_OS_12202088_12202088 - 2001 512k.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12202088` |
| `P01_512Kb_Experimental-Need_Testing_OS_12208322_12208322 - 2001 512k.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12208322` |
| `XDF for Operating System 12202088 - 2001 512Kb PCM - Version 5.xdf` | `.XDF` | `632,321` bytes | General Motors Operating System ID `12202088` |
| `XDF for Operating System 12208322 - 2001 512Kb PCM - Version 5.xdf` | `.XDF` | `632,321` bytes | General Motors Operating System ID `12208322` |
| `~~Operating System 12212156 - 512Kb PCM - 2002 model year.xdf` | `.XDF` | `618,420` bytes | General Motors Operating System ID `12212156` |

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
