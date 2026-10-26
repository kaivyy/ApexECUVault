# JAZZ CITY MOBILIO BRV L15 - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/JAZZ_CITY_MOBILIO_BRV_L15`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `13 files` (0 binary dumps, 13 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `JAZZ_CITY_MOBILIO_BRV_L15` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `37805-RD1-X520_Honda_Fit_1.4_16v_SH7058_1Mb.xdf` | `.XDF` | `4,458` bytes | Honda Keihin Factory Calibration Package `37805-RD1-X520` |
| `37805-RME-A220_Honda_Fit_2008_Base__Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `168,318` bytes | Honda Keihin Factory Calibration Package `37805-RME-A220` |
| `37805-RME-A520_Honda_Fit_2007_Base__Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,343` bytes | Honda Keihin Factory Calibration Package `37805-RME-A520` |
| `37805-RME-A690_Honda_Fit_2007_Base_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,336` bytes | Honda Keihin Factory Calibration Package `37805-RME-A690` |
| `37805-RME-A720_Honda_Fit_2008_Base_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,336` bytes | Honda Keihin Factory Calibration Package `37805-RME-A720` |
| `37805-RME-A890_Honda_Fit_2007_Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,337` bytes | Honda Keihin Factory Calibration Package `37805-RME-A890` |
| `37805-RME-C220_Honda_Fit_2008_Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,337` bytes | Honda Keihin Factory Calibration Package `37805-RME-C220` |
| `37805-RP3-3060_Honda_Fit_2009_Base__Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `4,473` bytes | Honda Keihin Factory Calibration Package `37805-RP3-3060` |
| `37805-RP3-4050_Honda_Fit_2009_Base_1.5L__L4_-_Gas.xdf` | `.XDF` | `4,466` bytes | Honda Keihin Factory Calibration Package `37805-RP3-4050` |
| `37805-RP3-A170_Honda_Fit_2009_2010_Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `4,472` bytes | Honda Keihin Factory Calibration Package `37805-RP3-A170` |
| `37805-RP3-A770_Honda_Fit_2012_2013_Base__Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `4,478` bytes | Honda Keihin Factory Calibration Package `37805-RP3-A770` |
| `37805-RP6-A560_Honda_Fit_2012_2013_Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `7,804` bytes | Honda Keihin Factory Calibration Package `37805-RP6-A560` |
| `HONDA_37805-5A4-J81_JAZZ_GK5.xdf` | `.XDF` | `12,149` bytes | TunerPro Binary Definition Map |

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
