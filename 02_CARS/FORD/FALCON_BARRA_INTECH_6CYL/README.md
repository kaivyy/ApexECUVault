# FALCON BARRA INTECH 6CYL - ECU Calibration Suite

**Repository Path**: `02_CARS/FORD/FALCON_BARRA_INTECH_6CYL`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `26 files` (13 binary dumps, 13 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `FALCON_BARRA_INTECH_6CYL` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `12AF_NGIC9A5.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `12BE_NGIC9B3.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `12CD_NGIC9CF.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `12FD_NGIC9F9.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `12UD-TurboEnhancedFuel.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `12UD_NGIC9UZ.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `12VC_NGIC9V7.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `12WD_NGIC9WG.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `12ZE_NGIC9Z4.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `22AB_NGIC9AJ.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `22VA_NGICA2Z.256k.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `3DAC Extended Alpha.xdf` | `.XDF` | `169,147` bytes | TunerPro Binary Definition Map |
| `3DAC PrePatched.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |
| `HWAD3 Early Access 0.1.xdf` | `.XDF` | `394,362` bytes | TunerPro Binary Definition Map |
| `N9XJ4 Extended v1.1.xdf` | `.XDF` | `263,102` bytes | TunerPro Binary Definition Map |
| `N9XJ4 Extended.xdf` | `.XDF` | `260,410` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.1.xdf` | `.XDF` | `329,472` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.11.xdf` | `.XDF` | `337,436` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.12.xdf` | `.XDF` | `338,115` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.2.xdf` | `.XDF` | `490,076` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.21.xdf` | `.XDF` | `561,688` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.3.xdf` | `.XDF` | `1,110,453` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.31-b.xdf` | `.XDF` | `1,111,829` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.32-b.xdf` | `.XDF` | `1,111,890` bytes | TunerPro Binary Definition Map |
| `NGIC9 Extended.xdf` | `.XDF` | `329,077` bytes | TunerPro Binary Definition Map |
| `NGIC9 Generic.bin` | `.BIN` | `262,144` bytes | Binary Firmware / Calibration Dump |

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
