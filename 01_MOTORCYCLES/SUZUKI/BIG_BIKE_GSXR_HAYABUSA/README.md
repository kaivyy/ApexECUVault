# BIG_BIKE_GSXR_HAYABUSA - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/SUZUKI/BIG_BIKE_GSXR_HAYABUSA`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `41 files` (33 binary dumps, 8 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `BIG_BIKE_GSXR_HAYABUSA` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1999–2020

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `21H50_DJ0HSE01.bin` | **1999–2020** | 1.00 MB | `3f40fd1a860e1eda30ba8e03db4debb8` | Factory Binary Firmware Dump |
| `32990-10L1x - 5JCZSJ10.bin` | **1999–2020** | 2.00 MB | `309c55441c98c724e69c9d3e5ef5d454` | Factory Binary Firmware Dump |
| `32990-48L00.bin` | **1999–2020** | 2.00 MB | `aea03e67b829875ad9a7fbad7b7500c3` | Factory Binary Firmware Dump |
| `32990-48L00.xdf` | **1999–2020** | 3.64 MB | `dd2ddc0bf743bcf0d196331c243bfffd` | TunerPro Binary Definition Map |
| `32990-48L10-US.bin` | **1999–2020** | 2.00 MB | `339b43063d986d74602eb2e4f6bc1487` | Factory Binary Firmware Dump |
| `32990-48L10-US.xdf` | **1999–2020** | 3.65 MB | `58f9c7fc4e699eb3fdc929bdb0791af8` | TunerPro Binary Definition Map |
| `32990-48L20-EU.bin` | **1999–2020** | 2.00 MB | `c65a12f1022b1c5d11d5c671c2807b2e` | Factory Binary Firmware Dump |
| `32990-48L20-EU.xdf` | **1999–2020** | 3.65 MB | `cc07ba980ef236b1c11e771877fd1c05` | TunerPro Binary Definition Map |
| `32990-48L30.bin` | **1999–2020** | 2.00 MB | `375361112aeb25925a97664376463b8a` | Factory Binary Firmware Dump |
| `32990-48L30.xdf` | **1999–2020** | 3.64 MB | `79e172767c3743547d2eb6476e3f20a4` | TunerPro Binary Definition Map |
| `37H00_DJ55SE00.bin` | **1999–2020** | 1.00 MB | `d478341ed77c1863c7a70d96b7189b43` | Factory Binary Firmware Dump |
| `5JCUSJ40.ori` | **1999–2020** | 1.94 MB | `f21b4444d19efec466e6376be40b7369` | Factory Binary Firmware Dump |
| `5JCXSJ10.bin` | **1999–2020** | 2.00 MB | `04211f298f230c05bb8cc34e084fdb60` | Factory Binary Firmware Dump |
| `5JCZSJB0.bin` | **1999–2020** | 2.00 MB | `4092637db15b5f4bca4bf35fb7a3868a` | Factory Binary Firmware Dump |
| `5JCZSJB0.xdf` | **1999–2020** | 3.55 MB | `cd47ef7565fff5d796db887308582c00` | TunerPro Binary Definition Map |
| `5JCZSNC0.bin` | **1999–2020** | 2.00 MB | `73cac8994c0a3a222a866236a158fcac` | Factory Binary Firmware Dump |
| `5JCZSNC0.xdf` | **1999–2020** | 3.55 MB | `c944f9823e583f15c1cc94c0fd537867` | TunerPro Binary Definition Map |
| `Bking.bin` | **1999–2020** | 1.00 MB | `53a3793301d649effe82553af5324a9d` | Factory Binary Firmware Dump |
| `BkingUS.bin` | **1999–2020** | 1.00 MB | `5d1d6989da83b4a2857ca97fe1a9466b` | Factory Binary Firmware Dump |
| `DJ0HSE70.bin` | **1999–2020** | 1.00 MB | `b7a99d51ceca03dbaa94d5de93f67913` | Factory Binary Firmware Dump |
| `DJ47SE10.bin` | **1999–2020** | 1.00 MB | `c8b2690fb9b5c94a1cc9e5059a0864e3` | Factory Binary Firmware Dump |
| `DJ55SE10.bin` | **1999–2020** | 1.00 MB | `193c972a4ef6c2b56d2cf118084b2f60` | Factory Binary Firmware Dump |
| `DJE4SE01.bin` | **1999–2020** | 1.00 MB | `fb13700fc9469b9d1efc8d676615fb22` | Factory Binary Firmware Dump |
| `DJE4SE10.bin` | **1999–2020** | 1.00 MB | `14461fb30d5a953164c42ce5de77bd98` | Factory Binary Firmware Dump |
| `DJF4SE00.bin` | **1999–2020** | 1.00 MB | `0290db32aa30e62a8ff9ed32c5f7e3b7` | Factory Binary Firmware Dump |
| `DJF4SE10.bin` | **1999–2020** | 1.00 MB | `3206d24b86603d2e23964ee72db2eb18` | Factory Binary Firmware Dump |
| `G1BusaEUdefault.bin` | **1999–2020** | 256.0 KB | `232f3825793a9cc205df5b2ce494f898` | Factory Binary Firmware Dump |
| `G1BusaUSdefault.bin` | **1999–2020** | 256.0 KB | `8b4341eb858ce7cb205bfe9cd85a5720` | Factory Binary Firmware Dump |
| `GENERATIONAL_32920-10L00_Suzuki_GSX1300R_Hayabusa_Gen_3_2021_2026.xdf` | **2021–2026** | 2.5 KB | `fcd89f31f9ebd6e7d53695ae835d4cfa` | TunerPro Binary Definition Map |
| `GENERATIONAL_32920-15H00_Suzuki_GSX1300R_Hayabusa_Gen_2_2008_2020.xdf` | **2008–2020** | 2.5 KB | `0acf6ff2487d13d2e1df3645c83fa02d` | TunerPro Binary Definition Map |
| `Gixxer21H00.bin` | **1999–2020** | 1.00 MB | `91075fb798377ee821c4d0317d760afe` | Factory Binary Firmware Dump |
| `Gixxer21H10.bin` | **1999–2020** | 1.00 MB | `929a15247fe37f260c9f8ebb4dac7ef8` | Factory Binary Firmware Dump |
| `Gixxer21H70.bin` | **1999–2020** | 1.00 MB | `42e777d97e812716f6b144737400fcac` | Factory Binary Firmware Dump |
| `GixxerK7.bin` | **1999–2020** | 1.00 MB | `44ac5408d6c17624f803d500d8354bc1` | Factory Binary Firmware Dump |
| `GixxerK7EU.bin` | **1999–2020** | 1.00 MB | `56dee11858bc72d1ab07461fbe4c46ca` | Factory Binary Firmware Dump |
| `GixxerK8.bin` | **1999–2020** | 1.00 MB | `360fb679da4624b50476b14154de452d` | Factory Binary Firmware Dump |
| `Gixxerk9US.bin` | **1999–2020** | 1.00 MB | `9d56c12361fb5cdf0b1327a868e9a011` | Factory Binary Firmware Dump |
| `Hayabusa gen 3 stock.bin` | **1999–2020** | 2.00 MB | `04211f298f230c05bb8cc34e084fdb60` | Factory Binary Firmware Dump |
| `K8.bin` | **1999–2020** | 1.00 MB | `e339bebfefd7471a8fe51ef7ea215234` | Factory Binary Firmware Dump |
| `gixxerk9.bin` | **1999–2020** | 1.00 MB | `10ab07f34663e89cae00b3302bf1273e` | Factory Binary Firmware Dump |
| `suzuki hayabusa 32990-10L4.ori` | **1999–2020** | 1.94 MB | `f21b4444d19efec466e6376be40b7369` | Factory Binary Firmware Dump |

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
