# v7.1 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.1`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `25 files` (0 binary dumps, 25 definition maps)  

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
| `R0C9J8B2B_3081-080_017_002_v7.1.a2l` | **2015–2026** | 176.7 KB | `3e2ff06abf51164703c95d7b36036acb` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.1.a2l` | **2015–2026** | 176.7 KB | `56c2a671fbb8e126d18bb41059581bde` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.1.a2l` | **2015–2026** | 176.7 KB | `7de9b79bef1b7f182c2e1fbdc9ac7a60` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.1.a2l` | **2015–2026** | 176.7 KB | `a6834840c382691c79946ba49882ed6c` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.1.a2l` | **2015–2026** | 176.7 KB | `1ac54017e77e50792cfaa82f435e6746` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.1.a2l` | **2015–2026** | 176.7 KB | `0b30b8471eecd2259b06e2c7270965e5` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.1.a2l` | **2015–2026** | 176.7 KB | `e9f718e1e725c69d27205e7bc0049bcc` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.1.a2l` | **2015–2026** | 176.7 KB | `d532a8f779245831473bd5faeacb26c5` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.1.a2l` | **2015–2026** | 176.7 KB | `2883fd530d4c86149e981fd60d736583` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.1.a2l` | **2015–2026** | 176.7 KB | `7f1b16fa6b6ca7fdf31d0022159f8fd9` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.1.a2l` | **2015–2026** | 176.7 KB | `e65874921dc7442fb5ae5b18bfdb6e7b` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.1.a2l` | **2015–2026** | 176.7 KB | `58af158a8dc45de18d36e9e6f896a688` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.1.a2l` | **2015–2026** | 175.9 KB | `e59fbb90b8be637f5f877efb254b5210` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.1.a2l` | **2015–2026** | 176.9 KB | `fece732d66c65575d7e8e71e04368575` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.1.a2l` | **2015–2026** | 176.9 KB | `ffd50d6e74a8073bb941b4728aee155d` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.1.a2l` | **2015–2026** | 176.9 KB | `2c4577f01a3cf4e679c805ed4da88aef` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.1.a2l` | **2015–2026** | 176.9 KB | `b2d620472b6ee6b0c9d80375d5cf73d6` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.1.a2l` | **2015–2026** | 176.9 KB | `7815e6b0550dbf3e7e8a5f25a9fe7404` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.1.a2l` | **2015–2026** | 176.9 KB | `282d7baf17894489e180f9e41a00dab9` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.1.a2l` | **2015–2026** | 176.9 KB | `815624d6b9a5073b96cfd8bce2289daf` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.1.a2l` | **2015–2026** | 176.9 KB | `f82feca39f46ae6592d32ba92f4d9e3e` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.1.a2l` | **2015–2026** | 176.9 KB | `b6c06686e9ce676055a3136d61a6e608` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.1.a2l` | **2015–2026** | 176.9 KB | `523684688d2094dd245049a853f7ff8d` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.1.a2l` | **2015–2026** | 176.9 KB | `2a9c4403829ab203d345a6ac0837a30e` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.1.a2l` | **2015–2026** | 176.9 KB | `261d649f9d0de31d21e7bb07f9ad5800` | ASAM ASAP2 ECU Description File |

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
