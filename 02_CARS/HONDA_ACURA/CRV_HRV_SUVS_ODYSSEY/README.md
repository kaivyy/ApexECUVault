# CRV_HRV_SUVS_ODYSSEY - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CRV_HRV_SUVS_ODYSSEY`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `47 files` (1 binary dumps, 46 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CRV_HRV_SUVS_ODYSSEY` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2007–2023

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `37805-5PA-9630_Honda_CR-V_2020_EX__EX-L__Touring_1.5L_L4_-_Gas.xdf` | **2020** | 119.8 KB | `a0f98017c7437799fbcccb4d1496062d` | TunerPro Binary Definition Map |
| `37805-5PA-9640_Honda_CR-V_2020_EX__EX-L__Touring_1.5L_L4_-_Gas.xdf` | **2020** | 120.4 KB | `1be59576f69548c80fb43cb41a25e8b6` | TunerPro Binary Definition Map |
| `37805-PPA-3060_Honda_CR-V_2002_2003_EX__LX_2.4L__L4_-_Gas.xdf` | **2002–2003** | 1.6 KB | `ccca414f0fe2f33827899ef868736699` | TunerPro Binary Definition Map |
| `37805-PPA-3070_Honda_CR-V_2002_2003_EX__LX_2.4L__L4_-_Gas.xdf` | **2002–2003** | 1.6 KB | `6a865246054a8c1034431376ff4520f5` | TunerPro Binary Definition Map |
| `37805-PPA-4080_Honda_CR-V_2006_EX_2.4L__L4_-_Gas.xdf` | **2006** | 1.6 KB | `88ac9b7b4aa82582888288cf5c35d746` | TunerPro Binary Definition Map |
| `37805-PPA-4090_Honda_CR-V_2006_EX__LX__SE_2.4L__L4_-_Gas.xdf` | **2006** | 1.6 KB | `84e8d81652e57dbe408cbd2a584b300f` | TunerPro Binary Definition Map |
| `37805-PPA-4270_Honda_CR-V_2005_EX__LX__SE_2.4L__L4_-_Gas.xdf` | **2005** | 1.6 KB | `c0f51dfc5be2a542efca273b8bdda896` | TunerPro Binary Definition Map |
| `37805-PPA-4350_Honda_CR-V_2005_LX_2.4L__L4_-_Gas.xdf` | **2005** | 1.6 KB | `0463893f839d5ba08c3e3352677beefc` | TunerPro Binary Definition Map |
| `37805-PPA-K120_Honda_CR-V_2005_2006_EX_2.4L__L4_-_Gas.xdf` | **2005–2006** | 1.6 KB | `57c36f84c676042feec11064f151eb19` | TunerPro Binary Definition Map |
| `37805-PVJ-3060_Honda_Pilot_2005_EX__LX_3.5L__V6_-_Gas.xdf` | **2005** | 1.6 KB | `5ad76afb401b8285c224a79d90eba88d` | TunerPro Binary Definition Map |
| `37805-PVJ-A820_Honda_Pilot_2005_EX-L_3.5L__V6_-_Gas.xdf` | **2005** | 1.6 KB | `2c3008fe7b4e0dab96523fe17f75d518` | TunerPro Binary Definition Map |
| `37805-PVJ-X530_Honda_Pilot_2006_2007_EX__EX-L__LX_3.5L__V6_-_Gas.xdf` | **2006–2007** | 1.6 KB | `652e3655456aebcc9b605ef7723a52d3` | TunerPro Binary Definition Map |
| `37805-PZD-3060_Honda_Element_2003_2004_DX__EX__LX_DX__EX_2.4L__L4_-_Gas.xdf` | **2003–2004** | 1.6 KB | `ec04ea172c2d3f3cce49ef5a6ec01999` | TunerPro Binary Definition Map |
| `37805-PZD-3070_Honda_Element_2003_2004_DX__EX__LX_DX__EX_2.4L__L4_-_Gas.xdf` | **2003–2004** | 1.6 KB | `89dc81ed10fd1e560d1a89c212a26374` | TunerPro Binary Definition Map |
| `37805-PZD-3090_Honda_Element_2003_2004_DX__EX__LX_DX__EX_2.4L__L4_-_Gas.xdf` | **2003–2004** | 9.9 KB | `62dccee3ca6490f94d290b3d5fbedd2b` | TunerPro Binary Definition Map |
| `37805-PZD-4050_Honda_Element_2007_2008_EX__LX__SC_2.4L__L4_-_Gas.xdf` | **2007–2008** | 9.9 KB | `5113e1f4c1c7567e41210a4e989a4b49` | TunerPro Binary Definition Map |
| `37805-PZD-4170_Honda_Element_2007_2008_EX__LX__SC_2.4L__L4_-_Gas.xdf` | **2007–2008** | 9.9 KB | `3cfce1ea4cb4a57c60bf3f8f7a333bf4` | TunerPro Binary Definition Map |
| `37805-PZD-A480_Honda_Element_2010_2011_EX__LX_EX__LX__SC_2.4L__L4_-_Gas.xdf` | **2010–2011** | 9.9 KB | `1d5b96f37a5d4b20dbbf6356fb636332` | TunerPro Binary Definition Map |
| `37805-PZD-A590_Honda_Element_2010_2011_EX__LX_2.4L__L4_-_Gas.xdf` | **2010–2011** | 9.9 KB | `267e14651b7f6e4fb422721f5c4e401e` | TunerPro Binary Definition Map |
| `37805-PZD-A690_Honda_Element_2006_EX__LX_2.4L__L4_-_Gas.xdf` | **2006** | 9.8 KB | `f8f217c9e1b201065a9f8c89a8c83096` | TunerPro Binary Definition Map |
| `37805-PZD-A720_Honda_Element_2006_EX__LX_2.4L__L4_-_Gas.xdf` | **2006** | 9.8 KB | `eedb85d257b319b5a1a0d9961a4d21d9` | TunerPro Binary Definition Map |
| `37805-PZD-A820_Honda_Element_2005_EX__LX_2.4L__L4_-_Gas.xdf` | **2005** | 9.8 KB | `a226aa217b90b35d553c642c48849e2c` | TunerPro Binary Definition Map |
| `37805-REX-X540_Honda_CR-V_2.4_16v_SH7058_1Mb.xdf` | **2007–2023** | 4.9 KB | `1ca675ce0d4981ea5be7c96d3050fce5` | TunerPro Binary Definition Map |
| `37805-REZ-A570_Honda_CR-V_2.4_16v_SH7058_1Mb.xdf` | **2007–2023** | 4.9 KB | `9374033d9995421c00d9fd8c40bd6286` | TunerPro Binary Definition Map |
| `37805-RGL-A020_Honda_CR-V_2011_EX__EX-L__LX__SE_2.4L__L4_-_Gas.xdf` | **2011** | 8.2 KB | `12c55fcde73f40ee25f82c18b050f73b` | TunerPro Binary Definition Map |
| `37805-RGL-A570_Honda_Odyssey_2009_2010_EX__LX_3.5L__V6_-_Gas.xdf` | **2009–2010** | 8.2 KB | `206f507a1984351ec855e1c497878e78` | TunerPro Binary Definition Map |
| `37805-RGL-A730_Honda_Odyssey_2005_EX__LX_3.5L__V6_-_Gas.xdf` | **2005** | 8.2 KB | `e3dc59ea8d1c49a87ccfa80b028b7da8` | TunerPro Binary Definition Map |
| `37805-RGL-A840_Honda_Odyssey_2006_EX__LX_3.5L__V6_-_Gas.xdf` | **2006** | 7.6 KB | `a0de0c239065c85bcb6a49df453976ae` | TunerPro Binary Definition Map |
| `37805-RGL-A930_Honda_Odyssey_2007_EX__LX_3.5L__V6_-_Gas___ECU_Honda_Odyssey.xdf` | **2007** | 8.3 KB | `ba0e9c4cd996065441d6fef863ef3311` | TunerPro Binary Definition Map |
| `37805-RGL-K720_Honda_Odyssey_2008_EX__LX_3.5L__V6_-_Gas.xdf` | **2008** | 8.2 KB | `e5cbe3679182af99000889c0a59061a9` | TunerPro Binary Definition Map |
| `37805-RGM-A750_Honda_Odyssey_2005_EX-L__Touring_3.5L__V6_-_Gas.xdf` | **2005** | 7.6 KB | `e1e95b16c326cfcb56cf743b4b08dce7` | TunerPro Binary Definition Map |
| `37805-RGM-A840_Honda_Odyssey_2006_EX-L__Touring_3.5L__V6_-_Gas.xdf` | **2006** | 7.6 KB | `31a0c5f9946dc2957fcdc79c44e58379` | TunerPro Binary Definition Map |
| `37805-RGW-A060_Honda_Odyssey_2007_EX-L__Touring_3.5L__V6_-_Gas___ECU_Honda_.xdf` | **2007** | 7.8 KB | `aef355196efd5880d80462cf95fea4c3` | TunerPro Binary Definition Map |
| `37805-RGW-A960_Honda_Odyssey_2009_2010_EX-L__Touring_3.5L__V6_-_Gas___ECU_H.xdf` | **2009–2010** | 7.8 KB | `9662203d89d695498ccd2885273970cc` | TunerPro Binary Definition Map |
| `37805-RJA-A630_Honda_Odyssey_2008_EX-L__Touring_3.5L__V6_-_Gas.xdf` | **2008** | 7.6 KB | `08cbf4afcb3f8cf6e22c4aed50fbdc3e` | TunerPro Binary Definition Map |
| `37805-RJE-K720_Honda_RIDGELINE_3.5_V6_SH7058_1Mb.xdf` | **2007–2023** | 7.6 KB | `17ece29a9445a6de2a07dc20fb9c6117` | TunerPro Binary Definition Map |
| `37805-RME-A180_Honda_Pilot_2016_EX__EX-L_3.5L__V6_-_Gas.xdf` | **2016** | 78.5 KB | `ad6515f6299db2e1e4c6cd72893b385e` | TunerPro Binary Definition Map |
| `37805-RN0-A630_Honda_Pilot_2009_2010_EX__EX-L__LX__Touring_3.5L__V6_-_Gas.xdf` | **2009–2010** | 7.6 KB | `f91bc0f8ae22d3497a859d3ce16c9d49` | TunerPro Binary Definition Map |
| `37805-RN0-A770_Honda_Pilot_2011_EX__EX-L__LX__Touring_3.5L__V6_-_Gas___ECU_.xdf` | **2011** | 7.8 KB | `36f6a2adbdf6e40cb1da950c61905b76` | TunerPro Binary Definition Map |
| `37805-RN0-A830_Honda_Pilot_2009_2010_EX__EX-L__LX__Touring_3.5L__V6_-_Gas__.xdf` | **2009–2010** | 7.7 KB | `7cb24ce6a59ab344418a523c3ac09279` | TunerPro Binary Definition Map |
| `37805-RN0-A970_Honda_Pilot_2011_EX__EX-L__LX__Touring_3.5L__V6_-_Gas.xdf` | **2011** | 7.1 KB | `d68d20dca559641f785fa6482b118396` | TunerPro Binary Definition Map |
| `37805-RV0-A650_Honda_Odyssey_2011_2013_EX__EX-L__LX_3.5L__V6_-_Gas___ECU_Ho.xdf` | **2011–2013** | 7.2 KB | `0acb8147c95fa7c9afdfd67e7e442d57` | TunerPro Binary Definition Map |
| `37805-RV0-A780_Honda_Odyssey_2014_2015_2016_EX__EX-L__LX__SE__Touring__Tour.xdf` | **2014–2015** | 7.2 KB | `f8a3f621879cd4b4871d600d5874226c` | TunerPro Binary Definition Map |
| `37805-RV0-X580_Honda_Odyssey_2011_2013_Touring__Touring_Elite_3.5L__V6_-_Ga.xdf` | **2011–2013** | 7.1 KB | `2e7f1c3a023ceec8aece30ba9fb32776` | TunerPro Binary Definition Map |
| `37805-RZA-A570_Honda_CR-V_2.0_16v_SH7058_1Mb.xdf` | **2007–2023** | 3.8 KB | `ad85a6c7142cce94e0f74a5a74358ff4` | TunerPro Binary Definition Map |
| `37805-RZA-A770_Honda_CR-V_2007_2008_2009_EX__EX-L__LX_2.4L__L4_-_Gas.xdf` | **2007–2008** | 3.8 KB | `147394d80e37cf4f9c38dbb9bfa14fdb` | TunerPro Binary Definition Map |
| `HONDA_CRV_RM_2012-2016_2.4L_K24Z_KEIHIN_37805-R5A-U140-M1.rwd` | **2012–2016** | 2.94 MB | `da1dd3f098a23e40711b1a85e222646f` | Factory Binary Firmware Dump |

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
