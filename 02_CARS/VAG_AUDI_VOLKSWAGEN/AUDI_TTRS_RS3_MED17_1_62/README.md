# AUDI_TTRS_RS3_MED17_1_62 - ECU Calibration Suite

**Repository Path**: `02_CARS/VAG_AUDI_VOLKSWAGEN/AUDI_TTRS_RS3_MED17_1_62`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `10 files` (3 binary dumps, 7 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `AUDI_TTRS_RS3_MED17_1_62` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2009–2016

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `404A_normal.xdf` | **2009–2016** | 3.35 MB | `5d9a89b73cf8871fb1f8a1066a524b32` | TunerPro Binary Definition Map |
| `404E_normal.xdf` | **2009–2016** | 6.32 MB | `bb2f80d0d05e130c4b0708b48a3cd8b9` | TunerPro Binary Definition Map |
| `404G_normal.xdf` | **2009–2016** | 3.35 MB | `5d9a89b73cf8871fb1f8a1066a524b32` | TunerPro Binary Definition Map |
| `404H_normal.xdf` | **2009–2016** | 5.46 MB | `8c1c9c3543e0f274c4e70eed0ce2afbe` | TunerPro Binary Definition Map |
| `404J_normal.xdf` | **2009–2016** | 3.32 MB | `ca10276639f32fe3b6f5a95733be2849` | TunerPro Binary Definition Map |
| `404L_normal.xdf` | **2009–2016** | 2.77 MB | `3c1c5ce2909f976ce725304c10ed4669` | TunerPro Binary Definition Map |
| `MED17_1_62_8S0907404L__0001_STOCK.bin` | **2009–2016** | 496.0 KB | `ffb9a3977bfe74161f205c2f88cde084` | Factory Binary Firmware Dump |
| `MED17_1_62_STOCK.bin` | **2009–2016** | 496.0 KB | `980065172d9069ceb371bd5af19d98f0` | Factory Binary Firmware Dump |
| `MED17_1_62_STOCK_alt.bin` | **2009–2016** | 496.0 KB | `0e2328309795542012b4266d14b9850a` | Factory Binary Firmware Dump |
| `MED17_D17162A01C000.ecu` | **2009–2016** | 4.40 MB | `e04b9358f3eb84a076dd95f3226a3bd8` | ECU / XML Calibration Map Definition |

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
