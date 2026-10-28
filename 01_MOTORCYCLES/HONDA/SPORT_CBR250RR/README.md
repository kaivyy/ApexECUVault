# SPORT_CBR250RR - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/SPORT_CBR250RR`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `20 files` (8 binary dumps, 12 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SPORT_CBR250RR` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2016–2026

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `38770-K64-N01.bin` | **2016–2026** | 1.00 MB | `e0c12d43c50c7c285df0307bef13f4b5` | Factory Binary Firmware Dump |
| `38770-K64-R02.bin` | **2016–2026** | 1.00 MB | `f87f1dc65059e08f496e62fd0872a6e7` | Factory Binary Firmware Dump |
| `CBR250RR-38770-K64-N04_BIN.bin` | **2016–2026** | 1.00 MB | `c069d5b2d1476a728ba14a43ef73dc7a` | Factory Binary Firmware Dump |
| `CBR250RR-38770-K64-ND1_BIN.bin` | **2016–2026** | 1.00 MB | `5c616504f3b6306adff2ad04a17ab68c` | Factory Binary Firmware Dump |
| `CBR250RR_38770-K64-N04_PUBLIC_v1.xdf` | **2016–2026** | 89.0 KB | `8beae407f19171868ea92c8f56748426` | TunerPro Binary Definition Map |
| `CBR250RR_38770-K64-ND1_PUBLIC_v1.xdf` | **2016–2026** | 83.3 KB | `cb0b660f54754f38efbc1ad750aa4967` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-N04_Honda_CBR250RR_Gen_1_(2016-2019)_Standard_&_ABS.xdf` | **2016–2019** | 9.5 KB | `04be9df5087b128d0865bc6c1a2eed22` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-NB1_Honda_CBR250RR_Gen_2_SP_(2020-2022)_Non-QS.xdf` | **2020–2022** | 9.5 KB | `ca5015c2f8f9aa7988be8bddc0d6aef1` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-ND1_Honda_CBR250RR_Gen_2_SP_(2020-2022)_Quick_Shifter.xdf` | **2020–2022** | 9.5 KB | `5ba7c328b2c7b46ec1d84af75557376c` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-NL1_Honda_New_CBR250RR_Gen_3_Facelift_(2023-2026)_Standard_38.7PS.xdf` | **2023–2026** | 9.5 KB | `544c171ffadc975b54ae241d3b0fe591` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-NM1_Honda_New_CBR250RR_Gen_3_Facelift_(2023-2026)_SP_Quick_Shifter_42PS.xdf` | **2023–2026** | 9.6 KB | `c287ba68bf9a068f8938d73bc7272d74` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-R02_Honda_CBR250RR_HRC_Racing_ECU_(2017-2024).xdf` | **2017–2024** | 9.5 KB | `0afbe5a886e9729dd423085f000c4bc7` | TunerPro Binary Definition Map |
| `HONDA_38770-K64-J01_Honda_Generic_ECM.xdf` | **2016–2026** | 16.3 KB | `6b23d0eae7e35613a845574759ba1d33` | TunerPro Binary Definition Map |
| `HONDA_38770-K64-N01_Honda_Generic_ECM.xdf` | **2016–2026** | 16.3 KB | `e17d45e5d6ddac57dee1b4c57f7bf34f` | TunerPro Binary Definition Map |
| `HONDA_38770-K64-N04_Honda_Generic_ECM.xdf` | **2016–2026** | 16.3 KB | `cae354c06883e17cb0afd70bd3b4abcc` | TunerPro Binary Definition Map |
| `HONDA_38770-K64-NB1_Honda_Generic_ECM.xdf` | **2016–2026** | 16.3 KB | `beb0798ad823769667fb5235ffd8f790` | TunerPro Binary Definition Map |
| `STOCK_ORIGINAL_38770-K64-N01_Honda_CBR250RR_Gen1_(2016-2019)_Thai.bin` | **2016–2019** | 1.00 MB | `e0c12d43c50c7c285df0307bef13f4b5` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_38770-K64-N04_Honda_CBR250RR_Gen1_(2016-2019)_Indo.bin` | **2016–2019** | 1.00 MB | `c069d5b2d1476a728ba14a43ef73dc7a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_38770-K64-ND1_Honda_CBR250RR_Gen2_SP_(2020-2022)_QS_Indo.bin` | **2020–2022** | 1.00 MB | `5c616504f3b6306adff2ad04a17ab68c` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_38770-K64-R02_Honda_CBR250RR_HRC_Race_ECU_(2017-2024).bin` | **2017–2024** | 1.00 MB | `f87f1dc65059e08f496e62fd0872a6e7` | Factory Binary Firmware Dump |

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
