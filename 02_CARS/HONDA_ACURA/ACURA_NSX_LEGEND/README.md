# ACURA NSX & LEGEND V6 - Factory Master Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/ACURA_NSX_LEGEND`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `19 files` (18 binary dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Koleksi master kalibrasi asli pabrikan Keihin untuk ikon supercar Acura NSX (NA1 3.0L C30A V6 VTEC) dan sedan mewah performa Acura Legend (KA7 / KA8 3.2L Type I 200 hp dan Type II 230 hp C32A). Mencakup firmware dump pabrik asli untuk transmisi manual dan otomatis (OEM NSX91M, NSX94, PY3-A02, PY3-A55, PY3-G52 European, PY3-Y52, PX9-A05, PX9-A57, JDM Type I, JDM Type II), dipasangkan secara presisi dengan TunerPro XDF definitions untuk kalibrasi VTEC crossover point, fuel delivery, dan ignition timing advance.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Keihin / Honda OBD1 3.0L & 3.2L V6 PGM-FI Engine Control Module`
- **Arsitektur MCU & Memori**: `Oki 66207 / 66507 16-Bit Engine Processor (27C256 32KB / 27C512 64KB EPROM)`
- **Protokol Diagnostik & Flashing**: `Honda 3-Pin & 5-Pin DLC Diagnostic Protocol / Direct EPROM Programmer Read`

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
| `Acura_NSX_and_Legend.xdf` | `TunerPro Definition Map` | 637,576 | Definisi peta parameter kalibrasi TunerPro (637,576 bytes) untuk konversi skala dan offset tabel ECU |
| `JDM Type I (PY3-902).BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `JDM Type II.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `NSX91M OEM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `NSX94M OEM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PR7-A03.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PR7-xxx.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PX9-A05, A15, A04, A55, A65.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PX9-A57, A67, L57, A17, A07.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PX9-L68 - California.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PY3-A02, A52.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PY3-A06, A53.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PY3-A55.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PY3-A57.BIN` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PY3-A58.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PY3-A72.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PY3-G52 European.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PY3-Y52 Guatemala.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Py3-A58 stock.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |

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
