# SPORT_CB150R_CBR150R - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/SPORT_CB150R_CBR150R`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `33 files` (7 binary dumps, 26 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SPORT_CB150R_CBR150R` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `38770-KPP-602.bin` | **2000–2024** | 56.0 KB | `1353ef8c9d307d5d505ce52cdc96f419` | Factory Binary Firmware Dump |
| `38770-KPP-N02.bin` | **2000–2024** | 56.0 KB | `4e0df92ab66f570fdfb94835d6c81494` | Factory Binary Firmware Dump |
| `38770-KPP-T03.bin` | **2000–2024** | 56.0 KB | `14abcbc6aafdd507d209d7e9975271e6` | Factory Binary Firmware Dump |
| `GENERATIONAL_38770-K15-P01_Honda_All_New_CB150R_Streetfire_Gen_4_Inverted_Fork_(2021-2026).xdf` | **2021–2026** | 5.5 KB | `9cc91454a83c8cb85ac17c3431344396` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K3B-N01_Honda_CB150X_Adventure_Touring_(2021-2026).xdf` | **2021–2026** | 5.4 KB | `6b5cc821384cceec5a1b73726754e934` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K45-G01_Honda_CBR150R_Gen_3_Facelift_LED_(2016-2018).xdf` | **2016–2018** | 5.4 KB | `50fde4c4b6bb0c6278673f0d9f32a470` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K45-N01_Honda_CBR150R_Gen_2_Lokal_Dual_Eyes_(2014-2016).xdf` | **2014–2016** | 5.4 KB | `25cc735f56a713c36504c466b5994e92` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K45-N41_Honda_CBR150R_Gen_4_Facelift_ABS_&_Emergency_Stop_(2018-2020).xdf` | **2018–2020** | 5.4 KB | `602d57a4e0de479a3a1645f905ea1004` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K45-R01_Honda_All_New_CBR150R_Gen_5_Inverted_Fork_SFF-BP_(2021-2026).xdf` | **2021–2026** | 5.5 KB | `f75ed8eaf88fc0dd9f881d6ddf7c7c8f` | TunerPro Binary Definition Map |
| `HONDA_38770-K0A-A01_CB300R_Neo_Sports_Cafe_(2018-2024).xdf` | **2018–2024** | 16.3 KB | `2a2d4b2f293e4dab194f7f3367084a66` | TunerPro Binary Definition Map |
| `HONDA_38770-K0A-R11_CB300R_Neo_Sports_Cafe_(2018-2024).xdf` | **2018–2024** | 16.3 KB | `6f1597abed06ef229c9dd4a9a6186642` | TunerPro Binary Definition Map |
| `HONDA_38770-K15-601_CB150R_Streetfire.xdf` | **2000–2024** | 16.3 KB | `5e3b66afbe4e417c95ad5717f39356f7` | TunerPro Binary Definition Map |
| `HONDA_38770-K15-888_CB150R_Streetfire.xdf` | **2000–2024** | 16.3 KB | `509b5123d9906428df8113d6572b9771` | TunerPro Binary Definition Map |
| `HONDA_38770-K15-903_CB150R_Streetfire.xdf` | **2000–2024** | 16.3 KB | `fed0c9f19bcbe7bbb4f6d76340c10cbd` | TunerPro Binary Definition Map |
| `HONDA_38770-K15-921_CB150R_Streetfire.xdf` | **2000–2024** | 16.3 KB | `814a3df3c2b4a0f0ac883d487ab3b2a2` | TunerPro Binary Definition Map |
| `HONDA_38770-K18-902_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `e8632dc2ea4d3701db9231c74dbdde22` | TunerPro Binary Definition Map |
| `HONDA_38770-K18-941_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `3772842e83c0c2c2f2cee8aef4b07153` | TunerPro Binary Definition Map |
| `HONDA_38770-K18-961_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `052a1677480deefd3ea9e15dca389ff3` | TunerPro Binary Definition Map |
| `HONDA_38770-K33-D02_CBR300R___CB300F_(2014-2020).xdf` | **2014–2020** | 16.3 KB | `897f4d02e267bc5fac9cc7b171f4e355` | TunerPro Binary Definition Map |
| `HONDA_38770-K33-D22_CBR300R___CB300F_(2014-2020).xdf` | **2014–2020** | 16.3 KB | `016d443b003cc7c88012911cf73a22ae` | TunerPro Binary Definition Map |
| `HONDA_38770-K33-N03_CBR300R___CB300F_(2014-2020).xdf` | **2014–2020** | 16.3 KB | `1703b6cdec10ec7b9c3648c7b38544c6` | TunerPro Binary Definition Map |
| `HONDA_38770-K45-N01_CBR150R_LED_(2016-2024).xdf` | **2016–2024** | 16.3 KB | `9ed671b5880e7986eafa7b43a362597a` | TunerPro Binary Definition Map |
| `HONDA_38770-K45-N42_CBR150R_LED_(2016-2024).xdf` | **2016–2024** | 16.3 KB | `3a4bedfd57755f004f007204cb75f6d9` | TunerPro Binary Definition Map |
| `HONDA_38770-K45-NA1_CBR150R_LED_(2016-2024).xdf` | **2016–2024** | 16.3 KB | `9cf3fea2120ddeba02867a00662f84d3` | TunerPro Binary Definition Map |
| `HONDA_38770-K94-T02_CBR150R_(Indonesia).xdf` | **2000–2024** | 16.3 KB | `7d16656dc9628f178786f8fe6085d3ae` | TunerPro Binary Definition Map |
| `HONDA_38770-K98-E02_CB150R_Neo_Sports_Cafe_(2017-2024).xdf` | **2017–2024** | 16.3 KB | `4bb29b0f645b8a5267933f8660afc0bc` | TunerPro Binary Definition Map |
| `HONDA_38770-KPP-602_CBR150R_(2011-2015).xdf` | **2011–2015** | 16.3 KB | `846ef5a6b4b560d07c9e83cc7f441c76` | TunerPro Binary Definition Map |
| `HONDA_38770-KPP-N02_CBR150R_(2011-2015).xdf` | **2011–2015** | 16.3 KB | `b28c7ea8a312b9f00e57e7a768136b8a` | TunerPro Binary Definition Map |
| `HONDA_38770-KPP-T03_CBR150R_(2011-2015).xdf` | **2011–2015** | 16.3 KB | `178678b420baeab3a6f181084afd4719` | TunerPro Binary Definition Map |
| `HONDA_CB150R_EXMOTION_K94_T02_96KB_ORI.bin` | **2000–2024** | 96.0 KB | `818b5d1758d0f82d086a7f1f75e7b506` | Factory Binary Firmware Dump |
| `HONDA_CBR150R_FACELIFT_2019_64KB_ORI.bin` | **2019** | 64.0 KB | `389ae529c6d277677aece7fe4aeb2fae` | Factory Binary Firmware Dump |
| `HONDA_CBR150R_K45_TA1_64KB_ORI.bin` | **2000–2024** | 64.0 KB | `ec461f79908d3b2e30861463109fa3ec` | Factory Binary Firmware Dump |
| `HONDA_CBR150R_KPP_T03_56KB_ORI.bin` | **2000–2024** | 56.0 KB | `14abcbc6aafdd507d209d7e9975271e6` | Factory Binary Firmware Dump |

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
