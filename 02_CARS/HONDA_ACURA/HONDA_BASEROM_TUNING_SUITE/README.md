# HONDA_BASEROM_TUNING_SUITE - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/HONDA_BASEROM_TUNING_SUITE`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `30 files` (30 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `HONDA_BASEROM_TUNING_SUITE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1992–2000

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `BMTune_V1.0.0.bin` | **1992–2000** | 32.0 KB | `f70dca12e790e887447a460f8b40e601` | Factory Binary Firmware Dump |
| `BMTune_V1.0.1.bin` | **1992–2000** | 32.0 KB | `a6a33c26b5a20971bfad769dce126bec` | Factory Binary Firmware Dump |
| `BMTune_V1.0.2.bin` | **1992–2000** | 32.0 KB | `7f1d013a43353fe1d2ca4a40d0ca0f45` | Factory Binary Firmware Dump |
| `BMTune_V1.0.2_NO_MOD.bin` | **1992–2000** | 32.0 KB | `162ef252b2dc5d3703028e1a9a15cce8` | Factory Binary Firmware Dump |
| `BMTune_V1.0.3.bin` | **1992–2000** | 32.0 KB | `4bbfdd7241811528f31fa9149cc8d28e` | Factory Binary Firmware Dump |
| `BMTune_V1.0.3_NO_MOD.bin` | **1992–2000** | 32.0 KB | `eb49ea1df7633c28bf17202a67cfe57e` | Factory Binary Firmware Dump |
| `BMTune_V1.0.4.bin` | **1992–2000** | 32.0 KB | `9e10c86989d97117ff5a7aef25e69a64` | Factory Binary Firmware Dump |
| `BMTune_V1.0.4_NO_MOD.bin` | **1992–2000** | 32.0 KB | `fa5d39417eb08f3dae74b39e4e09b471` | Factory Binary Firmware Dump |
| `BMTune_V1.0.5.bin` | **1992–2000** | 32.0 KB | `87bb8d90f3aa01f48a7e2be97f9fdbca` | Factory Binary Firmware Dump |
| `BMTune_V1.0.5_NO_MOD.bin` | **1992–2000** | 32.0 KB | `1bbae2f71585a79ea60a65cc5b9face9` | Factory Binary Firmware Dump |
| `BMTune_V1.0.6.bin` | **1992–2000** | 32.0 KB | `cb9b7bb00e990f9b9782416d8ad46d4e` | Factory Binary Firmware Dump |
| `BMTune_V1.0.6_NO_MOD.bin` | **1992–2000** | 32.0 KB | `5efcd35a9ad1fd65b3dd24e74365cd10` | Factory Binary Firmware Dump |
| `BMTune_V1.0.7.bin` | **1992–2000** | 32.0 KB | `4f2be07be613adcb4aa5812837a36204` | Factory Binary Firmware Dump |
| `BMTune_V1.0.7_NO_MOD.bin` | **1992–2000** | 32.0 KB | `2493805c36d0d7ffa4eb3a5b3721a8d1` | Factory Binary Firmware Dump |
| `BMTune_V1.0.8.bin` | **1992–2000** | 32.0 KB | `8686b23133c64c3a17b2e46768a4e39b` | Factory Binary Firmware Dump |
| `BMTune_V1.0.8_NO_MOD.bin` | **1992–2000** | 32.0 KB | `b8878313ae57a69829a61ae37c726e6d` | Factory Binary Firmware Dump |
| `BMTune_V1.0.9.bin` | **1992–2000** | 32.0 KB | `672533024a8247c01c5283d9b83859a3` | Factory Binary Firmware Dump |
| `BMTune_V1.0.FF.bin` | **1992–2000** | 32.0 KB | `d55c392b5635701ac5ab10b62f559417` | Factory Binary Firmware Dump |
| `BMTune_V1.1.0.bin` | **1992–2000** | 32.0 KB | `57054941ac36cb2a626eee5486263f6d` | Factory Binary Firmware Dump |
| `BMTune_V1.1.1.bin` | **1992–2000** | 32.0 KB | `59c5676665a4eae698ea7200ab573701` | Factory Binary Firmware Dump |
| `BMTune_V1.1.2.bin` | **1992–2000** | 32.0 KB | `5d2e9cc74073836b63c7f2394ab3c9b1` | Factory Binary Firmware Dump |
| `BMTune_V1.1.3.bin` | **1992–2000** | 32.0 KB | `46e27344177034a1c131e1c426efcbb2` | Factory Binary Firmware Dump |
| `BMTune_V1.1.4.bin` | **1992–2000** | 32.0 KB | `d9a489751e4b69383a3f397e37214a7c` | Factory Binary Firmware Dump |
| `BMTune_V1.1.5.bin` | **1992–2000** | 32.0 KB | `0f091f658761602df7a24783683be0dd` | Factory Binary Firmware Dump |
| `BMTune_V1.1.6.bin` | **1992–2000** | 32.0 KB | `e2d5f1ed837f5b80955ebfd8817aef27` | Factory Binary Firmware Dump |
| `BMTune_V1.1.7.bin` | **1992–2000** | 32.0 KB | `b3bbf2e6ebe22b917849a7926c5d491b` | Factory Binary Firmware Dump |
| `BMTune_V1.1.8.bin` | **1992–2000** | 32.0 KB | `7f8a7e96cb9809a1b86129128c020073` | Factory Binary Firmware Dump |
| `BMTune_V1.1.9.bin` | **1992–2000** | 32.0 KB | `2fe160836452f1e3760d3f1beb4b4901` | Factory Binary Firmware Dump |
| `BMTune_V1.2.0.bin` | **1992–2000** | 32.0 KB | `090f492ee63b095f3ce49f854db74a24` | Factory Binary Firmware Dump |
| `BMTune_V1.2.1.bin` | **1992–2000** | 32.0 KB | `36f4cd9375ed1c94fd39f5627a55e02c` | Factory Binary Firmware Dump |

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
