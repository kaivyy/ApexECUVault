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

* **Rentang Tahun / Model Year**: 1998–2010

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `12AF_NGIC9A5.256k.bin` | **1998–2010** | 256.0 KB | `ba73856610803713c3cbe86a44377f3f` | Factory Binary Firmware Dump |
| `12BE_NGIC9B3.256k.bin` | **1998–2010** | 256.0 KB | `956675312536ba1600ac05e20670b51b` | Factory Binary Firmware Dump |
| `12CD_NGIC9CF.256k.bin` | **1998–2010** | 256.0 KB | `b8bf23db71a16b2a64e6d01106d05776` | Factory Binary Firmware Dump |
| `12FD_NGIC9F9.256k.bin` | **1998–2010** | 256.0 KB | `37208c17d320535180ea0ef615a55c5d` | Factory Binary Firmware Dump |
| `12UD-TurboEnhancedFuel.bin` | **1998–2010** | 256.0 KB | `1bf9b180d0bcd2f0752e540f4f636fe2` | Factory Binary Firmware Dump |
| `12UD_NGIC9UZ.256k.bin` | **1998–2010** | 256.0 KB | `51b1e4fe858d8498eed593e6c06fd00e` | Factory Binary Firmware Dump |
| `12VC_NGIC9V7.256k.bin` | **1998–2010** | 256.0 KB | `553c7b0d05f2ba6b6aa11535253525c6` | Factory Binary Firmware Dump |
| `12WD_NGIC9WG.256k.bin` | **1998–2010** | 256.0 KB | `5db014395b690fa7169543a21dea1cb7` | Factory Binary Firmware Dump |
| `12ZE_NGIC9Z4.256k.bin` | **1998–2010** | 256.0 KB | `9a92151df8cca7753f84fc34464999be` | Factory Binary Firmware Dump |
| `22AB_NGIC9AJ.256k.bin` | **1998–2010** | 256.0 KB | `2aac62b296caa3be655a5e341ed984c8` | Factory Binary Firmware Dump |
| `22VA_NGICA2Z.256k.bin` | **1998–2010** | 256.0 KB | `9ab4d9d4734b44ddba007d83d49a0f36` | Factory Binary Firmware Dump |
| `3DAC Extended Alpha.xdf` | **1998–2010** | 165.2 KB | `c4c81208e0f5f98e431cfb2962e540ed` | TunerPro Binary Definition Map |
| `3DAC PrePatched.bin` | **1998–2010** | 256.0 KB | `9e5825008f152376c896af659a69e940` | Factory Binary Firmware Dump |
| `HWAD3 Early Access 0.1.xdf` | **1998–2010** | 385.1 KB | `5dbe568c3dfc299e435e907f84f10c5d` | TunerPro Binary Definition Map |
| `N9XJ4 Extended v1.1.xdf` | **1998–2010** | 256.9 KB | `c5b464110a9589f4130d877a159c0d0b` | TunerPro Binary Definition Map |
| `N9XJ4 Extended.xdf` | **1998–2010** | 254.3 KB | `e6289cccf4476e4ac4269a6000278430` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.1.xdf` | **1998–2010** | 321.8 KB | `a86bfe65875fc6385aeaa7f3cde7747e` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.11.xdf` | **1998–2010** | 329.5 KB | `924c853ac12f47bd5496c927b62980ea` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.12.xdf` | **1998–2010** | 330.2 KB | `33f15c812bb6fbaaa8de8e23a4a95b38` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.2.xdf` | **1998–2010** | 478.6 KB | `b1c4001dccdc7092ead68af2e43b302d` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.21.xdf` | **1998–2010** | 548.5 KB | `a67ccbd487a25226935f2e9d3765d40c` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.3.xdf` | **1998–2010** | 1.06 MB | `64d05f2f70267cf8952cb69fad8bee59` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.31-b.xdf` | **1998–2010** | 1.06 MB | `00b13751c3e4ca5b3dce216098cf1346` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.32-b.xdf` | **1998–2010** | 1.06 MB | `280d9f62741d500a34679be209f8b35b` | TunerPro Binary Definition Map |
| `NGIC9 Extended.xdf` | **1998–2010** | 321.4 KB | `2db964227e8d6a87b63dd414c4411980` | TunerPro Binary Definition Map |
| `NGIC9 Generic.bin` | **1998–2010** | 256.0 KB | `ba73856610803713c3cbe86a44377f3f` | Factory Binary Firmware Dump |

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
