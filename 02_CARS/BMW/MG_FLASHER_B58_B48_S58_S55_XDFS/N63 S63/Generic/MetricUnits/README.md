# MetricUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/N63 S63/Generic/MetricUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `27 files` (0 binary dumps, 27 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MetricUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `H4C99274B_4acf-010_050_004.MetricUnits.xdf` | **2015–2026** | 775.3 KB | `80562ce01939e44c099b458b6f1e343f` | TunerPro Binary Definition Map |
| `H4C993A3B_4acf-020_120_003.MetricUnits.xdf` | **2015–2026** | 848.8 KB | `e9d7811b2fdd3ddd10ec4205bc2d939d` | TunerPro Binary Definition Map |
| `H4C99695B_4acf-030_110_005.MetricUnits.xdf` | **2015–2026** | 868.8 KB | `57fd7fcb802b294a47762bd6984eba7a` | TunerPro Binary Definition Map |
| `H4C996B5B_4acf-030_120_005.MetricUnits.xdf` | **2015–2026** | 868.8 KB | `57fd7fcb802b294a47762bd6984eba7a` | TunerPro Binary Definition Map |
| `H4C996H5B_4acf-030_150_005.MetricUnits.xdf` | **2015–2026** | 868.8 KB | `9fd906dc4109dc5552692971cb7eff8d` | TunerPro Binary Definition Map |
| `H4C996K5B_4acf-030_160_005.MetricUnits.xdf` | **2015–2026** | 868.8 KB | `06b3ffa5836ecbf9ab34235a24ca9220` | TunerPro Binary Definition Map |
| `H4C996K6B_4acf-030_160_006.MetricUnits.xdf` | **2015–2026** | 868.8 KB | `06b3ffa5836ecbf9ab34235a24ca9220` | TunerPro Binary Definition Map |
| `H4C996P5B_4acf-030_170_005.MetricUnits.xdf` | **2015–2026** | 868.8 KB | `54272717eac701fbca437b307db66ea7` | TunerPro Binary Definition Map |
| `H4C996R5B_4acf-030_180_073.MetricUnits.xdf` | **2015–2026** | 868.8 KB | `883501d937d56e612915558fa56c7fe5` | TunerPro Binary Definition Map |
| `H4C9L8A5B_4acf-040_110_005.MetricUnits.xdf` | **2015–2026** | 889.3 KB | `e118364ad384d2789cd11a5cf65983d1` | TunerPro Binary Definition Map |
| `H4C9L8E6B_4acf-040_120_006.MetricUnits.xdf` | **2015–2026** | 889.3 KB | `4e83409f4ad530b24627a6713dada4fe` | TunerPro Binary Definition Map |
| `H4C9L8J5B_4acf-040_130_005.MetricUnits.xdf` | **2015–2026** | 889.3 KB | `dc63274b5b29aa1f75516157d543c201` | TunerPro Binary Definition Map |
| `H4C9L8N5B_4acf-040_150_005.MetricUnits.xdf` | **2015–2026** | 889.3 KB | `baf565fc4ee7ecee5eb672b0dd3b4565` | TunerPro Binary Definition Map |
| `V4C9F4K6B_4963-040_170_006.MetricUnits.xdf` | **2015–2026** | 869.0 KB | `f0bfbfba16aa8d3c716c5f278ea40197` | TunerPro Binary Definition Map |
| `V4C9F4N6B_4963-040_180_006.MetricUnits.xdf` | **2015–2026** | 869.0 KB | `dffaadca2f150d8c721fa1fc91536059` | TunerPro Binary Definition Map |
| `V4C9H6H6B_4963-060_130_006.MetricUnits.xdf` | **2015–2026** | 903.1 KB | `7458f4c9306be28d27a13be2aa3ce9d6` | TunerPro Binary Definition Map |
| `V4C9H6N7B_4963-060_150_007.MetricUnits.xdf` | **2015–2026** | 903.1 KB | `a7a77a7eef1a96fa70408c58c89799d6` | TunerPro Binary Definition Map |
| `V4C9H6S8B_4963-060_170_008.MetricUnits.xdf` | **2015–2026** | 903.1 KB | `348cb4085dae556641944900e3aed8a7` | TunerPro Binary Definition Map |
| `V4C9J717B_4963-070_030_007.MetricUnits.xdf` | **2015–2026** | 912.7 KB | `e33e3f24df51482a004c200019d48a97` | TunerPro Binary Definition Map |
| `V4C9J796B_4963-070_060_006.MetricUnits.xdf` | **2015–2026** | 912.7 KB | `6f1633115f0c93f173c5294b8bfd20b4` | TunerPro Binary Definition Map |
| `V4C9J7A5B_4963-070_070_005.MetricUnits.xdf` | **2015–2026** | 912.7 KB | `cd21fcb9f4887e769f1a7d08af42b315` | TunerPro Binary Definition Map |
| `V4C9J7N6B_4963-070_080_006.MetricUnits.xdf` | **2015–2026** | 912.7 KB | `287d8cb4441b4cfa08876991dabae6b1` | TunerPro Binary Definition Map |
| `V4C9J7S8B_4963-070_100_008.MetricUnits.xdf` | **2015–2026** | 912.7 KB | `b93939e9036cfb179b02541197644b24` | TunerPro Binary Definition Map |
| `V4C9J7V5B_4963-070_120_005.MetricUnits.xdf` | **2015–2026** | 912.7 KB | `aed664e91e999c6fcb737b8e24d60807` | TunerPro Binary Definition Map |
| `V4C9J7W5B_4963-070_130_005.MetricUnits.xdf` | **2015–2026** | 912.7 KB | `aed664e91e999c6fcb737b8e24d60807` | TunerPro Binary Definition Map |
| `V4C9L8N6B_4963-080_060_006.MetricUnits.xdf` | **2015–2026** | 900.4 KB | `276ef952dab7e30b9874af0956e6c9d1` | TunerPro Binary Definition Map |
| `V4C9L8S9B_4963-080_080_009.MetricUnits.xdf` | **2015–2026** | 900.4 KB | `39b30bfdd7a45dc9d0a52eee861054dc` | TunerPro Binary Definition Map |

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
