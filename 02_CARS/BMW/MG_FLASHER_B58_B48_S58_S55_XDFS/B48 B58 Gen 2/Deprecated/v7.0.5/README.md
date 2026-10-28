# v7.0.5 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.0.5`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `38 files` (0 binary dumps, 38 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.0.5` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R4C9F4E6B_5d55-040_150_006_v7.0.5.a2l` | **2015–2026** | 172.3 KB | `6aafd796436f3943c3283fdabf388d8a` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.0.5.a2l` | **2015–2026** | 172.3 KB | `568f5fc18a84a2fb812fc97d5d5b8c66` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.0.5.a2l` | **2015–2026** | 172.3 KB | `6b34ad78d2bc59add387a105ecc8c5fb` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.0.5.a2l` | **2015–2026** | 172.3 KB | `7403c674c60fb501f2b7c71656e1a6e0` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.0.5.a2l` | **2015–2026** | 172.3 KB | `25963f806297e7588fc8ba8e6b28ec11` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `06547b16d8c8210a950b8dba02e0cfd5` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `1dda31cbff7606953dfb3a6765817ebd` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `50a6ca0ed1c3fdea663a54c504f097da` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `385e48d3baf7bd91a192bd77287c2bf2` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `6d27631d117425f663fee0f5163b9c46` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `8faa5f5d100e9d48e0efb50b00666635` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `97ad629c960106fa4028f6bdfaea4eb7` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `b68c9fd359a2e1ffa2de407430ae0e91` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `e287470a4997b1563d67da40ba072e2b` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `f1810cbd1d7b1f47bba8207eb90b324d` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `b172e61b6fa23c3b2ac1ffcdce89f297` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `0ac3c0fb650571c4901acb09bf0eac6e` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `9596ce0500a338f6b0f2d67ef99e2816` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `758f838a1150d3e555ca2d39e6681986` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `2385c030be8efc4101c476caff8dd7d5` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `81858f9008948d74a9c6b7f553db0f3f` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `39a2177a031f97bf7a4689e29024bcc6` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `f4fc5634ad274863bd9c90a32f902e4b` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `a25e22d959ccbe487463331f30aa2ae0` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `d63b28d8697d77b858cd5a09514b95d8` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `56a9d6cbcc78f2433128dbcb561eba71` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `d1cb2dfac128cad89d39e633f9cfbfa9` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `402cda587765471e5cd1dcaf13d8f9c5` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `049a4c63473effc851b56aaac82fb194` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `6e4a08500a43ca841b49e125ec0aafb5` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `9ac290261d6b1cb287d1c7d407309213` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `3fe6d6faff4fa1a11002d425ee400668` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `a26e958e8b957211ace4c9437fb37ad0` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `fe653b8ae122897a0be62fe5db0f9ee2` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `af0d26e6af7d8056de792c83ed9c9df4` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `490daee8110d181f790622e212699f76` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `0c4260a1271d489797b47184cb6d1187` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.0.5.a2l` | **2015–2026** | 174.1 KB | `afd45ed23db71df527268bad7104f4b7` | ASAM ASAP2 ECU Description File |

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
