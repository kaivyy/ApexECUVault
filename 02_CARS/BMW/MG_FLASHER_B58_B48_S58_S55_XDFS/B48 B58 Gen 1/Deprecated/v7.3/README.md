# v7.3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.3`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `52 files` (0 binary dumps, 52 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.3` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R0C9J8B2B_3081-080_017_002_v7.3.a2l` | **2015–2026** | 833.4 KB | `3b1301f4bfacbb443d0687fdf0c61f71` | ASAM ASAP2 ECU Description File |
| `R0C9J8B2B_3081-080_017_002_v7.3.xdf` | **2015–2026** | 2.69 MB | `b652936646c1b33e698549f3b255973c` | TunerPro Binary Definition Map |
| `R0C9J8D2B_3081-080_021_002_v7.3.a2l` | **2015–2026** | 833.4 KB | `c249054bae4c18797d6fef152f0826e5` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.3.xdf` | **2015–2026** | 2.69 MB | `b88a8031f5a09f339e92cf18df74ef8b` | TunerPro Binary Definition Map |
| `R0C9J8I2B_3081-080_029_002_v7.3.a2l` | **2015–2026** | 833.4 KB | `7f72834ce07e7d6fd3374472e9bc2c63` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.3.xdf` | **2015–2026** | 2.69 MB | `4b41c8a72aa70baa31f89355c0674677` | TunerPro Binary Definition Map |
| `R0C9J8I3B_3081-080_029_003_v7.3.a2l` | **2015–2026** | 833.4 KB | `864b9bd42b1d3c5e47f1654d91abe867` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.3.xdf` | **2015–2026** | 2.69 MB | `4b41c8a72aa70baa31f89355c0674677` | TunerPro Binary Definition Map |
| `R0C9J8I4B_3081-080_029_004_v7.3.a2l` | **2015–2026** | 833.4 KB | `b39d59daad6380e1cbb17beb96afe530` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.3.xdf` | **2015–2026** | 2.69 MB | `4b41c8a72aa70baa31f89355c0674677` | TunerPro Binary Definition Map |
| `R0C9J962B_3081-090_010_002_v7.3.a2l` | **2015–2026** | 833.4 KB | `62967d59ed8ed31ae148291cbffd1448` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.3.xdf` | **2015–2026** | 2.69 MB | `9d4783c4954d80e954fcee2d0242e351` | TunerPro Binary Definition Map |
| `R0C9J9E3B_3081-090_020_003_v7.3.a2l` | **2015–2026** | 833.4 KB | `acb5da999373a80864fb55c7e91349f7` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.3.xdf` | **2015–2026** | 2.69 MB | `6a4c27df0a62e08ba7f7c3b7268fc917` | TunerPro Binary Definition Map |
| `R0C9J9E4B_3081-090_020_004_v7.3.a2l` | **2015–2026** | 833.4 KB | `7d728128ee58a0c565548dfb342c48ad` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.3.xdf` | **2015–2026** | 2.69 MB | `e01d7c1e3939fdb74c4123a5b27baa65` | TunerPro Binary Definition Map |
| `R0C9JA05B_3081-090_025_005_v7.3.a2l` | **2015–2026** | 833.4 KB | `6cfe38eb0c2378d1124b5d5bdd2fbb36` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.3.xdf` | **2015–2026** | 2.69 MB | `c31fc833308e73213626964ebf6f1a50` | TunerPro Binary Definition Map |
| `R0C9JA15B_3081-090_030_005_v7.3.a2l` | **2015–2026** | 833.4 KB | `4f7cc030cffb0e319d8f560cda87f3ef` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.3.xdf` | **2015–2026** | 2.69 MB | `5420f0e327197d2f3606440fe8905b9b` | TunerPro Binary Definition Map |
| `R0C9JC05B_3081-090_050_005_v7.3.a2l` | **2015–2026** | 833.4 KB | `49111d0a921e789a8d2efc5028e5a428` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.3.xdf` | **2015–2026** | 2.69 MB | `00f421bab5f2b5647bf6e626dda28c9c` | TunerPro Binary Definition Map |
| `R0C9JD06B_3081-090_060_006_v7.3.a2l` | **2015–2026** | 833.4 KB | `32939d143f86a852246c9d045f697f15` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.3.xdf` | **2015–2026** | 2.69 MB | `0cc6400042e2ae51931628893fd737a2` | TunerPro Binary Definition Map |
| `R0C9JE15B_3081-090_080_005_v7.3.a2l` | **2015–2026** | 833.4 KB | `ecab99eb48ddad653b161ab94d9bb8c8` | ASAM ASAP2 ECU Description File |
| `R0C9JE15B_3081-090_080_005_v7.3.xdf` | **2015–2026** | 2.69 MB | `f1dea6257babe0e7d3cf4771a4b52849` | TunerPro Binary Definition Map |
| `R1C9I562B_3076-050_006_002_v7.3.a2l` | **2015–2026** | 798.3 KB | `56040f98305c1ec91e5c44f55181a144` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.3.xdf` | **2015–2026** | 2.60 MB | `9cd2a8dd28d48f00967194b28b3ea567` | TunerPro Binary Definition Map |
| `R1C9J8B2B_3076-080_017_002_v7.3.a2l` | **2015–2026** | 833.7 KB | `5eb6f183b304defb2bacc72b72690910` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.3.xdf` | **2015–2026** | 2.69 MB | `c5a6f118c80fafcaee02f1120f35a202` | TunerPro Binary Definition Map |
| `R1C9J8B3B_3076-080_017_003_v7.3.a2l` | **2015–2026** | 833.7 KB | `41ccc8540048bdfb9902609cc1e021bb` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.3.xdf` | **2015–2026** | 2.69 MB | `c5a6f118c80fafcaee02f1120f35a202` | TunerPro Binary Definition Map |
| `R1C9J8I2B_3076-080_029_002_v7.3.a2l` | **2015–2026** | 833.7 KB | `fe45cb83d1ba92c12af07c8dfd7ae7bf` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.3.xdf` | **2015–2026** | 2.69 MB | `6ec585707f6fc145aa535af4d4baef1f` | TunerPro Binary Definition Map |
| `R1C9J8I7B_3076-080_029_007_v7.3.a2l` | **2015–2026** | 833.7 KB | `98e209906f0db5a4ca8874d3c11fe536` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.3.xdf` | **2015–2026** | 2.69 MB | `6ec585707f6fc145aa535af4d4baef1f` | TunerPro Binary Definition Map |
| `R1C9J962B_3076-090_010_002_v7.3.a2l` | **2015–2026** | 833.7 KB | `a98c14065f862628bdb0334f7d710be5` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.3.xdf` | **2015–2026** | 2.69 MB | `fd67fa3ff5348db444e69f6ce9d526cc` | TunerPro Binary Definition Map |
| `R1C9J9E3B_3076-090_020_003_v7.3.a2l` | **2015–2026** | 833.7 KB | `989d2a87a47583e60881071518b46d0e` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.3.xdf` | **2015–2026** | 2.69 MB | `e1541e7b68cd97617e7c3c0f18a071ad` | TunerPro Binary Definition Map |
| `R1C9J9E5B_3076-090_020_005_v7.3.a2l` | **2015–2026** | 833.7 KB | `fc8a6e8e5f8af7ab6d9a9277485ef716` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.3.xdf` | **2015–2026** | 2.69 MB | `f1f580c55fa81154e51f0f6030d5337e` | TunerPro Binary Definition Map |
| `R1C9J9E7B_3076-090_020_007_v7.3.a2l` | **2015–2026** | 833.7 KB | `d404b4e2ee06436ea2a70f7df5a18af5` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.3.xdf` | **2015–2026** | 2.69 MB | `e1541e7b68cd97617e7c3c0f18a071ad` | TunerPro Binary Definition Map |
| `R1C9JA05B_3076-090_025_005_v7.3.a2l` | **2015–2026** | 833.7 KB | `26ea2a518ba99acdffaf56b029d19ade` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.3.xdf` | **2015–2026** | 2.69 MB | `61ef3b08e39e89de10c935460061a868` | TunerPro Binary Definition Map |
| `R1C9JC05B_3076-090_050_005_v7.3.a2l` | **2015–2026** | 833.7 KB | `0e136b69d65f8cedd6019de8ed9bd8cd` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.3.xdf` | **2015–2026** | 2.69 MB | `99a70c6a140ad2647f3438c612eba265` | TunerPro Binary Definition Map |
| `R1C9JD06B_3076-090_060_006_v7.3.a2l` | **2015–2026** | 833.7 KB | `fe11a0ec4a102e309ad854a73d4eedc0` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.3.xdf` | **2015–2026** | 2.69 MB | `79c59f0a37ae58fe7735fccca172d774` | TunerPro Binary Definition Map |
| `R1C9JE15B_3076-090_080_005_v7.3.a2l` | **2015–2026** | 833.7 KB | `2a407af03fa89f4ca10997e712ff1508` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.3.xdf` | **2015–2026** | 2.69 MB | `4fa6c026e919e870796e2f4bf1890774` | TunerPro Binary Definition Map |

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
