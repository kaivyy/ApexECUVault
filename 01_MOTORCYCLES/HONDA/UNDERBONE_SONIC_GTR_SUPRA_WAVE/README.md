# HONDA UNDERBONE SONIC GTR SUPRA WAVE CUB - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/UNDERBONE_SONIC_GTR_SUPRA_WAVE`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `88 files` (11 binary/calibration dumps, 77 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `UNDERBONE_SONIC_GTR_SUPRA_WAVE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Underbone & Moped Fleet (Supra X 125, Wave 110i/125i, Revo FI, Blade, Dream, Super Cub, Sonic 150R, Supra GTR 150) Keihin/Shindengen ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `GENERATIONAL_38770-K56-N11_Honda_Supra_GTR_150___Winner_150_Gen_1_2016_2019.xdf` | `.XDF` | `2,553` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K56-V01_Honda_Supra_GTR_150_Facelift___Winner_X_Gen_2_2020_2025.xdf` | `.XDF` | `2,560` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K03-H01_Wave_110i_(2019-2020).xdf` | `.XDF` | `16,700` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K03-N32_Wave_110i_(2019-2020).xdf` | `.XDF` | `16,700` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K03-T61_Wave_110i_(2019-2020).xdf` | `.XDF` | `16,700` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K0G-962_Super_Cub_110_Pro.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K1M-T01_Wave_110i_AT.xdf` | `.XDF` | `16,691` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K2J-T01_Wave_110i___Super_Cub_(2021-2024).xdf` | `.XDF` | `16,712` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K2J-TH1_Wave_110i___Super_Cub_(2021-2024).xdf` | `.XDF` | `16,712` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K3F-T01_Wave_125i_(2023-2024).xdf` | `.XDF` | `16,700` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K41-N01_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K56-M01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K56-M91_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K56-N01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K56-N11_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K56-NJ1_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K56-V01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K56-V51_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K58-N41_Wave_110i___Wave_125i_(2020-2022).xdf` | `.XDF` | `16,712` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K58-T81_Wave_110i___Wave_125i_(2020-2022).xdf` | `.XDF` | `16,712` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K58-TC2_Wave_110i___Wave_125i_(2020-2022).xdf` | `.XDF` | `16,712` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K73-M41_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K73-M62_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K73-T32_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K73-T61_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K73-TC2_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K73-V42_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KWW-642_Wave_110i_(2009-2018).xdf` | `.XDF` | `16,700` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KWW-643_Wave_110i_(2009-2018).xdf` | `.XDF` | `16,700` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KYZ-713_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KYZ-T03_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KYZ-T41_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KYZ-V21_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KYZ-V71_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KZV-A61_Dream_Super_Cub_110_(2013-2017).xdf` | `.XDF` | `16,710` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-613_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-622_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-643_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-A21_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-A22_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-D01_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-D21_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-F21_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MEL-L22_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-622_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-644_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-671_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-691_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-702_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-741_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-761_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-773_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-861_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-871_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-A21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-D21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-F21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-J21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-J41_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MFL-L21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-A01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-A92_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-D01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-D62_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-F01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-F63_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-J01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-L01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MGP-T42_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKF-A22_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKF-D43_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKF-D72_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKF-H11_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKF-L13_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKFA-A22_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,712` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKFA-D72_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,712` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKFA-DK2_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,712` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_DREAM_SUPERCUB_38770_K1M_T01_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_SUPERCUB_38770_KZV_T03_48KB_ORI.bin` | `.BIN` | `49,152` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_SUPRA_X_125_38770_KYL_T01_56KB_ORI.bin` | `.BIN` | `57,344` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_SUPRA_X_125_38770_KYZ_T03_48KB_ORI.bin` | `.BIN` | `49,152` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_SUPRA_X_125_38770_KYZ_T41_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_SUPRA_X_125_HELMIN_38770_K73_T32_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_WAVE_REVO_110I_38770_K03_H01_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_WAVE_REVO_110I_38770_K03_T61_48KB_ORI.bin` | `.BIN` | `49,152` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_WAVE_REVO_110I_38770_K2J_T01_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_WAVE_REVO_110I_38770_K58_T81_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_WAVE_REVO_110I_38770_KWW_643_48KB_ORI.bin` | `.BIN` | `49,152` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
