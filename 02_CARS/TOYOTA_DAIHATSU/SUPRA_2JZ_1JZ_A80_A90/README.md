# SUPRA 2JZ 1JZ A80 A90 - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/SUPRA_2JZ_1JZ_A80_A90`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `9 files` (0 binary dumps, 9 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SUPRA_2JZ_1JZ_A80_A90` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `GENERATIONAL_89661-14370_Toyota_Supra_MK3_JZA70_1JZ-GTE_TwinTurbo_1990_1993.xdf` | `.XDF` | `7,371` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-14480_Toyota_Supra_JZA80_2JZ-GTE_TwinTurbo_JDM_MT_1993_1997.xdf` | `.XDF` | `7,374` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-14560_Toyota_Supra_JZA80_2JZ-GTE_TwinTurbo_USDM_MT_550cc_1993_1998.xdf` | `.XDF` | `7,381` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-14830_Toyota_Supra_JZA80_2JZ-GTE_VVTi_6MT_1997_2002.xdf` | `.XDF` | `8,146` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-14840_Toyota_Supra_JZA80_2JZ-GTE_VVTi_AT_1997_2002.xdf` | `.XDF` | `8,145` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-22810_Toyota_Chaser_JZX100_1JZ-GTE_VVTi_MT_1996_2001.xdf` | `.XDF` | `7,757` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_B48B20_Toyota_GR_Supra_A90_2.0T_Bosch_MG1CS024_2020_2024.xdf` | `.XDF` | `8,929` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_B58B30O1_Toyota_GR_Supra_A90_3.0T_Facelift_MG1CS024_2021_2024.xdf` | `.XDF` | `8,934` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_B58B30_Toyota_GR_Supra_A90_3.0T_Bosch_MG1CS024_2019_2020.xdf` | `.XDF` | `8,929` bytes | TunerPro Binary Definition Map |

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
