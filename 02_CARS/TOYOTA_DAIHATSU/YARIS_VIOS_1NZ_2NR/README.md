# YARIS_VIOS_1NZ_2NR - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/YARIS_VIOS_1NZ_2NR`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `11 files` (10 binary dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `YARIS_VIOS_1NZ_2NR` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2002–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `89663-52823.bin` | **2002–2024** | 736.0 KB | `58eb8851d161037aecc21a423593e560` | Factory Binary Firmware Dump |
| `89663-52D30.bin` | **2002–2024** | 736.0 KB | `c32b1805eb056aa93989bbe2f9b83641` | Factory Binary Firmware Dump |
| `89663-52E91.bin` | **2002–2024** | 496.0 KB | `3ec27ed7072bdfe5d8af8444e6e20439` | Factory Binary Firmware Dump |
| `89663-52F01.bin` | **2002–2024** | 736.0 KB | `9f6ea82eefc59cdbf38a4fb4095af37e` | Factory Binary Firmware Dump |
| `89663-52F11.bin` | **2002–2024** | 736.0 KB | `63bd0bc11779249583fd41e5d336a15a` | Factory Binary Firmware Dump |
| `TOYOTA_89663-52xxx_VIOS.xdf` | **2002–2024** | 9.8 KB | `9b770c086209f131f29661b69aa6890b` | TunerPro Binary Definition Map |
| `TOYOTA_VIOS_YARIS_GEN2_2008_1.5L_1NZFE_MANUAL_89663-52E91.bin` | **2008** | 496.0 KB | `3ec27ed7072bdfe5d8af8444e6e20439` | Factory Binary Firmware Dump |
| `TOYOTA_VIOS_YARIS_GEN2_2009_1.5L_1NZFE_AUTO_89663-52F01.bin` | **2009** | 736.0 KB | `9f6ea82eefc59cdbf38a4fb4095af37e` | Factory Binary Firmware Dump |
| `TOYOTA_VIOS_YARIS_GEN2_2010_1.5L_1NZFE_AUTO_89663-52F11.bin` | **2010** | 736.0 KB | `63bd0bc11779249583fd41e5d336a15a` | Factory Binary Firmware Dump |
| `TOYOTA_VIOS_YARIS_GEN3_2014_1.5L_1NZFE_AUTO_89663-52D30.bin` | **2014** | 736.0 KB | `c32b1805eb056aa93989bbe2f9b83641` | Factory Binary Firmware Dump |
| `TOYOTA_YARIS_VIOS_1.3L_2SZFE_89663-52823.bin` | **2002–2024** | 736.0 KB | `58eb8851d161037aecc21a423593e560` | Factory Binary Firmware Dump |

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
