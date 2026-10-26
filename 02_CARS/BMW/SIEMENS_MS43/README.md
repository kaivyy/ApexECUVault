# SIEMENS MS43 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/SIEMENS_MS43`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `17 files` (0 binary dumps, 17 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SIEMENS_MS43` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `MS43 ECU Definitions.xml` | `.XML` | `513,710` bytes | Siemens / Continental DME Calibration Data |
| `MS43 logger_METRIC_EN_v1.0.0 - ext load.xml` | `.XML` | `62,908` bytes | Siemens / Continental DME Calibration Data |
| `MS43 logger_METRIC_EN_v1.0.0.xml` | `.XML` | `64,814` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430037_ENG_512K_v1.16.xdf` | `.XDF` | `3,313,194` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430037_ENG_64K_v1.16.xdf` | `.XDF` | `3,313,188` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430055_ENG_512K_v1.16.xdf` | `.XDF` | `3,500,961` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430055_ENG_64K_v1.16.xdf` | `.XDF` | `3,500,955` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430056_ENG_512K_v1.16.xdf` | `.XDF` | `3,509,939` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430056_ENG_64K_v1.16.xdf` | `.XDF` | `3,509,933` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430064_ENG_512K_v1.16.xdf` | `.XDF` | `3,568,377` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430064_ENG_64K_v1.16.xdf` | `.XDF` | `3,568,371` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430066_ENG_512K_v1.16.xdf` | `.XDF` | `3,620,768` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430066_ENG_64K_v1.16.xdf` | `.XDF` | `3,620,762` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430069_ENG_512K_v1.16.xdf` | `.XDF` | `3,627,965` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430069_ENG_64K_v1.16.xdf` | `.XDF` | `3,627,959` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430069_ExtendedLoad_ENG_512K_v1.16.xdf` | `.XDF` | `3,627,837` bytes | Siemens / Continental DME Calibration Data |
| `Siemens_MS43_MS430069_ExtendedLoad_ENG_64K_v1.16.xdf` | `.XDF` | `3,627,823` bytes | Siemens / Continental DME Calibration Data |

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
