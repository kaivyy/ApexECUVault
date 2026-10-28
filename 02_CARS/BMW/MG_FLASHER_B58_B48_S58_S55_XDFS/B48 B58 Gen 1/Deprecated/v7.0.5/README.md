# v7.0.5 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.0.5`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `25 files` (0 binary dumps, 25 definition maps)  

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
| `R0C9J8B2B_3081-080_017_002_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `7396dbc94de6116f053c406ed44aaa0e` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `b400aa0bae0b8c1419a2fef8090e16f2` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `2eddb58cd010600a8aaa9228cecef2ea` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `32b5836b4568766d498ae8cfd259bda1` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `b3a6d085105f1e1fef9521db2779db9f` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `9c3046d0555daf08825638fafc26cdbf` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `a75b4c44fcfd7c4292077f11adf81c22` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `dedc0f4428b8437ccd86c5a6f99e144f` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `188d9ae156c463808bdfcc8c60b0c573` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `c599035461631c4c21174d72414bfa81` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `406f16833d3c991813d5cb8f4015d6ae` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.0.5.a2l` | **2015–2026** | 168.3 KB | `e969e94e30344a56a251ec540afc9b28` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.0.5.a2l` | **2015–2026** | 167.4 KB | `3b10a115975276c19e6ab1e57cbf9e51` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `179d3dd2badc094781b2259581b7c023` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `f00cfa703859be75eb2c3160e91eda88` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `28741a059b753d4eab615b8155c5359f` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `1e22d2f54774c6a4ee1817ff726ad44d` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `853e24b04b12c4419453f7dbd2b480af` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `ac2eb77f95a69c1985036a45246d9fa2` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `ac59461a679d0eb5639d25787e80e6f5` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `a9540446cfb597c357c46793cf8cfba9` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `eeeb79793204e6e9d6605f0f35603670` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `fbdb8a15c59adb5b9878ec1290850da3` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `3d05c61001c2439d714ba0c697fab892` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.0.5.a2l` | **2015–2026** | 168.4 KB | `31185e01dd73db5bc36cafdbccd0467e` | ASAM ASAP2 ECU Description File |

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
