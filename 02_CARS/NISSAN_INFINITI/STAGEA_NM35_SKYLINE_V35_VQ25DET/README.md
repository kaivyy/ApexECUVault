# NISSAN STAGEA NM35 & SKYLINE V35 - VQ25DET Hitachi / Unisia Jecs Suite

**Repository Path**: `02_CARS/NISSAN_INFINITI/STAGEA_NM35_SKYLINE_V35_VQ25DET`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `6 files` (6 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Koleksi 6 berkas biner kalibrasi asli pabrikan (512KB) dan tune stage bertingkat untuk Nissan Stagea NM35 AR-X FOUR dan Nissan Skyline V35 dengan mesin turbo VQ25DET 2.5L V6 Turbo Neo Di AWD (280 PS). Berbagi arsitektur ECU Hitachi/Unisia Jecs dengan Nissan Skyline GT-R R34, Stagea WGNC34, dan Infiniti FX35/G35.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Hitachi / Unisia Jecs 32-Bit Engine Control Unit`
- **Arsitektur MCU & Memori**: `Renesas SH7055 / SH7058 512KB Flash ROM`
- **Protokol Diagnostik & Flashing**: `Nissan Consult II / K-Line (ISO 14230 KWP2000) / Bench Bootmode`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`, `0110C6`, `MS430069`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`, `32920-xxxxx`): Nomor resmi Denso MCU firmware flash untuk mobil dan motor.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx-xxxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **VAG Hardware / Software IDs** (misal `038906012xx`, `03G906021xx`, `8D0907558xx`): Nomor bagian resmi Volkswagen Audi Group untuk identifikasi kalibrasi mesin EDC15, EDC16, dan ME7.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2001–2007

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `ecu.bin` | **2001–2007** | 512.0 KB | `7c6cf88facdac55e3ebbc70ad92208db` | Factory Binary Firmware Dump |
| `nm35_vq25det_STAGE1.bin` | **2001–2007** | 512.0 KB | `3099787cb3401a627529b1ffaa3827e5` | Factory Binary Firmware Dump |
| `nm35_vq25det_STAGE2.bin` | **2001–2007** | 512.0 KB | `3099787cb3401a627529b1ffaa3827e5` | Factory Binary Firmware Dump |
| `nm35_vq25det_STAGE3.bin` | **2001–2007** | 512.0 KB | `3099787cb3401a627529b1ffaa3827e5` | Factory Binary Firmware Dump |
| `nm35_vq35det_FACTORY.bin` | **2001–2007** | 512.0 KB | `7c6cf88facdac55e3ebbc70ad92208db` | Factory Binary Firmware Dump |
| `stockecu11.bin` | **2001–2007** | 512.0 KB | `7c6cf88facdac55e3ebbc70ad92208db` | Factory Binary Firmware Dump |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro / RomRaider yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, Smoke Limiter, Torque-to-Fuel Limiter, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance, Low/High Octane Timing, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow & Boost Management**: Peta Target Boost Pressure, Wastegate Duty Cycle (WGDC / N75 Map), MAF/MAP Scaling, dan Throttle Response Curves (Driver Wish).
- **Safety Limits & Thresholds**: Rev Limiter (Hard/Soft Cut), Top Speed Limiter (Vmax), Overboost Fuel Cut, EGT (Exhaust Gas Temperature) Protection, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
