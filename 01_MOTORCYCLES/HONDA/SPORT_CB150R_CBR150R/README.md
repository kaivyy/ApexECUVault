# HONDA SPORT CB150R CBR150R - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/SPORT_CB150R_CBR150R`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `33 files` (7 binary/calibration dumps, 26 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SPORT_CB150R_CBR150R` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda 150cc DOHC 4-Valve Sport Fleet (CBR150R KPP/K45/K45N/K45R, CB150R Streetfire K15, CB150R ExMotion K94) Keihin ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `38770-KPP-602.bin` | `.BIN` | `57,344` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-KPP-N02.bin` | `.BIN` | `57,344` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-KPP-T03.bin` | `.BIN` | `57,344` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `GENERATIONAL_38770-K15-P01_Honda_All_New_CB150R_Streetfire_Gen_4_Inverted_Fork_(2021-2026).xdf` | `.XDF` | `5,585` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K3B-N01_Honda_CB150X_Adventure_Touring_(2021-2026).xdf` | `.XDF` | `5,572` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K45-G01_Honda_CBR150R_Gen_3_Facelift_LED_(2016-2018).xdf` | `.XDF` | `5,555` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K45-N01_Honda_CBR150R_Gen_2_Lokal_Dual_Eyes_(2014-2016).xdf` | `.XDF` | `5,547` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K45-N41_Honda_CBR150R_Gen_4_Facelift_ABS_&_Emergency_Stop_(2018-2020).xdf` | `.XDF` | `5,575` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K45-R01_Honda_All_New_CBR150R_Gen_5_Inverted_Fork_SFF-BP_(2021-2026).xdf` | `.XDF` | `5,599` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K0A-A01_CB300R_Neo_Sports_Cafe_(2018-2024).xdf` | `.XDF` | `16,713` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K0A-R11_CB300R_Neo_Sports_Cafe_(2018-2024).xdf` | `.XDF` | `16,713` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K15-601_CB150R_Streetfire.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K15-888_CB150R_Streetfire.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K15-903_CB150R_Streetfire.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K15-921_CB150R_Streetfire.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K18-902_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K18-941_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K18-961_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K33-D02_CBR300R___CB300F_(2014-2020).xdf` | `.XDF` | `16,715` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K33-D22_CBR300R___CB300F_(2014-2020).xdf` | `.XDF` | `16,715` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K33-N03_CBR300R___CB300F_(2014-2020).xdf` | `.XDF` | `16,715` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K45-N01_CBR150R_LED_(2016-2024).xdf` | `.XDF` | `16,702` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K45-N42_CBR150R_LED_(2016-2024).xdf` | `.XDF` | `16,702` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K45-NA1_CBR150R_LED_(2016-2024).xdf` | `.XDF` | `16,702` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K94-T02_CBR150R_(Indonesia).xdf` | `.XDF` | `16,698` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K98-E02_CB150R_Neo_Sports_Cafe_(2017-2024).xdf` | `.XDF` | `16,713` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KPP-602_CBR150R_(2011-2015).xdf` | `.XDF` | `16,694` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KPP-N02_CBR150R_(2011-2015).xdf` | `.XDF` | `16,694` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KPP-T03_CBR150R_(2011-2015).xdf` | `.XDF` | `16,694` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_CB150R_EXMOTION_K94_T02_96KB_ORI.bin` | `.BIN` | `98,304` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CBR150R_FACELIFT_2019_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CBR150R_K45_TA1_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CBR150R_KPP_T03_56KB_ORI.bin` | `.BIN` | `57,344` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
