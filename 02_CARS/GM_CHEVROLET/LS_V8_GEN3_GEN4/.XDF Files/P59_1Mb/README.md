# P59_1Mb - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/LS_V8_GEN3_GEN4/.XDF Files/P59_1Mb`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `10 files` (8 binary dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `P59_1Mb` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `'04 Chevy MPV  4x4 Half Ton LM7 os12587603.bin` | **2004** | 1.00 MB | `07cfa958303ce233016c29c5d9983dcb` | Factory Binary Firmware Dump |
| `'04 GMC 1T 4x4 8.1 L18 os12587603.bin` | **2004** | 1.00 MB | `52d7d7c7d6de397b5e7d86f83d4658d0` | Factory Binary Firmware Dump |
| `03_Sierra_LM7_4L60E_DBW_OS12587603.bin` | **2003** | 1.00 MB | `412a4d7cfb38fe24fc00f5a09dd40d83` | Factory Binary Firmware Dump |
| `2004 2500 LQ4 Auto 2wd stock OS12587603.bin` | **2004** | 1.00 MB | `59698a2f43fc1bd1c080ef9e65bbc7bc` | Factory Binary Firmware Dump |
| `2004 Escalade 5.3AutoStock OS12587603.bin` | **2004** | 1.00 MB | `a01110a0bd863433c5129748d54b613f` | Factory Binary Firmware Dump |
| `C1500_5.3L_OS12587603.bin` | **2000–2024** | 1.00 MB | `d093d51c6966f57825d77d158f8b9e4c` | Factory Binary Firmware Dump |
| `Chevy_1500_4x2_LM7 _OS12587603.bin` | **2000–2024** | 1.00 MB | `a88e7062f3019e59b12314f56ed985d0` | Factory Binary Firmware Dump |
| `Chevy_1500_4x4_MPV_L59_12587603.bin` | **2000–2024** | 1.00 MB | `1428a0038c2a3385befca2350796017c` | Factory Binary Firmware Dump |
| `No Password - Operating System 12587603 - 1Mb PCM - 2004 model year.xdf` | **2004** | 616.9 KB | `5be466e0bbbe39b09d50b6ec9db8d4fc` | TunerPro Binary Definition Map |
| `Operating System 12587603 - 1Mb PCM - 2004 model year.xdf` | **2004** | 617.2 KB | `d2d3d2bfc08a93161fd0d4fa5ed0fb6d` | TunerPro Binary Definition Map |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi yang tersedia, struktur kalibrasi mencakup parameter esensial:
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
