# HONDA TRAIL CRF SERIES - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/TRAIL_CRF150L_CRF250L`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `23 files` (6 binary/calibration dumps, 17 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `TRAIL_CRF150L_CRF250L` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Dual-Sport, Trail & Motocross Fleet (CRF110F, CRF150L, CRF250L/Rally, CRF450R/HRC) Keihin ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `38770-EKCJ-J000.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-KYK-D12.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-KYK-D12.xdf` | `.XDF` | `18,666` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `38770-MEN-E21.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MKE-DataSettings.xdf` | `.XDF` | `23,570` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_38770-K84-901_Honda_CRF150L_Trail_Dual_Purpose_2017_2025.xdf` | `.XDF` | `2,547` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K1T-A11_CRF300L___CRF300_Rally_(2021-2024).xdf` | `.XDF` | `16,713` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K1T-T01_CRF300L___CRF300_Rally_(2021-2024).xdf` | `.XDF` | `16,713` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-K84-901_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KYK-D12_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KZZ-902_CRF250L___CRF250M___CRF250_Rally.xdf` | `.XDF` | `16,719` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KZZ-914_CRF250L___CRF250M___CRF250_Rally.xdf` | `.XDF` | `16,719` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KZZ-A22_CRF250L___CRF250M___CRF250_Rally.xdf` | `.XDF` | `16,719` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KZZ-J01_CRF250L___CRF250M___CRF250_Rally.xdf` | `.XDF` | `16,711` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KZZ-J81_CRF250L___CRF250M___CRF250_Rally.xdf` | `.XDF` | `16,711` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-KZZ-L41_CRF250L___CRF250M___CRF250_Rally.xdf` | `.XDF` | `16,711` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKE-A71_Honda_Generic_ECM.xdf` | `.XDF` | `16,704` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKE-A81_Honda_Generic_ECM.xdf` | `.XDF` | `16,704` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKE-AF3_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_38770-MKK-D02_Africa_Twin_CRF1000L___CRF1100L.xdf` | `.XDF` | `16,706` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_CRF110F_38770_KYK_D12_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CRF450R_38770_MEN_E21_256KB_ORI.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CRF450R_HRC_38770_EKCJ_J000_256KB_ORI.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
