# ALFA ROMEO 33 BOXER - Bosch Motronic ML4.1 Calibration Suite

**Repository Path**: `02_CARS/ALFA_ROMEO/ALFA_33_BOXER_MOTRONIC_ML4`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `3 files` (2 binary dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Koleksi berkas biner firmware asli (32,768 bytes) untuk unit ECU Bosch Motronic ML4.1 pada jajaran mesin legendaris Alfa Romeo Boxer 4-silinder (1.7L 8V & 16V) pada Alfa Romeo 33 (Type 905/907). Disertai dengan peta definisi TunerPro XDF komprehensif (33.xdf) untuk tuning kurva bahan bakar pengapian injeksi multi-point, dwell timing, cold start enrichment, dan rev limiter.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Bosch Motronic ML4.1 (Digital Engine Management)`
- **Arsitektur MCU & Memori**: `Intel 8051 / 8052 Microcontroller (27C256 / 27C512 32KB EPROM)`
- **Protokol Diagnostik & Flashing**: `Bosch 3-Pin Diagnostic K-Line / EPROM Programmer Read`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **OEM Part Numbers** (misal `0261xxxxxx`, `12587603`, `38770-xxx`, `23710-xxxxx`): Standar identifikasi universal pabrikan untuk ECU dan nomor perakitan modul.
- **Operating System / Software IDs** (misal `52373027`, `12592618`, `BG11_ECE_HS_008`, `PY3-A02`): Alamat dan software baseline pabrik yang tertanam di blok memori ROM.
- **TunerPro XDF Maps & A2L Definitions**: File deskriptor matematis yang memetakan offset memori hex ke unit engineering nyata (RPM, ms injeksi, derajat pengapian, kPa, persen bukaan katup).

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **EcuFlash**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `33.xdf` | `TunerPro Definition Map` | 263,039 | Definisi peta parameter kalibrasi TunerPro (263,039 bytes) untuk konversi skala dan offset tabel ECU |
| `Alfa_33_142.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Alfa_33_147.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, MAF/MAP Transfer Functions, Smoke Limiter, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance independen, High/Low Octane Timing Tables, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow, Boost & Cam Phasing**: Target Boost Pressure, Wastegate Duty Cycle (WGDC), Electronic Throttle Valve (Drive-by-Wire) Angle, dan Variable Cam Phasing (VANOS, VTC, VTEC).
- **Safety Limits & Thresholds**: Rev Limiter (Hard & Soft Cut), Top Speed Limiter (Vmax), Overboost Protection, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
