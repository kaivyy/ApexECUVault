# v7.0.2 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.0.2`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `25 files` (0 binary dumps, 25 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.0.2` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R0C9J8B2B_3081-080_017_002_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `b0cbc24c6b78639ed2c30701b92fe26a` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `a89560acac1dcd8955af6f36a448d58a` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `9133c3f3c5c5e3f044009a44b7e537d7` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `d5b3a943b27a9fd7f0146aee8b2c2d5e` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `4453c34047f8fe9d5092eca06c74e1ed` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `5625f3cec7a035cf1da5c736d47f3891` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `82afd390fbe518864318e37fd4a63bf9` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `537589e11c72b95e2b59d6c343401851` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `9461cf61746b6166e63e655c24698d0c` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `4c67eeeb01fcc0795192216733d67cf0` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `ca90c198d71227d7b0534f3095cb82b2` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `07de193375be6a48b195516c52a26c29` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.0.2.a2l` | **2015–2026** | 152.6 KB | `578e5af1eea77239bcb6f95b72676206` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `9400197ef20faba2dff20ec883ceb71b` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.0.2.a2l` | **2015–2026** | 161.3 KB | `a5562b3e1af1e899c70632e7f9de40c5` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `c09341817baf669a22267f39229ade3c` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `e98737201850fa23a77ce5350f94f997` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `09ecb5d92d314e6a3efd51c96fd358df` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `007e61813f9ce3bc47a609774369febf` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `7aa0ed8961dba87229e1b9d40662dd91` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `80a346fad0b6bd97d844a6bba4c4ec73` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `9328078fe656ce5df3efaa5f96af338f` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `ac21a5b378e0cebe555f160c47f85e0c` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `181cc6d6f29eaa408c236e2960587cee` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.0.2.a2l` | **2015–2026** | 152.7 KB | `e3b4fd78596b36060702788e01f6cb60` | ASAM ASAP2 ECU Description File |

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
