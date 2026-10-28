# v7.2.3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.2.3`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `25 files` (0 binary dumps, 25 definition maps)  

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
| `R0C9J8B2B_3081-080_017_002_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `46344edaa7bf84e8346e01b16190530c` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `86c1ad03a900b2fe18922e58ca96a275` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `1a448ebdad32c22b6f955c75a1ca89b6` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `89c4f263825346d0859f85d30400ddfd` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `00fb118961c2e4b6fe04edffe0e7c73c` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `04c604402a46670c42a9c26faa73099a` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `d02eff343b8c16d0f42fb512747870c1` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `0e3636bf014f1df72ec0d60c52e8077e` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `30d4e5c0cedf7d63575830c2fcdd03b8` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `34d63338150f58058d6ab97feb0e0504` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `044ab2af79dfc1064a3a2853ef8c2005` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.2.3.a2l` | **2015–2026** | 483.3 KB | `c150de755d44f40efacedb6832735359` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.2.3.a2l` | **2015–2026** | 458.1 KB | `e62a913ce9375e81a1dd1c906ff9219f` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `1e59ee054a4e1f210f3c928cf6491bb9` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.2.3.a2l` | **2015–2026** | 485.0 KB | `ac8ae217880e69cd363dfa44c359c42f` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `c0718516ffb296b2cd684821ca824ecc` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `b3ae448b3f27da0dbac4e48df84a7979` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `79db803db6fe77c2c17a6439df7dbe54` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.2.3.a2l` | **2015–2026** | 485.0 KB | `b07f42aaaa9f8ee3427a5426094b739d` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `e746fb7cc7f84ab9564c51090d0e3ea7` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `7352d1daf0694181f938db64033686b3` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `4eba9062b6fee8e412a569546f71f570` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `1fd770e4cf39d0f627af433cf142b425` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `430b9d9a63d9ca775dd29a1146d0cc6d` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.2.3.a2l` | **2015–2026** | 483.6 KB | `3dbf93cab399ea917ba3216d5815d3b7` | ASAM ASAP2 ECU Description File |

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
