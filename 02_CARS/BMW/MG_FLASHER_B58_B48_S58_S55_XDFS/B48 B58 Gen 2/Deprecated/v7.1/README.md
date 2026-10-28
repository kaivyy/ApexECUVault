# v7.1 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.1`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `38 files` (0 binary dumps, 38 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.1` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R4C9F4E6B_5d55-040_150_006_v7.1.a2l` | **2015–2026** | 179.1 KB | `795154f9d16f00d90c57a77631fcbda7` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.1.a2l` | **2015–2026** | 179.1 KB | `ec03de9fbcc0bcc4b8a86757b7137138` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.1.a2l` | **2015–2026** | 179.1 KB | `f758f0042313679a1cf4e2ae287dcac2` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.1.a2l` | **2015–2026** | 179.1 KB | `373980da97ef1a8794971bcb448cff6e` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.1.a2l` | **2015–2026** | 179.1 KB | `fa0087de62d9dcb8a308a6d82ed5ea5a` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `a3961f128c243e5cdac9677529d1bc1d` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `ccd879b96779134c6105edb818d3f5dd` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `62aad654fdc635a9e7156de83b519fd4` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.1.a2l` | **2015–2026** | 180.9 KB | `bf525956987d93a1981c210ec3611844` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `56835fbb0d1f92f7d46960ed6e91734b` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.1.a2l` | **2015–2026** | 180.9 KB | `94327d19b577268815fa0f44edd4e2e5` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.1.a2l` | **2015–2026** | 180.9 KB | `cc98fc981ea634599866040e5a3eb2da` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `612a9f62ebdbd09d55bb009f22ef817f` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `39107634b653f8e9de3f3a1dff7a7f60` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `599c2dee5cf1992580e87aea5fbb67dd` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `0e4b6332a02e1fe53556671d944b04c1` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `9d5f199826f5c03b889c66c45ce16be7` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `f026fe39a44ef78df9ac9d1de8de9260` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `91fc520e6e90fa469ed6ec8ffd5387b5` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.1.a2l` | **2015–2026** | 180.9 KB | `fbce6810d24d2ca48795c2dc79dbb6a3` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.1.a2l` | **2015–2026** | 180.9 KB | `598e960e21f093f222f511d301f146e3` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.1.a2l` | **2015–2026** | 180.9 KB | `efa48a89a2fc1e2455fac06fb1417aaa` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `bd134bac54d5f05e842e1189461638a9` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.1.a2l` | **2015–2026** | 180.9 KB | `3d16e4aafc83af331292c08e196f87ed` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.1.a2l` | **2015–2026** | 180.9 KB | `97ab5419c44a61c13d716fc1bf04c7f5` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `53cec47c19ddd32fcaf96d3c35e6e92b` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `eef392d9471e532b09ceffc5858713e5` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `1142fe3ecb370e1416ae23f8f51a88b0` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `f07fb9f41f0ab86a9ceeef7f98fa655a` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.1.a2l` | **2015–2026** | 180.9 KB | `c1cc61c1ab2438b09f552b11f10a05ee` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.1.a2l` | **2015–2026** | 180.9 KB | `e65a2c2d9b9b1459c51daefea79f60b4` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `2a204408b7a6b88933d696dc91190bca` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `d7049d3a69acf3d51f3919c11b22420f` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.1.a2l` | **2015–2026** | 180.9 KB | `2854b84782cd8cde7d821bd5e340ccf5` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.1.a2l` | **2015–2026** | 180.9 KB | `b6787ce2dceb117912ebf2c9bda3de78` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.1.a2l` | **2015–2026** | 180.9 KB | `66d4ad5f2bdffec4ec5f5a0ac534c425` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.1.a2l` | **2015–2026** | 180.9 KB | `d123eab05bf9bb62951e3d68f2aee6f5` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.1.a2l` | **2015–2026** | 180.9 KB | `4fa964597e41f1fcd0fb457e503c06e7` | ASAM ASAP2 ECU Description File |

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
