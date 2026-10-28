# v7.2.3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.2.3`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `42 files` (0 binary dumps, 42 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.2.3` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R4C9F4E6B_5d55-040_150_006_v7.2.3.a2l` | **2015–2026** | 484.6 KB | `41af14d057e9627a089aa4133c4cd36a` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.2.3.a2l` | **2015–2026** | 484.6 KB | `f75344cc09c2e3a2ea8903ac691add94` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.2.3.a2l` | **2015–2026** | 484.6 KB | `af5a363d7c1803fb8ec97bb96bae5ad6` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.2.3.a2l` | **2015–2026** | 484.6 KB | `69f8d7a7f8430fe38fd2ed15c5051b47` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.2.3.a2l` | **2015–2026** | 484.6 KB | `c7b967c0469b2798fb92d4115a3f40ee` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `68b880432cdf271c640e5eb043cb11fb` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `0afe9947e5fa803e2aba9cd7b2a2615c` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `e403027cd2cea3f4cf99402e9e8ec86b` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `e014e04c05b3d1847256816f7766c36b` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `1ac11beb0625984110437ec5ec97c3dc` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `3b839ae2c22c7b5338d60dbee9130d04` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `852b85a569c3f9e72d361b9e925afa32` | ASAM ASAP2 ECU Description File |
| `R4C9H5V5B_5d55-050_220_005_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `56484bc8929d13b791ab5240924b3030` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `4ad596facad633afa863c5ff79b8eb31` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `a702b5c8f8b3ffac7dbdbffecbe379e4` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `15dafba00c1658ebb4501a694554fd15` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `b175bb6a9a760fc67401949ab2e79f21` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `34533ad7b389e1082d407995ecfbaf3b` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `2250a1d12832d3fb66bd5fa44010e94a` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `811569db0d37e321c3095c3b15aa21eb` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `6021ed1f1d3c88f4e3e69230d0df1b1c` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `f5689ca23eca92fc5da28aab2e593e54` | ASAM ASAP2 ECU Description File |
| `R4C9H6V5B_5d55-060_190_005_v7.2.3.a2l` | **2015–2026** | 487.2 KB | `d1ae77843d7d8723c2f8b92e73346f4f` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `a145fd3d6edb023088444046e58d75d3` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `e62b3a5647ee2dc057a577a7a2e990fc` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `3524b64e26ffe73deb45ff8c890a76ef` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `69357141633a94d5cd6a0479badc6e97` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `abdf4ed490b5d894aaa1043542077c04` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `2ab4c4616a9d79d8e5c0f7eb409fecb0` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `1290429a3b9b4d49045e40ebe8c819f8` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `3a13b4c12b89f6a8145855d3c4eb0e79` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `2221258a51ae32209ae556bc84caa0a9` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `505756b849916dd3c0b88a72924364fd` | ASAM ASAP2 ECU Description File |
| `R4C9J7V5B_5d55-070_120_005_v7.2.3.a2l` | **2015–2026** | 487.8 KB | `aaabe5dce5392f1f539854ddf11bc790` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.2.3.a2l` | **2015–2026** | 483.2 KB | `395de902d0cf4a1f0c331d2929524e12` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.2.3.a2l` | **2015–2026** | 483.2 KB | `6721530e41b452557876cc2836c84489` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.2.3.a2l` | **2015–2026** | 483.2 KB | `3df7b61f2238ce87ad3c3d2d3306c78e` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.2.3.a2l` | **2015–2026** | 483.2 KB | `c2c5d4f305e2040cf084153e74eb93a7` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.2.3.a2l` | **2015–2026** | 483.2 KB | `55f0b2e9739f795d108503dfa5d91dcf` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.2.3.a2l` | **2015–2026** | 483.2 KB | `ab6e29fa8f0a85fcf489b9093ab82658` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.2.3.a2l` | **2015–2026** | 483.2 KB | `75f9c5632b85c5b9691fa618d0d63753` | ASAM ASAP2 ECU Description File |
| `R4C9L8V6B_5d55-080_100_006_v7.2.3.a2l` | **2015–2026** | 483.2 KB | `0b7411641b02da3d3b31b4caf97ff292` | ASAM ASAP2 ECU Description File |

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
