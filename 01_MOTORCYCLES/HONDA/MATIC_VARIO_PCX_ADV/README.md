# HONDA MATIC VARIO PCX ADV CLICK - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/MATIC_VARIO_PCX_ADV`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `36 files` (3 binary/calibration dumps, 33 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MATIC_VARIO_PCX_ADV` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda 110cc - 750cc Automatic & Crossover Fleet (Click 110, Vario 125/150/160, PCX, ADV 150/160, X-ADV 750) Keihin ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `GENERATIONAL_38770-K0W-NA1_Honda_All_New_ADV_160_eSP+_2022_2025.xdf` | `.XDF` | `2,539` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K1ZG-N21_Honda_All_New_PCX_160_eSP+_Gen_4_2021_2025.xdf` | `.XDF` | `2,546` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K2SA-N01_Honda_All_New_Vario_160___Click_160_2022_2025.xdf` | `.XDF` | `2,549` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K59-A11_Honda_Vario_150_Gen_1_LED_eSP_(2015-2017).xdf` | `.XDF` | `5,563` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K59-A71_Honda_All_New_Vario_150_Gen_2_Keyless_(2018-2022).xdf` | `.XDF` | `5,573` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K60-B01_Honda_Vario_125_Gen_2_LED_eSP_(2015-2017).xdf` | `.XDF` | `5,567` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K60-B61_Honda_All_New_Vario_125_Gen_3_(2018-2022).xdf` | `.XDF` | `5,563` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-KZR-601_Honda_Vario_125_Gen_1_Bohlam___Helm-in_(2012-2014).xdf` | `.XDF` | `5,572` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K0WF-T01_ADV150_2017-2019_ADV_150___ADV_160_(2019-2024).xdf` | `.XDF` | `10,181` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K0WF-T01_ADV150_ADV_150___ADV_160_(2019-2024).xdf` | `.XDF` | `10,171` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K0WM-TA1_ADV160_ADV_150___ADV_160_(2019-2024).xdf` | `.XDF` | `10,171` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K1ZF-T01_PCX160_NOABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | `.XDF` | `10,179` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K1ZF-T11_PCX160ABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | `.XDF` | `10,176` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K1ZP-T51_PCX160_NOABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | `.XDF` | `10,179` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K1ZP-T71_PCX160_ABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | `.XDF` | `10,177` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K2VH-T11_CLICK125_2023_Click_125i_(2023-2024).xdf` | `.XDF` | `10,171` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K36F-T01_PCX150_2014-2015_PCX_150_(2014-2017).xdf` | `.XDF` | `10,171` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K36S-T31__PCX150_2016-2017_PCX_150_(2014-2017).xdf` | `.XDF` | `10,172` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K46-N21_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K46-N31_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K46-NA1_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K59K-T11_Click150_2018-2020_Click_150i_(2018-2022).xdf` | `.XDF` | `10,176` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K60F-T01_Click125_2014-2015_Click_125i_LED_(2018-2022).xdf` | `.XDF` | `10,180` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K60S-T71_Click125_2016-2017_Click_125i_LED_(2018-2022).xdf` | `.XDF` | `10,180` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_30400-K97F-T_PCX150_2017-2019_PCX_150_Smart_Key_(2018-2020).xdf` | `.XDF` | `10,181` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K46-N01_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KVG-V42_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKH-C02_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKH-C03_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKH-D01_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKH-D22_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKH-D23_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKH-D42_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_CLICK_VARIO_110_KVB_S53_48KB_ORI.bin` | `.BIN` | `49,152` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_XADV_750_38770_MKH_D22_512KB_ORI.bin` | `.BIN` | `524,288` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_XADV_750_38770_MKH_D42_512KB_ORI.bin` | `.BIN` | `524,288` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
