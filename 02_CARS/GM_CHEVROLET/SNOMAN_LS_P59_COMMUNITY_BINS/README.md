# SNOMAN LS P59 COMMUNITY BINS - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/SNOMAN_LS_P59_COMMUNITY_BINS`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `18 files` (18 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SNOMAN_LS_P59_COMMUNITY_BINS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: OEM Production

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `04 Chevy 1500 4x2 LM7 12606960.bin` | **2004** | 1.00 MB | `9b0d3cfba355dc0fda0be12cb19af61b` | Factory Binary Firmware Dump |
| `04_hummer_lq4.bin` | **2004** | 1.00 MB | `e1c4e30c4c941a65f58a64d6e1a77d55` | Factory Binary Firmware Dump |
| `1997 5.7L LT1 Camaro BTZB M6 Manual.bin` | **1997** | 512.0 KB | `5f5219e67d567ccee3649bc86eae7a54` | Factory Binary Firmware Dump |
| `2004 4.3L LU3 Manual Full Size Truck 4x2 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `b0679a169f0b7cf19856620f3c70d632` | Factory Binary Firmware Dump |
| `2004 4.8L LR4 DBC 4L80E Express Van 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `eda61905771f7f65501fe28595c9982f` | Factory Binary Firmware Dump |
| `2004 4.8L LR4 DBW Manual NV3500 4x4 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `18d80bb8f2f1d122be816512e022fccd` | Factory Binary Firmware Dump |
| `2004 5.3L L59 DBW 4L60E 4x4 Flex Fuel 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `63324d558a2f79d814c7ed2d51a31f56` | Factory Binary Firmware Dump |
| `2004 5.3L LM4 GMC Envoy 4x4 12587603 OS Stock.bin` | **2004** | 1.00 MB | `bd9e17fb61c9875bef0fa4da507d71dc` | Factory Binary Firmware Dump |
| `2004 6.0L LQ4 DBC 4L80E Express Van 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `5ee37365a85e04e5e40ba9aab9bd781c` | Factory Binary Firmware Dump |
| `2004 6.0L LQ4 DBW 4L65E 4x4 Yukon 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `35bc3d13bda2cb9cbde6865b6b57843b` | Factory Binary Firmware Dump |
| `2004 6.0L LQ4 DBW 4L80E 4x4 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `88240bba0a02fa90ec0ee231bb618309` | Factory Binary Firmware Dump |
| `2004 6.0L LQ4 DBW Manual NV4500 4x4 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `e6da1d152e19c9ba9bf70f1c4d3c823a` | Factory Binary Firmware Dump |
| `2004 6.0L LQ9 DBW 4L65E AWD Silverado SS 12587603 OS STOCK.bin` | **2004** | 1.00 MB | `17c7bbd9aedfaece1fbcb5727e4e543f` | Factory Binary Firmware Dump |
| `2004 Blazer 4.3L (12587603).bin` | **2004** | 1.00 MB | `f2597cf945592660e8186d4d21b59d1e` | Factory Binary Firmware Dump |
| `2004-4.8L-LR4-DBC-4L80E-Express-Van-12587603-OS-STOCK.bin` | **2004** | 1.00 MB | `eda61905771f7f65501fe28595c9982f` | Factory Binary Firmware Dump |
| `Escalade 2004 LQ9 6.0_4L60E.bin` | **2004** | 1.00 MB | `55048d16aff6a212c517def0e14c4f61` | Factory Binary Firmware Dump |
| `LS1A-1998-Fbody.bin` | **1998** | 512.0 KB | `e6c1a52f75f162cbc645f33447131483` | Factory Binary Firmware Dump |
| `Stock_2004_GMC_Sierra_1500_4x4_Lm7_4l60e_truck_copy.bin` | **2004** | 1.00 MB | `3f38992de7441771607c1f614e9e6c3b` | Factory Binary Firmware Dump |

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
