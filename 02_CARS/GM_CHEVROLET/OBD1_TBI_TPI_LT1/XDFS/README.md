# XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/OBD1_TBI_TPI_LT1/XDFS`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `51 files` (0 binary dumps, 51 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `0D_tpv4_v200.xdf` | **2000–2024** | 971.3 KB | `804eda07f5e5ecec31493831ec3420b8` | TunerPro Binary Definition Map |
| `0D_tpv5_v250.xdf` | **2000–2024** | 1.30 MB | `e3c7d5656b2f404905a876c3c3ea449f` | TunerPro Binary Definition Map |
| `0E_tpv4_v200.xdf` | **2000–2024** | 848.5 KB | `c601dbfa54b0403e8b80c58dfc0cae2e` | TunerPro Binary Definition Map |
| `0E_tpv5_v250.xdf` | **2000–2024** | 1.13 MB | `899905e81e466e66731812fefd07214d` | TunerPro Binary Definition Map |
| `1C.xdf` | **2000–2024** | 32.9 KB | `627bae712930efe5ca19c7f857c85671` | TunerPro Binary Definition Map |
| `1D.xdf` | **2000–2024** | 68.0 KB | `ca870afc97970c7a0203d93f89eb3547` | TunerPro Binary Definition Map |
| `1F.xdf` | **2000–2024** | 59.2 KB | `0069aaf3cc463ab6e37eaea8d27125fe` | TunerPro Binary Definition Map |
| `1FA.xdf` | **2000–2024** | 95.6 KB | `3e53851494f389f1ac1633ed82f5141f` | TunerPro Binary Definition Map |
| `24.xdf` | **2000–2024** | 59.5 KB | `b166db15f8726637628ce211affd1af6` | TunerPro Binary Definition Map |
| `24A.xdf` | **2000–2024** | 64.9 KB | `2a8f240d752fa7c1f4a4891007b4666a` | TunerPro Binary Definition Map |
| `2E.xdf` | **2000–2024** | 144.8 KB | `e77d190879f66c492254292284344ace` | TunerPro Binary Definition Map |
| `2E_tpv5.xdf` | **2000–2024** | 390.1 KB | `28f8629c5907fc434d33e4d8d3bda985` | TunerPro Binary Definition Map |
| `31.xdf` | **2000–2024** | 69.1 KB | `9a9ca3918c0a4fb5b73784b891cfcddf` | TunerPro Binary Definition Map |
| `31_tpv5_v250.xdf` | **2000–2024** | 1.13 MB | `c658a57430e07e2eed3a39f683868876` | TunerPro Binary Definition Map |
| `32.xdf` | **2000–2024** | 63.1 KB | `c367341613ab2cd124f70cd365e4d3d8` | TunerPro Binary Definition Map |
| `32B.xdf` | **2000–2024** | 53.2 KB | `e7dc5fba030a851b626f737fa8eda777` | TunerPro Binary Definition Map |
| `3A.xdf` | **2000–2024** | 59.8 KB | `3a49b59e41d3eeb3fd7d1e5c8c6a2b72` | TunerPro Binary Definition Map |
| `42.xdf` | **2000–2024** | 103.4 KB | `0cde3cffeb54da5499c86f1cb67bb20d` | TunerPro Binary Definition Map |
| `4E.xdf` | **2000–2024** | 85.2 KB | `24dcbfacda3270de8c537a2f433e8981` | TunerPro Binary Definition Map |
| `58ASunbird.xdf` | **2000–2024** | 77.5 KB | `d94a5608a16ab1e476f5302b1652dd36` | TunerPro Binary Definition Map |
| `58SyTy.xdf` | **2000–2024** | 300.3 KB | `78c77de74fc8fbf0af326da3bfea8a6a` | TunerPro Binary Definition Map |
| `5B4.xdf` | **2000–2024** | 76.2 KB | `62a8356abae1f4d87565e542970ef94e` | TunerPro Binary Definition Map |
| `5B5.xdf` | **2000–2024** | 66.8 KB | `291a29247f2fba379d9d20bec30eb763` | TunerPro Binary Definition Map |
| `5B6.xdf` | **2000–2024** | 108.1 KB | `c78f172646cca3be2fe590a1f679156a` | TunerPro Binary Definition Map |
| `5B_TPV5.xdf` | **2000–2024** | 244.4 KB | `3e61a7493204932b887cc717f4470730` | TunerPro Binary Definition Map |
| `61v3.xdf` | **2000–2024** | 118.7 KB | `e0e4cb7c8f9259456bdad3e1a5fe8c44` | TunerPro Binary Definition Map |
| `62.xdf` | **2000–2024** | 58.5 KB | `a68927cb920bd32f232d94d4810ee6c8` | TunerPro Binary Definition Map |
| `6D.xdf` | **2000–2024** | 89.8 KB | `d799cc785b61bb714c91c8fc19bfc117` | TunerPro Binary Definition Map |
| `6E.xdf` | **2000–2024** | 101.1 KB | `12e7942dd255e652b8aab097785190e0` | TunerPro Binary Definition Map |
| `83A.xdf` | **2000–2024** | 40.5 KB | `ebc949f39a3d71440c01b85e9a0726e2` | TunerPro Binary Definition Map |
| `85.xdf` | **2000–2024** | 75.4 KB | `4be0c3006b1fad1a7ceb6c20609a45e2` | TunerPro Binary Definition Map |
| `88.xdf` | **2000–2024** | 85.3 KB | `5f86a48c7c2a618c6ba8182b24ad73f4` | TunerPro Binary Definition Map |
| `8B.xdf` | **2000–2024** | 101.4 KB | `d1c22df86f24321235a01ce08bbcd6dd` | TunerPro Binary Definition Map |
| `8E.xdf` | **2000–2024** | 51.6 KB | `cf4bdedf9b983f426d8c41e4d8fb9b83` | TunerPro Binary Definition Map |
| `8F.xdf` | **2000–2024** | 576.9 KB | `4a11ad5b4e9463fd4608c215f4ffd2bc` | TunerPro Binary Definition Map |
| `8F_v2.xdf` | **2000–2024** | 424.6 KB | `3a75ff0ff0291cddcc0daae811fab275` | TunerPro Binary Definition Map |
| `94.xdf` | **2000–2024** | 51.0 KB | `d4a176576f23691a1ffa7fae0e162277` | TunerPro Binary Definition Map |
| `99.xdf` | **2000–2024** | 48.9 KB | `bc781c3f1bc1e46117d19c988d72facd` | TunerPro Binary Definition Map |
| `A1.xdf` | **2000–2024** | 238.3 KB | `94ac187c3e1c3b06931ce6ac85ad32d6` | TunerPro Binary Definition Map |
| `A1_tpv4.xdf` | **2000–2024** | 170.1 KB | `86d7783267afd43e31e79820889dec6f` | TunerPro Binary Definition Map |
| `A1_tpv5.xdf` | **2000–2024** | 704.9 KB | `a2a680bc3594f2497833f1476835c03f` | TunerPro Binary Definition Map |
| `DA2.xdf` | **2000–2024** | 40.1 KB | `dd8399829d365e4357db3d0064e3f830` | TunerPro Binary Definition Map |
| `DA3.xdf` | **2000–2024** | 139.3 KB | `bd74ed20a97cd1583c548aec8e7c2299` | TunerPro Binary Definition Map |
| `DF.xdf` | **2000–2024** | 87.2 KB | `12a23c3b7dbea0b6ee3146619416a2a0` | TunerPro Binary Definition Map |
| `E6_tpv4_v200.xdf` | **2000–2024** | 968.1 KB | `b1d2565222f3b5f787045ba41f08b964` | TunerPro Binary Definition Map |
| `E6_tpv5_v250.xdf` | **2000–2024** | 1.29 MB | `b18a10aa3ad774e57c56b1d089c565e5` | TunerPro Binary Definition Map |
| `E8.xdf` | **2000–2024** | 99.6 KB | `3886afdb9b966b16b220bc65b924c878` | TunerPro Binary Definition Map |
| `EE.xdf` | **2000–2024** | 138.5 KB | `99b0ceb1ab9243f3eeb7b0b50b3314cb` | TunerPro Binary Definition Map |
| `F0.xdf` | **2000–2024** | 61.9 KB | `5b24dfbe888ce0ce2940c1e8a80c7157` | TunerPro Binary Definition Map |
| `Super_8dm2.ecu` | **2000–2024** | 133.3 KB | `1fcb0c4ccc55169d16ba4c942ed3597f` | ECU / XML Calibration Map Definition |
| `T31.xdf` | **2000–2024** | 131.0 KB | `5ebd78628d4548875378686746d8c2c2` | TunerPro Binary Definition Map |

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
