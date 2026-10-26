# JAZZ CITY MOBILIO BRV L15 - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/JAZZ_CITY_MOBILIO_BRV_L15`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `13 files` (0 binary/calibration dumps, 13 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `JAZZ_CITY_MOBILIO_BRV_L15` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Jazz, City, Mobilio, BR-V 1.5L L15 Engine Platform. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805-RD1-X520_Honda_Fit_1.4_16v_SH7058_1Mb.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-A220_Honda_Fit_2008_Base__Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `168,318` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-A520_Honda_Fit_2007_Base__Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,343` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-A690_Honda_Fit_2007_Base_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,336` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-A720_Honda_Fit_2008_Base_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,336` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-A890_Honda_Fit_2007_Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,337` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-C220_Honda_Fit_2008_Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `3,337` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RP3-3060_Honda_Fit_2009_Base__Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `4,473` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RP3-4050_Honda_Fit_2009_Base_1.5L__L4_-_Gas.xdf` | `.XDF` | `4,466` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RP3-A170_Honda_Fit_2009_2010_Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `4,472` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RP3-A770_Honda_Fit_2012_2013_Base__Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `4,478` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RP6-A560_Honda_Fit_2012_2013_Sport_1.5L__L4_-_Gas.xdf` | `.XDF` | `7,804` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_37805-5A4-J81_JAZZ_GK5.xdf` | `.XDF` | `12,149` bytes | TunerPro Binary Definition Map / Parameter Layout |

### Subdirektori Tambahan

- **`OFFICIAL_CALIBRATION_PACKAGES/`**: Mengelola 22 aset kalibrasi lanjutan.

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
