# YARIS CROSS VELOZ 2NR-VE - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/YARIS_CROSS_VELOZ_2NR_VE`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `2 files` (1 binary/calibration dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `YARIS_CROSS_VELOZ_2NR_VE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Toyota Veloz, Avanza Gen 3, Yaris Cross 2NR-VE & Renesas RH850 P1M-E SecOC MCU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `GENERATIONAL_89661-BZ890_Toyota_Veloz_Yaris_Cross_1.5_2NR-VE_(2022-2026).xdf` | `.XDF` | `10,061` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `TOYOTA_RH850_P1M_E_SECOC_8965B4512000.bin` | `.BIN` | `1,081,344` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
