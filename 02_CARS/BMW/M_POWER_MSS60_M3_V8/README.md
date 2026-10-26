# BMW M3 (E90 / E92 / E93) - Siemens MSS60 DME S65B40 V8 Master Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_MSS60_M3_V8`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `16 files` (14 binary dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Koleksi master kalibrasi resmi pabrikan Siemens MSS60 Digital Motor Electronics untuk mesin legendaris BMW S65B40 4.0-liter naturally aspirated V8 (414 hp / 420 PS, 8,400 RPM redline) pada platform BMW M3 generasi E90 Sedan, E92 Coupe, dan E93 Convertible (spesifikasi pasar ECE Eropa dan US Amerika Utara). Mencakup berkas biner kalibrasi bertenaga penuh (.hex) untuk subsistem pengapian (IGN) dan injeksi (INJ), serta dilengkapi dengan berkas definisi standar industri ASAP2 A2L resmi pabrikan (inj.a2l dan ign.a2l) untuk pemetaan presisi individual throttle bodies (ITB), Double-VANOS variable valve timing, knock sensing via ion-current technology, rev limiter 8,400 RPM, dan pemetaan launch control.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Siemens MSS60 Dual-Core High Performance DME`
- **Arsitektur MCU & Memori**: `Dual Motorola / Freescale MPC563 / MPC564 32-Bit PowerPC (5MB+ External Flash)`
- **Protokol Diagnostik & Flashing**: `BMW DS2 / K-Line / D-CAN (ISO 15765-4 500kbps UDS) / BDM Bootmode`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **OEM Part Numbers** (misal `0261xxxxxx`, `12587603`, `38770-xxx`, `23710-xxxxx`): Standar identifikasi universal pabrikan untuk ECU dan nomor perakitan modul.
- **Operating System / Software IDs** (misal `52373027`, `12592618`, `BG11_ECE_HS_008`, `PY3-A02`): Alamat dan software baseline pabrik yang tertanam di blok memori ROM.
- **TunerPro XDF Maps & A2L Definitions**: File deskriptor matematis yang memetakan offset memori hex ke unit engineering nyata (RPM, ms injeksi, derajat pengapian, kPa, persen bukaan katup).

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **EcuFlash**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2007–2013

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `IGN_E90_BG11_ECE_HS_008 _530_2_ign_4.hex` | **2006–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_ECE_HS_009 _530_3_ign_.hex` | **2006–2013** | 5.11 MB | `247a98e2367b0443c1231d7a61602f52` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_ECE_HS_009 _530_3_ign__1.hex` | **2006–2013** | 5.11 MB | `247a98e2367b0443c1231d7a61602f52` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_008 _530_2_ign.hex` | **2006–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_008 _530_2_ign_1.hex` | **2006–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_011 _530_3_2710_ign_1.hex` | **2006–2013** | 5.11 MB | `553690b2f051ba0f87128c4f3cc13764` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_011 _530_3_2710_ign_2.hex` | **2006–2013** | 5.11 MB | `b5e7a7ec47530bd6d65d114d2744d732` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_ECE_HS_008 _530_2_inj_4.hex` | **2006–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_ECE_HS_009 _530_3_inj_.hex` | **2006–2013** | 5.11 MB | `e9ccb7c7a970aac780a21e1bb1eaa5e4` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_ECE_HS_009 _530_3_inj__1.hex` | **2006–2013** | 5.11 MB | `e9ccb7c7a970aac780a21e1bb1eaa5e4` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_008 _530_2_inj.hex` | **2006–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_008 _530_2_inj_1.hex` | **2006–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_011 _530_3_2710_inj_1.hex` | **2006–2013** | 5.11 MB | `be9ef94f82f46babd2f6eccf16b2b13c` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_011 _530_3_2710_inj_2.hex` | **2006–2013** | 5.11 MB | `be9ef94f82f46babd2f6eccf16b2b13c` | Intel HEX Calibration Firmware |
| `ign.a2l` | **2007–2013** | 3.00 MB | `60868050e5271b20634816729a858e78` | ECU / ASAP2 Calibration Map Definition |
| `inj.a2l` | **2007–2013** | 3.99 MB | `1ad46d85e8b34d60e8a7c9ed30da6bbc` | ECU / ASAP2 Calibration Map Definition |

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
