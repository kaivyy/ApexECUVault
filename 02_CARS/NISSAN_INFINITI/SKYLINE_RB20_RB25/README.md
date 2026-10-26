# SKYLINE RB20 RB25 - ECU Calibration Suite

**Repository Path**: `02_CARS/NISSAN_INFINITI/SKYLINE_RB20_RB25`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `64 files` (64 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SKYLINE_RB20_RB25` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `ECR33_RB25DET_13U00_MT_MEC-R720.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DET_13U01_MT_MEC-R260.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DET_21U00_MT_MECR520.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DET_21U02_MT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DET_21U03.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DET_21U11_AT_MECR531.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DET_21U60_MT_MECR530.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DET_21U70.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DE_17U14_AT_MECR514.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ECR33_RB25DE_28U00_MT_MEC-R700.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA500_MT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA501_MT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA502_MT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA510_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA511_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA512_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA513_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA560_MT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `ER34_RB25DET_AA570_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_04U00_MT_MEC-R106.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_04U02_MT_MEC-R132.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_04U11_AT_MECR109.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_04U12_AT_MECR127.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_04U60_MT_GTS4.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_04U70_AT_GTS4_MEC-R117.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_10U01_MEC-R210B.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_10U11_MEC-217.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_11U00_MT_MEC-212B.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_11U01.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_11U10_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_11U60_MT_MEC-214B.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `HCR32_RB20DET_11U70_MT_MEC-215B.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_13U00_MT_MEC-R720.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_13U01_MT_MEC-R260.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U00_MT_MECR520.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U02_MT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U03.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U11_AT_MECR531.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U60_MT_MECR530.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U70.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DE_17U14_AT_MECR514.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ECR33_RB25DE_28U00_MT_MEC-R700.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA500_MT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA501_MT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA502_MT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA510_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA511_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA512_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA513_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA560_MT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA570_AT.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U00_MT_MEC-R106.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U02_MT_MEC-R132.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U11_AT_MECR109.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U12_AT_MECR127.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U60_MT_GTS4.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U70_AT_GTS4_MEC-R117.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_10U01_MEC-R210B.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_10U11_MEC-217.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U00_MT_MEC-212B.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U01.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U10_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U60_MT_MEC-214B.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U70_MT_MEC-215B.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |

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
