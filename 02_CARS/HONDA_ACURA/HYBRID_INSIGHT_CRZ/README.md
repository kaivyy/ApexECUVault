# HYBRID INSIGHT CRZ - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/HYBRID_INSIGHT_CRZ`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `25 files` (0 binary dumps, 25 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `HYBRID_INSIGHT_CRZ` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `37805-PHM-4060_Honda_Insight_2002_2003_Base_1.0L__L3_-_Electric__Gas.xdf` | `.XDF` | `1,609` bytes | Honda Keihin Factory Calibration Package `37805-PHM-4060` |
| `37805-PHM-4070_Honda_Insight_2004_Base_1.0L__L3_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PHM-4070` |
| `37805-PHM-4080_Honda_Insight_2005_Base_1.0L__L3_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PHM-4080` |
| `37805-PHM-A530_Honda_Insight_2006_Base_1.0L__L3_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PHM-A530` |
| `37805-PLM-3150_Honda_Insight_2001_2002_2003_Base_1.0L__L3_-_Electric__Gas.xdf` | `.XDF` | `1,614` bytes | Honda Keihin Factory Calibration Package `37805-PLM-3150` |
| `37805-PZA-3060_Honda_Civic_2003_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-3060` |
| `37805-PZA-3270_Honda_Civic_2003_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-3270` |
| `37805-PZA-4070_Honda_Civic_2004_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-4070` |
| `37805-PZA-4250_Honda_Civic_2004_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-4250` |
| `37805-PZA-4290_Honda_Civic_2004_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-4290` |
| `37805-PZA-5250_Honda_Civic_2004_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-5250` |
| `37805-PZA-A660_Honda_Civic_2005_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-A660` |
| `37805-PZA-C660_Honda_Civic_2005_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-C660` |
| `37805-PZA-L640_Honda_Civic_2005_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZA-L640` |
| `37805-PZD-3050_Honda_Civic_2005_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `1,604` bytes | Honda Keihin Factory Calibration Package `37805-PZD-3050` |
| `37805-RBJ-4050_Honda_Insight_2010_EX_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `7,246` bytes | Honda Keihin Factory Calibration Package `37805-RBJ-4050` |
| `37805-RBJ-A430_Honda_Insight_2012_2013_2014_EX_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `7,256` bytes | Honda Keihin Factory Calibration Package `37805-RBJ-A430` |
| `37805-RBJ-L440_Honda_Insight_2012_2013_2014_EX_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `7,256` bytes | Honda Keihin Factory Calibration Package `37805-RBJ-L440` |
| `37805-RBJ-L560_Honda_Insight_1.3_16v_SH7058_1Mb.xdf` | `.XDF` | `7,230` bytes | Honda Keihin Factory Calibration Package `37805-RBJ-L560` |
| `37805-RD1-X020_Honda_Accord_2006_2007_Hybrid_3.0L__V6_-_Electric__Gas___ECU.xdf` | `.XDF` | `4,577` bytes | Honda Keihin Factory Calibration Package `37805-RD1-X020` |
| `37805-RMX-A630_Honda_Civic_2009_2010_2011_Hybrid__Hybrid-L_1.3L__L4_-_Elect.xdf` | `.XDF` | `2,781` bytes | Honda Keihin Factory Calibration Package `37805-RMX-A630` |
| `37805-RMX-X050_Honda_Civic_2006_Hybrid_1.3L__L4_-_Electric__Gas.xdf` | `.XDF` | `2,761` bytes | Honda Keihin Factory Calibration Package `37805-RMX-X050` |
| `37805-RTW-A050_Honda_CR-Z_2011_Base__EX_1.5L__L4_-_Electric__Gas.xdf` | `.XDF` | `169,494` bytes | Honda Keihin Factory Calibration Package `37805-RTW-A050` |
| `37805-RTW-A060_Honda_CR-Z_2012_Base__EX_1.5L_L4_-_Electric__Gas.xdf` | `.XDF` | `165,112` bytes | Honda Keihin Factory Calibration Package `37805-RTW-A060` |
| `37805-RTW-P020_Honda_CR-Z_2011_Base__EX_1.5L__L4_-_Electric__Gas.xdf` | `.XDF` | `3,921` bytes | Honda Keihin Factory Calibration Package `37805-RTW-P020` |

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
