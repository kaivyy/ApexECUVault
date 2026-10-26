# NAKED VIXION MT15 - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/YAMAHA/NAKED_VIXION_MT15`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `9 files` (2 binary dumps, 7 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `NAKED_VIXION_MT15` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `GENERATIONAL_3C1-H591A-00_Yamaha_Vixion_3C1_Gen_1_Old_(2007-2012).xdf` | `.XDF` | `5,561` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_BBS-H591A-00_Yamaha_XSR_155_Heritage_2019_2025_K_Line.xdf` | `.XDF` | `2,544` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_BBS-H591A-10_Yamaha_XSR_155_Connected_2023_2025_CANBUS.xdf` | `.XDF` | `2,545` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_BK7-H591A-00_Yamaha_All_New_Vixion_150_Gen_4_Assist_Slipper_(2017-2024).xdf` | `.XDF` | `5,581` bytes | TunerPro Binary Definition Map |
| `MT_15_B8D0.bin` | `.BIN` | `27,648` bytes | Yamaha Factory Renesas RL78 / Denso ROM |
| `MT_15_BHM0.bin` | `.BIN` | `27,648` bytes | Yamaha Factory Renesas RL78 / Denso ROM |
| `YAMAHA_1PA-H591A-00_Yamaha_New_Vixion_Advance_NVA_(1PA).xdf` | `.XDF` | `6,675` bytes | TunerPro Binary Definition Map |
| `YAMAHA_2TP-E591A-00_Yamaha_New_Vixion_Lightning_NVL_(2TP0).xdf` | `.XDF` | `6,689` bytes | TunerPro Binary Definition Map |
| `YAMAHA_B8D-H594A-00_Yamaha_MT-15_(B8D0).xdf` | `.XDF` | `11,857` bytes | Yamaha Factory Renesas RL78 / Denso ROM |

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
