# ECUFLASH_XML_DEFS - ECU Calibration Suite

**Repository Path**: `02_CARS/MITSUBISHI/GALANT_LEGNUM_VR4_6A13TT/ECUFLASH_XML_DEFS`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `9 files` (0 binary dumps, 9 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ECUFLASH_XML_DEFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1996–2002

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `20030010.xml` | **1996–2002** | 28.0 KB | `c5e9c7c9a06ac7c31714e86067c7c894` | ECU / XML Calibration Map Definition |
| `20030011.xml` | **1996–2002** | 28.0 KB | `00f7d4192828a8ab6e82cc375f1c1b46` | ECU / XML Calibration Map Definition |
| `20030013.xml` | **1996–2002** | 28.0 KB | `f5a929a9072734e04b9688540efa8dc1` | ECU / XML Calibration Map Definition |
| `22250305.xml` | **1996–2002** | 886 B | `b3163cbb551e0de3298362da3262355e` | ECU / XML Calibration Map Definition |
| `23810003.xml` | **1996–2002** | 28.0 KB | `2eac9d0ac78e0b908979b7ad49d5daf8` | ECU / XML Calibration Map Definition |
| `23810004.xml` | **1996–2002** | 28.0 KB | `f93c147de6d33e5eeca85329195fcffa` | ECU / XML Calibration Map Definition |
| `EMKS11.xml` | **1996–2002** | 12.8 KB | `5aea16f0b08ea26260c7f55dfca372d9` | ECU / XML Calibration Map Definition |
| `vr4_AT_base.xml` | **1996–2002** | 14.5 KB | `7c189061f85c8d3a32e49c4d1e6f3767` | ECU / XML Calibration Map Definition |
| `vr4base.xml` | **1996–2002** | 67.4 KB | `8345c86a0e1a2936dfbca7b1141806a3` | ECU / XML Calibration Map Definition |

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
