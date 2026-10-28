# v7.0 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.0`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `25 files` (0 binary dumps, 25 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.0` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R0C9J8B2B_3081-080_017_002_v7.0.a2l` | **2015–2026** | 171.4 KB | `749109edd82922f03c65c0a9afa592e8` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.0.a2l` | **2015–2026** | 171.4 KB | `e600005943ec9a6deb5d5eda86e6c405` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.0.a2l` | **2015–2026** | 171.4 KB | `a583ba3ac72dbf727fb49b660ba5f74f` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.0.a2l` | **2015–2026** | 171.4 KB | `86e38d224104623f9a6d43b762be57ef` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.0.a2l` | **2015–2026** | 171.4 KB | `7d7410a413899df6cfd219f6fdc479f9` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.0.a2l` | **2015–2026** | 171.4 KB | `f7b26833aa1b974da3c260aa90054b52` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.0.a2l` | **2015–2026** | 171.4 KB | `043fbe9230f3f01c2e54581f361f1718` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.0.a2l` | **2015–2026** | 171.4 KB | `54383fef82e93d23bc3a5d6a6126be44` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.0.a2l` | **2015–2026** | 171.4 KB | `7b4159aaa094087852c69f67db764fe1` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.0.a2l` | **2015–2026** | 171.4 KB | `003434761ddcdb28feedb744bfa09dd8` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.0.a2l` | **2015–2026** | 171.4 KB | `ffccfbdc6c029d3c79b9f7b6e3d93a30` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.0.a2l` | **2015–2026** | 171.4 KB | `1397a14af7014514f941d3befb3c8644` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.0.a2l` | **2015–2026** | 171.5 KB | `2595ed52ff02c4bf92943fae33fcaf1c` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.0.a2l` | **2015–2026** | 171.6 KB | `60028dc1d2f7150a8cc5be4c8368f248` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.0.a2l` | **2015–2026** | 171.6 KB | `69393dcfbc6ef5eb85b9781c138adebc` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.0.a2l` | **2015–2026** | 171.6 KB | `6da391b663c90230954e62112efe4719` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.0.a2l` | **2015–2026** | 171.6 KB | `4419bc5f72d36278de719e6404c5cc1f` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.0.a2l` | **2015–2026** | 171.6 KB | `655ff47bd21463207c420c24db731d38` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.0.a2l` | **2015–2026** | 171.6 KB | `eb053d2902475bcfe0d0bfecbcb6e8e4` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.0.a2l` | **2015–2026** | 171.6 KB | `68fea378f4f163c1b66e582b2f72d83e` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.0.a2l` | **2015–2026** | 171.6 KB | `7e19171b6597d164728614bca0f7d3b7` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.0.a2l` | **2015–2026** | 171.6 KB | `28422412bd25612bfce4d8b9782ab138` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.0.a2l` | **2015–2026** | 171.6 KB | `3e88f0235cf945d89edfa8fc89c020da` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.0.a2l` | **2015–2026** | 171.6 KB | `842f09a47be2b8480903ff8de1b7d0d8` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.0.a2l` | **2015–2026** | 171.6 KB | `ae42f48a60d22fa8e5923edf066b1f7f` | ASAM ASAP2 ECU Description File |

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
