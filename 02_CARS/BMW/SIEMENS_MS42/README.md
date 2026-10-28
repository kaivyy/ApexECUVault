# SIEMENS_MS42 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/SIEMENS_MS42`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `18 files` (16 binary dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SIEMENS_MS42` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1998–2001

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `Siemens_MS42_0110C6_E36Z3_M52TUB20_EU3.bin` | **1998–2001** | 512.0 KB | `5d6edbe6adb2bde3a40e876cf9d258c6` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E36Z3_M52TUB28_EU3_LHD.bin` | **1998–2001** | 512.0 KB | `0760e87aae47ebe7ba91c29972b146b3` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E36Z3_M52TUB28_EU3_RHD.bin` | **1998–2001** | 512.0 KB | `774f3286c19c03207b60ba899a1ceb84` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E38_M52TUB28_EU3.bin` | **1998–2001** | 512.0 KB | `d2edb2dc21cd288292568f2f21cd5485` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E39_M52TUB20_EU3.bin` | **1998–2001** | 512.0 KB | `ac6f43c675fbaae7de5398d40bb11995` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E39_M52TUB25_EU3_LHD.bin` | **1998–2001** | 512.0 KB | `adeb3e302d74dc0a132353556503ebfd` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E39_M52TUB25_EU3_RHD.bin` | **1998–2001** | 512.0 KB | `f8b716f00ee3e3e2a9dc709be9950e44` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E39_M52TUB28_EU3_LHD.bin` | **1998–2001** | 512.0 KB | `8537eec13e4331891862f7b7e61e23a3` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E39_M52TUB28_EU3_RHD.bin` | **1998–2001** | 512.0 KB | `890aa03afcdf513ed036f9ea77b8d85f` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E46_M52TUB20_EU2_CATV.bin` | **1998–2001** | 512.0 KB | `b09a0bce3683a561dbe4a9f2b15c33ac` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E46_M52TUB20_EU3.bin` | **1998–2001** | 512.0 KB | `dfdda11fd4e7df35dcdd880d83ccca9b` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E46_M52TUB24_THAI_RHD.bin` | **1998–2001** | 512.0 KB | `cbc98fe5b1a21093c2aecb5ad3392733` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E46_M52TUB25_EU3_LHD.bin` | **1998–2001** | 512.0 KB | `cbc98fe5b1a21093c2aecb5ad3392733` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E46_M52TUB25_EU3_RHD.bin` | **1998–2001** | 512.0 KB | `bc0a5c6f959ad572c5dda6ac411d6f8e` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E46_M52TUB28_EU3_LHD.bin` | **1998–2001** | 512.0 KB | `63ea68c0ecead90958f2ef4957cfba20` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_E46_M52TUB28_EU3_RHD.bin` | **1998–2001** | 512.0 KB | `f90e47fccbe0f23e010872e013c57864` | Factory Binary Firmware Dump |
| `Siemens_MS42_0110C6_ENG_32K_v1.3.xdf` | **1998–2001** | 2.21 MB | `5416cb08995fe71e9d60574fed24b293` | TunerPro Binary Definition Map |
| `Siemens_MS42_0110C6_ENG_512K_v1.3.xdf` | **1998–2001** | 2.21 MB | `8db31fe8ccd828c43ec882553d5354b1` | TunerPro Binary Definition Map |

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
