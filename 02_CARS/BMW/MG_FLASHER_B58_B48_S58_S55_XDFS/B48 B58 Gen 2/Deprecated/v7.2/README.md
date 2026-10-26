# v7.2 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.2`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `40 files` (0 binary dumps, 40 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.2` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `R4C9F4E6B_5d55-040_150_006_v7.2.xdf` | **2015–2026** | 1.24 MB | `23522041eecc3f977c111034fb4393de` | TunerPro Binary Definition Map |
| `R4C9F4K6B_5d55-040_170_006_v7.2.xdf` | **2015–2026** | 1.24 MB | `3918fef4ceb8ccbb01b5a268b41af6f0` | TunerPro Binary Definition Map |
| `R4C9F4N5B_5d55-040_180_005_v7.2.xdf` | **2015–2026** | 1.24 MB | `2910fceb0315a3c3392d982c732ee519` | TunerPro Binary Definition Map |
| `R4C9F4P7B_5d55-040_190_007_v7.2.xdf` | **2015–2026** | 1.24 MB | `2910fceb0315a3c3392d982c732ee519` | TunerPro Binary Definition Map |
| `R4C9F4P9B_5d55-040_190_009_v7.2.xdf` | **2015–2026** | 1.24 MB | `2910fceb0315a3c3392d982c732ee519` | TunerPro Binary Definition Map |
| `R4C9H5C5B_5d55-050_140_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `0a9c76b6894252e728d8a4138316ef4b` | TunerPro Binary Definition Map |
| `R4C9H5I5B_5d55-050_160_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `42d34c472b18ebc56b6f7cdfda8f3782` | TunerPro Binary Definition Map |
| `R4C9H5K5B_5d55-050_170_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `ca843077eb6f18b83acfc08482185833` | TunerPro Binary Definition Map |
| `R4C9H5N6B_5d55-050_180_006_v7.2.xdf` | **2015–2026** | 1.25 MB | `3f9794b6faabcec6f93f674e3e1b6f87` | TunerPro Binary Definition Map |
| `R4C9H5P7B_5d55-050_190_007_v7.2.xdf` | **2015–2026** | 1.25 MB | `93eac7d2051be58bade529cf9d18f908` | TunerPro Binary Definition Map |
| `R4C9H5P9B_5d55-050_190_009_v7.2.xdf` | **2015–2026** | 1.25 MB | `93eac7d2051be58bade529cf9d18f908` | TunerPro Binary Definition Map |
| `R4C9H5S8B_5d55-050_200_008_v7.2.xdf` | **2015–2026** | 1.25 MB | `fb02036d551fd2400ed59c5c27212a3e` | TunerPro Binary Definition Map |
| `R4C9H5V5B_5d55-050_220_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `7ef96d655da5014e1d2d67f8248b6e20` | TunerPro Binary Definition Map |
| `R4C9H695B_5d55-060_100_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `99e6bcd767b52768ebdb0e9062fccc93` | TunerPro Binary Definition Map |
| `R4C9H6B5B_5d55-060_110_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `9bcdbc11a167f5d2f746cc30408670b5` | TunerPro Binary Definition Map |
| `R4C9H6D7B_5d55-060_120_007_v7.2.xdf` | **2015–2026** | 1.25 MB | `381c9d594e7b9800a578741c7f48277b` | TunerPro Binary Definition Map |
| `R4C9H6H7B_5d55-060_130_007_v7.2.xdf` | **2015–2026** | 1.25 MB | `0ef7e98863581f830feab061cbdf7a75` | TunerPro Binary Definition Map |
| `R4C9H6K5B_5d55-060_140_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `a4e2cf16b5d53cf6584ab29164ac3cf9` | TunerPro Binary Definition Map |
| `R4C9H6N7B_5d55-060_150_007_v7.2.xdf` | **2015–2026** | 1.25 MB | `abe50ce42c65121dc67e3cbc409a6d88` | TunerPro Binary Definition Map |
| `R4C9H6P7B_5d55-060_160_007_v7.2.xdf` | **2015–2026** | 1.25 MB | `70e7359ec85df5badb84fcd4ca7421c5` | TunerPro Binary Definition Map |
| `R4C9H6P9B_5d55-060_160_009_v7.2.xdf` | **2015–2026** | 1.25 MB | `70e7359ec85df5badb84fcd4ca7421c5` | TunerPro Binary Definition Map |
| `R4C9H6S8B_5d55-060_170_008_v7.2.xdf` | **2015–2026** | 1.25 MB | `e89b9ae4f6337280cf44a719f8ef6e00` | TunerPro Binary Definition Map |
| `R4C9H6V5B_5d55-060_190_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `d700cb4dfca7e2d051287f40755768a7` | TunerPro Binary Definition Map |
| `R4C9J718B_5d55-070_030_008_v7.2.xdf` | **2015–2026** | 1.25 MB | `3917d43ad13d45b5b0956b938f258ac9` | TunerPro Binary Definition Map |
| `R4C9J755B_5d55-070_040_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `5e45093a9db105d249b6742997d31e97` | TunerPro Binary Definition Map |
| `R4C9J756B_5d55-070_040_006_v7.2.xdf` | **2015–2026** | 1.25 MB | `abe99dabf1e645f12209e25a631e7411` | TunerPro Binary Definition Map |
| `R4C9J758B_5d55-070_050_008_v7.2.xdf` | **2015–2026** | 1.25 MB | `4d575108c162f9c7d854ee88eda0fad8` | TunerPro Binary Definition Map |
| `R4C9J797B_5d55-070_060_007_v7.2.xdf` | **2015–2026** | 1.25 MB | `8f867bcf5b60e1ea5cd150fd83fb86c9` | TunerPro Binary Definition Map |
| `R4C9J7A5B_5d55-070_070_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `8f867bcf5b60e1ea5cd150fd83fb86c9` | TunerPro Binary Definition Map |
| `R4C9J7N5B_5d55-070_080_005_v7.2.xdf` | **2015–2026** | 1.25 MB | `e2bc1924b06f333cc9492442de3c1b93` | TunerPro Binary Definition Map |
| `R4C9J7P7B_5d55-070_090_007_v7.2.xdf` | **2015–2026** | 1.25 MB | `3412b592100a0c7351365f4d59802bfa` | TunerPro Binary Definition Map |
| `R4C9J7P9B_5d55-070_090_009_v7.2.xdf` | **2015–2026** | 1.25 MB | `3412b592100a0c7351365f4d59802bfa` | TunerPro Binary Definition Map |
| `R4C9J7S8B_5d55-070_100_008_v7.2.xdf` | **2015–2026** | 1.25 MB | `31a119f79930045fc0ea1fdd3ee03302` | TunerPro Binary Definition Map |
| `R4C9L857B_5d55-080_040_007_v7.2.xdf` | **2015–2026** | 1.24 MB | `8bdd99363b4cc75c87eb9c35b4c96810` | TunerPro Binary Definition Map |
| `R4C9L875B_5d55-080_055_005_v7.2.xdf` | **2015–2026** | 1.24 MB | `6a4f3ef1ae6b53448305c20e931dc73b` | TunerPro Binary Definition Map |
| `R4C9L8N5B_5d55-080_060_005_v7.2.xdf` | **2015–2026** | 1.24 MB | `f338bfac6560ff6faf931b425acdc90e` | TunerPro Binary Definition Map |
| `R4C9L8P7B_5d55-080_072_007_v7.2.xdf` | **2015–2026** | 1.24 MB | `75b38351190a2dcf0a45b383bdea557f` | TunerPro Binary Definition Map |
| `R4C9L8P9B_5d55-080_072_009_v7.2.xdf` | **2015–2026** | 1.24 MB | `75b38351190a2dcf0a45b383bdea557f` | TunerPro Binary Definition Map |
| `R4C9L8PCB_5d55-080_072_012_v7.2.xdf` | **2015–2026** | 1.24 MB | `70e5d036c5da99a096f3e6c22b02ee3d` | TunerPro Binary Definition Map |
| `R4C9L8S8B_5d55-080_080_008_v7.2.xdf` | **2015–2026** | 1.24 MB | `fcb5a512c444a18344b49705cc27dde7` | TunerPro Binary Definition Map |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro yang tersedia, struktur kalibrasi mencakup parameter esensial:
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
