# MetricUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/S58/Generic/MetricUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `14 files` (0 binary dumps, 14 definition maps)  

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
| `F4C9G577B_5c64-010_090_007.MetricUnits.xdf` | **2015–2026** | 987.3 KB | `6c8c6393928209dc5f2a91d009cb34d6` | TunerPro Binary Definition Map |
| `F4C9G595B_5c64-010_100_005.MetricUnits.xdf` | **2015–2026** | 987.3 KB | `6c8c6393928209dc5f2a91d009cb34d6` | TunerPro Binary Definition Map |
| `F4C9G5F5B_5c64-010_130_005.MetricUnits.xdf` | **2015–2026** | 987.3 KB | `df365bb6e0513661cf79b1fa7482a1ac` | TunerPro Binary Definition Map |
| `F4C9G5H5B_5c64-010_140_005.MetricUnits.xdf` | **2015–2026** | 987.3 KB | `3644063970290f7bfacef7807fae1702` | TunerPro Binary Definition Map |
| `F4C9L8A6B_5c64-020_050_006.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `666914ca7359a56849ff6fd37eab8a41` | TunerPro Binary Definition Map |
| `F4C9L8C5B_5c64-020_060_005.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `eb31802919c5acf1ea0b3436a5be0ce9` | TunerPro Binary Definition Map |
| `F4C9L8E6B_5c64-020_070_006.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `abef4d246b6142468bb7dc891ff57152` | TunerPro Binary Definition Map |
| `F4C9L8G7B_5c64-020_080_007.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `24a1a1555fa4335713f7f18a9f53008c` | TunerPro Binary Definition Map |
| `F4C9L8J5B_5c64-020_090_005.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `9dc00bb3d27c26ef72f4194198784616` | TunerPro Binary Definition Map |
| `F4C9L8N6B_5c64-020_110_006.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `43f7428dac2128e6b70e0e5c6345b826` | TunerPro Binary Definition Map |
| `F4C9L8R5B_5c64-020_130_005.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `ff23c51e8038f3e0cb1cd72d8afaf7a5` | TunerPro Binary Definition Map |
| `F4C9L8R6B_5c64-020_135_006.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `ff23c51e8038f3e0cb1cd72d8afaf7a5` | TunerPro Binary Definition Map |
| `F4C9L8Y8B_5c64-020_200_008.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `74326182c662e4b18fbde6ec25e6614b` | TunerPro Binary Definition Map |
| `F4C9LU16B_aed2-020_060_006.MetricUnits.xdf` | **2015–2026** | 1008.2 KB | `3cb1dc6bc6e69d5d7e416045bf8fa17e` | TunerPro Binary Definition Map |

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
