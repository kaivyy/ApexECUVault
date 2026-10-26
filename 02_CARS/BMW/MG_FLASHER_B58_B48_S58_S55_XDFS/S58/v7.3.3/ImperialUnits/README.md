# ImperialUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/S58/v7.3.3/ImperialUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `12 files` (0 binary dumps, 12 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ImperialUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `F4C9G577B_5c64-010_090_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.88 MB | `91ea56bb1bd243ef91f2f942bacf5aea` | TunerPro Binary Definition Map |
| `F4C9G595B_5c64-010_100_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.88 MB | `91ea56bb1bd243ef91f2f942bacf5aea` | TunerPro Binary Definition Map |
| `F4C9G5F5B_5c64-010_130_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.88 MB | `78b7fd2d2c7f616cd6e9471dfa8dcdd4` | TunerPro Binary Definition Map |
| `F4C9G5H5B_5c64-010_140_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.88 MB | `4b393e71b8557859f7fc00665ab8f43c` | TunerPro Binary Definition Map |
| `F4C9L8A6B_5c64-020_050_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.91 MB | `dd78a3ce64714933fd87cdb4855683c8` | TunerPro Binary Definition Map |
| `F4C9L8C5B_5c64-020_060_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.91 MB | `41b389cc214d28d6a8261e7052714fc4` | TunerPro Binary Definition Map |
| `F4C9L8E6B_5c64-020_070_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.91 MB | `d7393b5ad422bffb0eb33d0088d7a83a` | TunerPro Binary Definition Map |
| `F4C9L8G7B_5c64-020_080_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.91 MB | `e692f9257ea95d9a0322a4d7a983876e` | TunerPro Binary Definition Map |
| `F4C9L8J5B_5c64-020_090_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.91 MB | `fbee93b2bd1b8a2efe932adbc4e434d7` | TunerPro Binary Definition Map |
| `F4C9L8N6B_5c64-020_110_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.91 MB | `4f7c03e0de859dbe41d87ad776991a0e` | TunerPro Binary Definition Map |
| `F4C9L8R5B_5c64-020_130_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.91 MB | `1ee244d0e4334801a5689a3a9a3d6426` | TunerPro Binary Definition Map |
| `F4C9L8Y8B_5c64-020_200_008_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.97 MB | `5c08045a94b3368dd5ce79826ac82aac` | TunerPro Binary Definition Map |

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
