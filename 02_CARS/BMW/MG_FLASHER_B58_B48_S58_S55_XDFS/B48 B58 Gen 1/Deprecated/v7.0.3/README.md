# v7.0.3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.0.3`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `25 files` (0 binary dumps, 25 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.0.3` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R0C9J8B2B_3081-080_017_002_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `2106247cb3d4fd9f128a53e8081a5e49` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `6cd55c60f872cbead50c8fa8d5250071` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `d37648f0ac726af2a06eb52794614e31` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `0049197921c8065f275bce11d51aae65` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `b24ad6b98840e5cccedd1b16f7f904f5` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `c0e8273d5fede9fbc2524488441a9214` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `f990f0d4587a26a2d513dc8c306fe482` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `90fb6874e968ae83946e41121b4ca289` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `b0e4be1005c158c05863fbb9161082b5` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `b69a2a73b90cd4b10594eefcfa42cce8` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `eeafb3d474001c1ceb4c43dcfbb55a48` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `8df1b0e94540d062fcc0d1c5b3ab3584` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.0.3.a2l` | **2015–2026** | 152.6 KB | `a86b0f76dbf63459e09fd291835fe55c` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `d1c430847d93198f3a5f0afc9413b1c3` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.0.3.a2l` | **2015–2026** | 161.3 KB | `d580b130ca0ae18a904d21157a462b43` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `16e1ed739e3158dc003b8ad40085ce4d` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `7ec69051c944d3c52ad1b115c91c633f` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `ef4a8ca7373bab6edce8cb701c7f07a9` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `9f2375dab4b35c6633bf307aa0a30540` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `2983a8545cfada4565ca2946ba013224` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `fbda74a8e0ce7a27d8b12238594b5d8a` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `f7fad6694db0f1dd42e835d5924c6f3b` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `50e876c614641514816113b566b2a75e` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `3dc3898cfd2ffd18830c56d9c9c70ccf` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.0.3.a2l` | **2015–2026** | 152.7 KB | `35af80825f1403725f816eeb851de79a` | ASAM ASAP2 ECU Description File |

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
