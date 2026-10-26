# MUSTANG FALCON XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/FORD/MUSTANG_FALCON_XDFS`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `19 files` (4 binary dumps, 15 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MUSTANG_FALCON_XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `6DFC.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `6DFD.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `6DGC.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `6DGD.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `CBAZA.xdf` | `.XDF` | `317,307` bytes | TunerPro Binary Definition Map |
| `CDAN4.xdf` | `.XDF` | `172,791` bytes | TunerPro Binary Definition Map |
| `CRAJ0.xdf` | `.XDF` | `215,714` bytes | TunerPro Binary Definition Map |
| `GUF1.xdf` | `.XDF` | `493,261` bytes | TunerPro Binary Definition Map |
| `GUFA.xdf` | `.XDF` | `494,970` bytes | TunerPro Binary Definition Map |
| `GUFB.xdf` | `.XDF` | `496,699` bytes | TunerPro Binary Definition Map |
| `HWAD3.xdf` | `.XDF` | `44,157` bytes | TunerPro Binary Definition Map |
| `IAW045_06.xdf` | `.XDF` | `39,613` bytes | TunerPro Binary Definition Map |
| `IAW045_L01.xdf` | `.XDF` | `40,046` bytes | TunerPro Binary Definition Map |
| `L8edited1.0.xdf` | `.XDF` | `74,788` bytes | TunerPro Binary Definition Map |
| `LUX0.xdf` | `.XDF` | `374,255` bytes | TunerPro Binary Definition Map |
| `N4AGB.xdf` | `.XDF` | `69,593` bytes | TunerPro Binary Definition Map |
| `NVMG8.xdf` | `.XDF` | `411,833` bytes | TunerPro Binary Definition Map |
| `P8_research_ver2.0.xdf` | `.XDF` | `137,044` bytes | TunerPro Binary Definition Map |
| `T23B.xdf` | `.XDF` | `221,443` bytes | TunerPro Binary Definition Map |

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
