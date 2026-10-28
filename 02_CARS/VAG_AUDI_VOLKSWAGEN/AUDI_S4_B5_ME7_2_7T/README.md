# AUDI_S4_B5_ME7_2_7T - ECU Calibration Suite

**Repository Path**: `02_CARS/VAG_AUDI_VOLKSWAGEN/AUDI_S4_B5_ME7_2_7T`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `9 files` (5 binary dumps, 4 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `AUDI_S4_B5_ME7_2_7T` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1999–2002

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `4Z7907551AA.kp` | **1999–2002** | 20.4 KB | `64318b2e1ad17db7cd98e7d2b44c240b` | WinOLS Map Definition Pack |
| `4Z7907551R.kp` | **1999–2002** | 2.32 MB | `7919ca7138e62600f808f15c30b0ad17` | WinOLS Map Definition Pack |
| `8D0907551M-0002 (16Bit KFZW).bin` | **1999–2002** | 1.00 MB | `7cf3feb94b32e877b1d30eed34e57997` | Factory Binary Firmware Dump |
| `8D0907551M-0002 (stock MAP 5120 16Bit KFZW).bin` | **1999–2002** | 1.00 MB | `f11bfcc8df64c11bd858ee413f940386` | Factory Binary Firmware Dump |
| `8D0907551M-0002 (stock MAP 5120).bin` | **1999–2002** | 1.00 MB | `9e2598740860ba3548821914b523b8d9` | Factory Binary Firmware Dump |
| `8D0907551M-0002.bin` | **1999–2002** | 1.00 MB | `d56d9801e27145a77fc7bab1164e54eb` | Factory Binary Firmware Dump |
| `8D0907551M-002_5120-stock_map-nyet.bin` | **1999–2002** | 1.00 MB | `533e3a19b75ba0f6d922c4208d684e32` | Factory Binary Firmware Dump |
| `8D0907551M-20170411-16bit-kfzw.xdf` | **1999–2002** | 493.1 KB | `f6d19bcf33e6a35e842ddb2ab46fa343` | TunerPro Binary Definition Map |
| `8D0907551M-20190711.xdf` | **1999–2002** | 491.8 KB | `7df7ce24a3cea3ad5215b51ab89a417f` | TunerPro Binary Definition Map |

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
