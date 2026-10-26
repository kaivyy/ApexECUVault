# CLASSIC 4AGE 1UZ FE - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/CLASSIC_4AGE_1UZ_FE`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `36 files` (35 binary dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CLASSIC_4AGE_1UZ_FE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `GENERATIONAL_Toyota_4AGE_1UZFE_Denso_Classic.xdf` | `.XDF` | `2,965` bytes | TunerPro Binary Definition Map |
| `REMAP_STAGE1_Copy_of_cap.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_RAMtest.bin` | `.BIN` | `1,024` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_Superbootloader+1uzbootcopy.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_bigloaderF000.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_bigloaderfromtiny.bin` | `.BIN` | `1,024` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_cap.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_cap1-151801-0642.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_cap2-151801-2860.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_cap_D151802-0442.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_copytiny.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_reader.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_reader6301v1.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_replacement.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_test.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `REMAP_STAGE1_tinyloader.bin` | `.BIN` | `87` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Copy_of_cap.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_RAMtest.bin` | `.BIN` | `1,024` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Superbootloader+1uzbootcopy.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_bigloaderF000.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_bigloaderfromtiny.bin` | `.BIN` | `1,024` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_cap.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_cap1-151801-0642.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_cap2-151801-2860.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_cap4.bin` | `.BIN` | `4,199` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_cap_D151802-0442.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_cap_d151803-1320.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_cap_d151803-9260.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_cap_d151804-8081.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_copytiny.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_hacked9260.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_reader.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_reader6301v1.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_replacement.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_test.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_tinyloader.bin` | `.BIN` | `87` bytes | Binary Firmware / Calibration Dump |

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
