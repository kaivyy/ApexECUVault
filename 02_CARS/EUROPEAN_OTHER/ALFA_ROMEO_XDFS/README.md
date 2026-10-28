# ALFA_ROMEO_XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/EUROPEAN_OTHER/ALFA_ROMEO_XDFS`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `29 files` (0 binary dumps, 29 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ALFA_ROMEO_XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `145_1.4_16V_TS_0261204481_1037358388.xdf` | **2000–2024** | 448.8 KB | `bbc0af7871347bdb53476d567742a3d2` | TunerPro Binary Definition Map |
| `145_1.6_16V_TS_0261200695_1267358244.xdf` | **2000–2024** | 392 B | `757a66f9271cb91c6edced3e21ce1a96` | TunerPro Binary Definition Map |
| `145_1.7_16V_0261203354_1267358146.xdf` | **2000–2024** | 121.4 KB | `279cec50f1dc34899a950b6f72bbba75` | TunerPro Binary Definition Map |
| `145_1.7_16V_0261203849_358699.xdf` | **2000–2024** | 124.9 KB | `64937700a4121429cbb86a9bf5b216f6` | TunerPro Binary Definition Map |
| `145_2.0_16V_TS_0261204478_1037358492.xdf` | **2000–2024** | 168.6 KB | `20d4f49c1f0c6683bd50e313f665a73a` | TunerPro Binary Definition Map |
| `155_1.7_TS_0261200536_1267357669.xdf` | **2000–2024** | 170.4 KB | `af90cac0bbe803ca60f798db17dc26d0` | TunerPro Binary Definition Map |
| `155_1.8_16V_TS_0261203846_1267358560.xdf` | **2000–2024** | 145.5 KB | `0e0227bd6f84277a229f57f16ca5b05d` | TunerPro Binary Definition Map |
| `155_1.8_16V_TS_0261204168_355197.xdf` | **2000–2024** | 168.4 KB | `0e480a32323bcb0b15ab4d8f63d7c97a` | TunerPro Binary Definition Map |
| `155_1.8_TS_0261200536_1267356588.xdf` | **2000–2024** | 183.1 KB | `9db5856cdb306c27451d0030913d304f` | TunerPro Binary Definition Map |
| `155_1.8_TS_0261200536_1267357151.xdf` | **2000–2024** | 183.1 KB | `e2b2c7cf05ab91b17232e94cb739f9d1` | TunerPro Binary Definition Map |
| `155_1.8_TS_0261200536_1267357963.xdf` | **2000–2024** | 174.5 KB | `ebc905b534c80f1a1b0489054125225e` | TunerPro Binary Definition Map |
| `155_2.0_16V_TS_0261203862_355410.xdf` | **2000–2024** | 155.7 KB | `93bd40ee019245dbac7bb08de86d0357` | TunerPro Binary Definition Map |
| `155_2.0_16V_TS_0261203993_355908.xdf` | **2000–2024** | 155.7 KB | `6526da4595f4ec7f1f34614496c1c5bd` | TunerPro Binary Definition Map |
| `155_2.0_TS_0261200536_1267357094.xdf` | **2000–2024** | 183.1 KB | `2d6cd52c0e22c55d6d6b23c7d26e9b87` | TunerPro Binary Definition Map |
| `155_2.0_TS_0261200536_1267357151.xdf` | **2000–2024** | 183.1 KB | `dc1885e446a54efe7e796ce2b933926b` | TunerPro Binary Definition Map |
| `155_2.0_TS_0261200536_1267357669.xdf` | **2000–2024** | 170.4 KB | `3396e5a49b91cd32618a4918a5d58a7c` | TunerPro Binary Definition Map |
| `155_2.5_V6_0261200537_1267356596.xdf` | **2000–2024** | 106.1 KB | `a2235857f035c1a4065846f19f9d9dc4` | TunerPro Binary Definition Map |
| `155_2.5_V6_0261203829_1267358578.xdf` | **2000–2024** | 128.2 KB | `8a2a93c5339d1dcf957dfbc4f297698d` | TunerPro Binary Definition Map |
| `164_2.0_TS_0261200108_1267355452.xdf` | **2000–2024** | 216.6 KB | `2ac631405b7c9999db0a8d441bb9ce0f` | TunerPro Binary Definition Map |
| `164_2.0_TS_0261200108_1267355604.xdf` | **2000–2024** | 216.6 KB | `19dc04a2df6e3ef95cf5833040104e96` | TunerPro Binary Definition Map |
| `164_2.0_TS_0261200108_1267356191.xdf` | **2000–2024** | 216.7 KB | `d6b287d29b5bb559663535cd9bff7d65` | TunerPro Binary Definition Map |
| `164_3.0_12V_0261200117_1267355710.xdf` | **2000–2024** | 213.3 KB | `732da5ebf5ea102ad21d3cd981ba2cff` | TunerPro Binary Definition Map |
| `164_3.0_12V_0261200117_1267356096.xdf` | **2000–2024** | 212.6 KB | `eb1c2fe0727c72e3d23cbb13bac412e2` | TunerPro Binary Definition Map |
| `164_3.0_12V_0261200117_1267356310.xdf` | **2000–2024** | 212.6 KB | `be748034a4b2709dcd62b71683ee00fe` | TunerPro Binary Definition Map |
| `75_3.0_12V_0261200141_1267356097.xdf` | **2000–2024** | 206.5 KB | `655480d8e22b6d5aaa9050ec5f96d63c` | TunerPro Binary Definition Map |
| `GTV_2.0_16V_TS_0261203671_355934.xdf` | **2000–2024** | 155.7 KB | `f2b74e95cac281a651612c381fe9c1c3` | TunerPro Binary Definition Map |
| `GTV_2.0_V6_TURBO_0261203869_1267358696.xdf` | **2000–2024** | 141.7 KB | `ff81be3844d1882101ff2c9797df703a` | TunerPro Binary Definition Map |
| `GTV_2.0_V6_TURBO_0261203883_1037358648.xdf` | **2000–2024** | 142.2 KB | `656044d4aef8c8be550dad1fbeb7feef` | TunerPro Binary Definition Map |
| `SZ_3.0_12V_0261200141_1267355737.xdf` | **2000–2024** | 206.7 KB | `f9311be0af16c7c3a5e87e15014461d6` | TunerPro Binary Definition Map |

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
