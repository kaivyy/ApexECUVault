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

* **Rentang Tahun / Model Year**: 1988–1991

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `121_pm5_701.bin` | **1988–1991** | 16.0 KB | `c1a71ffe1a0d2c9e913699e6cb8ac208` | Factory Binary Firmware Dump |
| `p04_rev1_198.bin` | **1988–1991** | 32.0 KB | `244bfe94a3d5306b9322a98f017d4abb` | Factory Binary Firmware Dump |
| `p04_rev2_146.bin` | **1988–1991** | 32.0 KB | `fe8e425c4f3243323b73939a9b9d60ec` | Factory Binary Firmware Dump |
| `p04_rev3_171.bin` | **1988–1991** | 32.0 KB | `3dd1c56685f3b81b8e9ab5678ddd4520` | Factory Binary Firmware Dump |
| `p04_rev4_222.bin` | **1988–1991** | 32.0 KB | `e22cc549a8ab2751bfa7e5aa54132081` | Factory Binary Firmware Dump |
| `p04_rev5_136.bin` | **1988–1991** | 32.0 KB | `3ead4169c18df94a05729a5f34270c5e` | Factory Binary Firmware Dump |
| `p04_rev6_826.bin` | **1988–1991** | 32.0 KB | `8d2230dd7e79081e37e62735245d675a` | Factory Binary Firmware Dump |
| `p04_rev7_107.bin` | **1988–1991** | 32.0 KB | `5e7da87e4d5cdb1a403b4f6164925b0c` | Factory Binary Firmware Dump |
| `p04_rev8_128.bin` | **1988–1991** | 32.0 KB | `1ae65ab4ed174d07e388a7be826c8337` | Factory Binary Firmware Dump |
| `p04_rev9_140.bin` | **1988–1991** | 32.0 KB | `5b646891bb38b31a6a696f79d8bd24cc` | Factory Binary Firmware Dump |
| `p04_try_374.bin` | **1988–1991** | 32.0 KB | `df88aa07310de45fc0d7104aec57cf5b` | Factory Binary Firmware Dump |
| `pm5_dump_176.bin` | **1988–1991** | 32.0 KB | `cc08b15d100e94e5224982b11bf9a0d7` | Factory Binary Firmware Dump |
| `pm5_x30_1991508_175.bin` | **1988–1991** | 32.0 KB | `505a35a06c8aaa4a85bf9edee962f0c3` | Factory Binary Firmware Dump |
| `stock_p04-g01_131.bin` | **1988–1991** | 32.0 KB | `dedfb60aef63ab9e6cc8045403c6e5ea` | Factory Binary Firmware Dump |
| `stock_p04-g01_297.bin` | **1988–1991** | 32.0 KB | `dedfb60aef63ab9e6cc8045403c6e5ea` | Factory Binary Firmware Dump |
| `stock_p04-g02_sajmon1100_739.bin` | **1988–1991** | 32.0 KB | `df88aa07310de45fc0d7104aec57cf5b` | Factory Binary Firmware Dump |
| `stock_pm5_x30_120.bin` | **1988–1991** | 32.0 KB | `7719ed332d8b6783da4c3777cdd51b39` | Factory Binary Firmware Dump |

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
