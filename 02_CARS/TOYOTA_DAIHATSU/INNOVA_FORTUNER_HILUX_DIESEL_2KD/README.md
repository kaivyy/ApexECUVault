# INNOVA FORTUNER HILUX DIESEL 2KD - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/INNOVA_FORTUNER_HILUX_DIESEL_2KD`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `10 files` (6 binary dumps, 4 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `INNOVA_FORTUNER_HILUX_DIESEL_2KD` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2004–2015

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `GENERATIONAL_89663-0K180_INNOVA_NON_IC_Toyota_Kijang_Innova_2.5_D-4D_Gen_1_Non-Intercooler_(2004-2011).xdf` | **2004–2011** | 5.4 KB | `f3d847d8821a7774206d6b2897dcc339` | TunerPro Binary Definition Map |
| `GENERATIONAL_89663-0K750_INNOVA_VNT_Toyota_Kijang_Innova_2.5_D-4D_Gen_1_VN-Turbo_Intercooler_(2011-2015).xdf` | **2011–2015** | 5.4 KB | `226aa21afde583f159d71a00e9b3615d` | TunerPro Binary Definition Map |
| `GENERATIONAL_89663-0K750_Toyota_Innova_2.5_D_4D_VN_Turbo_Intercooler_2011_2015.xdf` | **2011–2015** | 1.5 KB | `8f8354630cfd53fd245e6584e3afcbc9` | TunerPro Binary Definition Map |
| `TOYOTA_89663-0K180_2KD.xdf` | **2004–2015** | 11.8 KB | `40354a237258699f8cac86235dfd0201` | TunerPro Binary Definition Map |
| `TOYOTA_FORTUNER_INNOVA_2012_2.7L_2TRFE_AUTO_89663-0K630.bin` | **2012** | 368.0 KB | `bc9e8ac16f923a62af7413c6e63ea86f` | Factory Binary Firmware Dump |
| `TOYOTA_FORTUNER_INNOVA_2014_2.7L_2TRFE_AUTO_89663-0KX30.bin` | **2014** | 512.0 KB | `056b4788d3e706ef9f9050895a27fa7b` | Factory Binary Firmware Dump |
| `TOYOTA_HIACE_HILUX_2011_2.5TD_2KDFTV_89663-26331.bin` | **2011** | 368.0 KB | `b3cbd5f50d25442e9e5562e4163009d8` | Factory Binary Firmware Dump |
| `TOYOTA_INNOVA_HILUX_2012_2.5TD_2KDFTV_MANUAL_89663-0KM60.bin` | **2012** | 496.0 KB | `c871a59bb497d208b5d63aa440003a01` | Factory Binary Firmware Dump |
| `TOYOTA_INNOVA_HILUX_2013_2.5TD_2KDFTV_MANUAL_89663-0KM63.bin` | **2013** | 496.0 KB | `bba31550b1c308a9270c562cd6930911` | Factory Binary Firmware Dump |
| `TOYOTA_INNOVA_HILUX_VNT_2014_2.5TD_2KDFTV_AUTO_89663-0KR70.bin` | **2014** | 992.0 KB | `5d52e47279a8ffcb3de351d13a0ad687` | Factory Binary Firmware Dump |

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
