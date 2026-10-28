# ACURA_NSX_LEGEND - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/ACURA_NSX_LEGEND`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `19 files` (18 binary dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ACURA_NSX_LEGEND` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1990–2005

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `Acura_NSX_and_Legend.xdf` | **1990–2005** | 622.6 KB | `3b5578088ff49f70ce8ccaa45ced78ad` | TunerPro Binary Definition Map |
| `JDM Type I (PY3-902).BIN` | **1990–2005** | 32.0 KB | `ff6ad98fe87bac672dc7d48a1b713ec5` | Factory Binary Firmware Dump |
| `JDM Type II.bin` | **1990–2005** | 32.0 KB | `7ba31c1093e0cebe8b2bd68707d90011` | Factory Binary Firmware Dump |
| `NSX91M OEM.bin` | **1990–2005** | 32.0 KB | `0280c365621b19d4dd891b38d321ef5c` | Factory Binary Firmware Dump |
| `NSX94M OEM.bin` | **1990–2005** | 32.0 KB | `1749874d307a3d6121600cd4bce4a7e7` | Factory Binary Firmware Dump |
| `PR7-A03.bin` | **1990–2005** | 32.0 KB | `e6a6c7a19715c8d3f792b62262b26c83` | Factory Binary Firmware Dump |
| `PR7-xxx.bin` | **1990–2005** | 32.0 KB | `a9d7c4ae2075a40e9d8fba04a4274a2f` | Factory Binary Firmware Dump |
| `PX9-A05, A15, A04, A55, A65.bin` | **1990–2005** | 32.0 KB | `0d19d91e0e4173d7d179e266ee1a7e6d` | Factory Binary Firmware Dump |
| `PX9-A57, A67, L57, A17, A07.bin` | **1990–2005** | 32.0 KB | `3bf1f14adbd56b5be3b3a50823b4d0f2` | Factory Binary Firmware Dump |
| `PX9-L68 - California.bin` | **1990–2005** | 32.0 KB | `bb4d5bb98ca4b475c723dcce3e32fd8f` | Factory Binary Firmware Dump |
| `PY3-A02, A52.bin` | **1990–2005** | 32.0 KB | `758c6309ad1cb14ca05f715e3f5eca68` | Factory Binary Firmware Dump |
| `PY3-A06, A53.bin` | **1990–2005** | 32.0 KB | `758c6309ad1cb14ca05f715e3f5eca68` | Factory Binary Firmware Dump |
| `PY3-A55.bin` | **1990–2005** | 32.0 KB | `83f921ad20a0b8fc6b52bfb2ebc4377e` | Factory Binary Firmware Dump |
| `PY3-A57.BIN` | **1990–2005** | 64.0 KB | `ca65a201725c97ed4a608f82b70b0d3b` | Factory Binary Firmware Dump |
| `PY3-A58.bin` | **1990–2005** | 32.0 KB | `2fb2e2fe57dcf98fb9a5896d9a50a000` | Factory Binary Firmware Dump |
| `PY3-A72.bin` | **1990–2005** | 32.0 KB | `755d3850fbd07d3ede94eab9df7b70eb` | Factory Binary Firmware Dump |
| `PY3-G52 European.BIN` | **1990–2005** | 32.0 KB | `b0a0f0636524f917163f2dc04c5b4f2c` | Factory Binary Firmware Dump |
| `PY3-Y52 Guatemala.bin` | **1990–2005** | 32.0 KB | `db7c882d1db09352c9a311dcfe837ff8` | Factory Binary Firmware Dump |
| `Py3-A58 stock.bin` | **1990–2005** | 32.0 KB | `ef0208ac8568af52bd6d2d39f5a29e67` | Factory Binary Firmware Dump |

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
