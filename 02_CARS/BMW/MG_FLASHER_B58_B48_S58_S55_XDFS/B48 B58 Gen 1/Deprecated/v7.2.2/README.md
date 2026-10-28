# v7.2.2 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.2.2`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `50 files` (0 binary dumps, 50 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.2.2` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2015–2026

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `R0C9J8B2B_3081-080_017_002_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `cad48d9a56db9172cde594aaf8dc8176` | ASAM ASAP2 ECU Description File |
| `R0C9J8B2B_3081-080_017_002_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `f3deae565b9576b5064d4a129329b7b8` | TunerPro Binary Definition Map |
| `R0C9J8D2B_3081-080_021_002_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `a33fa615a1386c2c93d9a62a64fdf1f5` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `09ab9c18eb4a13866338b1d2c978389d` | TunerPro Binary Definition Map |
| `R0C9J8I2B_3081-080_029_002_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `49f6cd8488225816c3075e5f552085cf` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `16c3e33ed27f06735bb499a09c8e49b1` | TunerPro Binary Definition Map |
| `R0C9J8I3B_3081-080_029_003_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `cfc1ba718aa58aaa6b2ca189bfdf3340` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `16c3e33ed27f06735bb499a09c8e49b1` | TunerPro Binary Definition Map |
| `R0C9J8I4B_3081-080_029_004_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `6ef46e5cde729e0c37df972f27ff052e` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `16c3e33ed27f06735bb499a09c8e49b1` | TunerPro Binary Definition Map |
| `R0C9J962B_3081-090_010_002_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `044e38a286ae353e75147e6ba79617b2` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `19299d43fd31f9fc953da676b03c16f6` | TunerPro Binary Definition Map |
| `R0C9J9E3B_3081-090_020_003_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `e288bc179800f388524d47e606feaddd` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `77416f99acb9e8c35c7620e50774547f` | TunerPro Binary Definition Map |
| `R0C9J9E4B_3081-090_020_004_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `eb7c3a22b438420dfaedb64c56a467c7` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `c6f369d07a4af1b0d3da8771ecd0da99` | TunerPro Binary Definition Map |
| `R0C9JA05B_3081-090_025_005_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `586a6c07bcf594fb93c2db3086b38786` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `ef2c1327eded88f38837d376bc472911` | TunerPro Binary Definition Map |
| `R0C9JA15B_3081-090_030_005_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `38684ec56e45c1bda8bb24849e67b460` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `481fbed7ba47c710b971270c4f0cc96b` | TunerPro Binary Definition Map |
| `R0C9JC05B_3081-090_050_005_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `97b8a4f5a292cde01efb5d5e41e0099e` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `af1fff8e3e799b349555147a67c5f145` | TunerPro Binary Definition Map |
| `R0C9JD06B_3081-090_060_006_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `e29b3a2549fb6e74a2dd05c4e6a080f0` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `81f968add5cf42038b5a002a73c1046e` | TunerPro Binary Definition Map |
| `R1C9I562B_3076-050_006_002_v7.2.2.a2l` | **2015–2026** | 457.9 KB | `6930955345575fa90ae61dae39222b40` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.2.2.xdf` | **2015–2026** | 1.24 MB | `745898a95bd90571025fa72624125642` | TunerPro Binary Definition Map |
| `R1C9J8B2B_3076-080_017_002_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `b85af2c1e1d226ed3af2a69d427d0a21` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `be3897b0d64ec97d1586eed89e486050` | TunerPro Binary Definition Map |
| `R1C9J8B3B_3076-080_017_003_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `76f77d2c5db6e188b5fabf308041455d` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `be3897b0d64ec97d1586eed89e486050` | TunerPro Binary Definition Map |
| `R1C9J8I2B_3076-080_029_002_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `2bc635923087fbfc8eb338b6eeef2f58` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `8a82572fbf99e2ebeeeec7e0efd8b29b` | TunerPro Binary Definition Map |
| `R1C9J8I7B_3076-080_029_007_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `a152f713f44455da7231fe4c9e09b401` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `5f20a1a4647877018c110ba9fa18f7e9` | TunerPro Binary Definition Map |
| `R1C9J962B_3076-090_010_002_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `c1175d73ddbda3081090037d7a0bf44c` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `c27d4633deb5a9f452eef164a39abfca` | TunerPro Binary Definition Map |
| `R1C9J9E3B_3076-090_020_003_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `2a592bc6088e4ca826a902cba6a66ee5` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `9d7c04b00041eb0754632294345e1e13` | TunerPro Binary Definition Map |
| `R1C9J9E5B_3076-090_020_005_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `46bf3dbdb41e9f7426bc1bd8b40cd69f` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `40f625b2af8dbf308462e2b043f43a28` | TunerPro Binary Definition Map |
| `R1C9J9E7B_3076-090_020_007_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `9b09f4104dccd94b5186ef3b3860145c` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `57ce95fae2e7fd40a3ad82c89462ef20` | TunerPro Binary Definition Map |
| `R1C9JA05B_3076-090_025_005_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `3930e4c69ca2bcbba3c0793b501ab863` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `044a668a5b08905eaecf722bcdca0cca` | TunerPro Binary Definition Map |
| `R1C9JC05B_3076-090_050_005_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `50217bc19194e750f3b406a8258f2425` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `6325164477b6dcc43d94f3f34a876f26` | TunerPro Binary Definition Map |
| `R1C9JD06B_3076-090_060_006_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `69fa7aa88ef834c5ba64a8a0a50618b7` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `b62bd67f9c00b1622e04afb35a4bf61c` | TunerPro Binary Definition Map |
| `R1C9JE15B_3076-090_080_005_v7.2.2.a2l` | **2015–2026** | 483.5 KB | `121615ac1154a5a99f8b6196eaf2486b` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.2.2.xdf` | **2015–2026** | 1.30 MB | `a398abeec0af00d1bf0132cc61530176` | TunerPro Binary Definition Map |

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
