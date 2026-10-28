# MINI_MOTO_GROM_MONKEY - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/MINI_MOTO_GROM_MONKEY`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `16 files` (5 binary dumps, 11 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MINI_MOTO_GROM_MONKEY` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `38770-K0F-A01.bin` | **2000–2024** | 96.0 KB | `b1b2d8fbdb85538f1b764e9059f0def5` | Factory Binary Firmware Dump |
| `38770-K0F-A01.xdf` | **2000–2024** | 15.5 KB | `cdffe0fc5392f14f81a4456a9e4c2f34` | TunerPro Binary Definition Map |
| `38770-K26-911.bin` | **2000–2024** | 48.0 KB | `eca31aa92cd73763dd6500174de10e0c` | Factory Binary Firmware Dump |
| `38770-K26-911.xdf` | **2000–2024** | 13.8 KB | `707232a042ceed90cd85b7aa09c88505` | TunerPro Binary Definition Map |
| `38770-K26-931.bin` | **2000–2024** | 48.0 KB | `cf324b8b009cf0f527ef34d8d6ba5021` | Factory Binary Firmware Dump |
| `38770-K26-B13.bin` | **2000–2024** | 64.0 KB | `3ce4aee4afaddf4d8ca3f194b13fc168` | Factory Binary Firmware Dump |
| `38770-K26-B13.xdf` | **2000–2024** | 12.5 KB | `5d433c3d0f453a7b4c72d425831b14e0` | TunerPro Binary Definition Map |
| `38770-K26-C31.bin` | **2000–2024** | 64.0 KB | `4ebb017f7ca9287ae5c54db3a8704106` | Factory Binary Firmware Dump |
| `38770-K26-C31.xdf` | **2000–2024** | 23.9 KB | `1d4c0cfe07e37230dd4b486fe80b2dc5` | TunerPro Binary Definition Map |
| `HONDA_38770-K0F-A01_Monkey_125_(2018-2020).xdf` | **2018–2020** | 16.3 KB | `ac6b42835a4acb708a145356c2d02960` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-901_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `d95896040243327d1aea4c12b2832cd3` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-911_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `802787442ffb7ba2f3a22e267dd30dcc` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-931_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `570e180502c1134751d23dfd3d39b64a` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-B02_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `08150f1f1ed5dcf906901a272e97b5f8` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-B13_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `56e94d9ce6e1975bea81247a6fcac38b` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-C31_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `8e252df9c45da9a0ae39467942fda777` | TunerPro Binary Definition Map |

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
