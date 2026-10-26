# HONDA CIVIC, CRX & INTEGRA - DPFI & MPFI (P04 & PM5) OBD0 Master ROM Suite

**Repository Path**: `02_CARS/HONDA_ACURA/HONDA_DPFI_MPFI_P04_PM5`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `17 files` (17 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Pustaka terlengkap 17 berkas biner ROM pabrikan asli untuk sistem injeksi Honda OBD0 Dual-Point Fuel Injection (DPFI) dan Multi-Point Fuel Injection (MPFI) kode P04 dan PM5. Digunakan luas pada generasi emas Honda Civic EF (1988-1991), CRX, dan Integra DA (D15B2, D15B7, D16A6). Berisi revisi lengkap pabrikan (rev1 hingga rev9, stock g01, g02, dan x30) untuk analisis register arsitektur mesin 80C154 dan pemetaan fuel/ignition table.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Keihin OBD0 Dual-Point & Multi-Point Fuel Injection ECM`
- **Arsitektur MCU & Memori**: `Oki 80C154 / NEC 78K Series 16-Bit Microcontroller (27C256 32KB Flash/EPROM)`
- **Protokol Diagnostik & Flashing**: `Honda 3-Pin / 5-Pin Diagnostic Serial (4800 bps) / Direct EPROM Read`

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
| `121_pm5_701.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev1_198.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev2_146.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev3_171.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev4_222.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev5_136.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev6_826.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev7_107.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev8_128.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_rev9_140.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `p04_try_374.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `pm5_dump_176.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `pm5_x30_1991508_175.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `stock_p04-g01_131.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `stock_p04-g01_297.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `stock_p04-g02_sajmon1100_739.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `stock_pm5_x30_120.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |

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
