# CIVIC 1.5L TURBO L15B - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CIVIC_1_5L_TURBO_L15B`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `12 files` (1 binary/calibration dumps, 11 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CIVIC_1_5L_TURBO_L15B` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Civic 1.5L Turbo Generation Platform. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805-5AA-A080_Honda_Civic_2017_EX-T_1.5L_L4_-_Gas.xdf` | `.XDF` | `100,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AA-A580_Honda_Civic_2016_2017_EX-L__EX-T_1.5L_L4_-_Gas.xdf` | `.XDF` | `103,402` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AA-A640_Honda_Civic_2016_2017_EX-L__EX-T__Touring_1.5L_L4_-_Gas.xdf` | `.XDF` | `108,116` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AM-A120_Honda_Civic_2019_Si_1.5L_L4_-_Gas.xdf` | `.XDF` | `101,115` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AM-A220_Honda_Civic_2020_Si_1.5L_L4_-_Gas.xdf` | `.XDF` | `121,713` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AN-A220_Honda_Civic_2019_Sport_1.5L_L4_-_Gas__2.0L_L4_-_Gas.xdf` | `.XDF` | `98,964` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5BF-A340_Honda_Civic_2020_Touring__Type_R_1.5L_L4_-_Gas__2.0L_L4_-_Ga.xdf` | `.XDF` | `121,164` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5BF-A340_Honda_Civic_2020_Touring__Type_R_1.5L_L4_-_Gas__2.0L_L4_-_Gas.xdf` | `.XDF` | `121,164` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_37805-5AA-A640_Honda_Civic_RS_Turbo_1.5L_VTEC_2016_2021.xdf` | `.XDF` | `1,527` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `GENERATIONAL_37805-64A-A01_CIVIC_GEN11_Honda_Civic_RS_Gen_11_VTEC_Turbo_FE___FL_(2021-2026).xdf` | `.XDF` | `5,580` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_37805-5AA-A01_CIVIC_TURBO.xdf` | `.XDF` | `12,148` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_CRV_CIVIC_TURBO_2017-2022_1.5L_L15B7_KEIHIN_37805-5LA-C940-M1.rwd` | `.RWD` | `2,031,746` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

### Subdirektori Tambahan

- **`OFFICIAL_CALIBRATION_PACKAGES/`**: Mengelola 127 aset kalibrasi lanjutan.

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
