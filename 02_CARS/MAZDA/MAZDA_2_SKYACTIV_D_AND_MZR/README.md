# MAZDA_2_SKYACTIV_D_AND_MZR - ECU Calibration Suite

**Repository Path**: `02_CARS/MAZDA/MAZDA_2_SKYACTIV_D_AND_MZR`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `11 files` (7 binary dumps, 4 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MAZDA_2_SKYACTIV_D_AND_MZR` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `MAZDA_2_GEN2_2010_1.3L_MZR_86HP_DENSO_ORIGINAL_READ.ori` | **2010** | 1.00 MB | `26395b013d94524dd9396a939e12065c` | Factory Binary Firmware Dump |
| `MAZDA_2_GEN2_2010_1.5L_MZR_DENSO_ORIGINAL_READ.ori` | **2010** | 1.00 MB | `26395b013d94524dd9396a939e12065c` | Factory Binary Firmware Dump |
| `MAZDA_2_GEN3_2015_1.5L_DIESEL_SKYACTIV_D_105HP_ORIGINAL_READ.ori` | **2015** | 4.00 MB | `a30ead7c8ab9b4df343bc98c739a47cd` | Factory Binary Firmware Dump |
| `Mazda-2015-2-1500-diesel-skyactiv-105HP-EGR_G.MOD` | **2015** | 4.00 MB | `f1ed5c7dcfa9fbbf400af876af501283` | ECU Calibration Asset |
| `Mazda-2015-2-1500-diesel-skyactiv-105HP_G.MOD` | **2015** | 4.00 MB | `86c8ba1dc419ccfdf009b30a56d62992` | ECU Calibration Asset |
| `Mazda-2015-2-1500-diesel-skyactiv-105HP_H_part.ori` | **2015** | 3.72 MB | `aad5a77f1e94858061c53f6ecd5bdef7` | Factory Binary Firmware Dump |
| `Mazda_2010_2_1300_MZR_86HP.ori` | **2010** | 1.00 MB | `26395b013d94524dd9396a939e12065c` | Factory Binary Firmware Dump |
| `Mazda_2015_2_1500_diesel_skyactiv_105HP_G.ori` | **2015** | 4.00 MB | `a30ead7c8ab9b4df343bc98c739a47cd` | Factory Binary Firmware Dump |
| `Mazda_2_sky_D_H_Quantum_Green_full.MOD` | **2000–2024** | 4.00 MB | `5f99176ae8dced08ad3f8738b3ed7087` | ECU Calibration Asset |
| `Mazda_2_sky_D_H_Quantum_Green_part.MOD` | **2000–2024** | 3.72 MB | `49b42e093e6fe862a1bd325159895e3b` | ECU Calibration Asset |
| `Mazda_2_sky_D_H_full.ori` | **2000–2024** | 4.00 MB | `d6baa6c4992c2de2d1d3c3e6858ccb7b` | Factory Binary Firmware Dump |

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
