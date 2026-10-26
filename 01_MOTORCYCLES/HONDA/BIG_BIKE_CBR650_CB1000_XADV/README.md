# HONDA BIG BIKE FOUR CYLINDER FLEET - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/BIG_BIKE_CBR650_CB1000_XADV`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `28 files` (26 binary/calibration dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `BIG_BIKE_CBR650_CB1000_XADV` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Multi-Cylinder Performance Fleet (CBR650F/R, CB650F/R, CB1000R, CB1000F, X-ADV 750) Keihin ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `38770-MFN-D01.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MFN-F01.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MGJ-D02.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MGZ-A03.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MGZ-C02.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MGZ-C03.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MGZ-D02.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MGZ.xdf` | `.XDF` | `145,434` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `38770-MJE-D41.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJE-G12.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJE-G52.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJE-T15.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJE-T52.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJE-TB1.bin` | `.BIN` | `524,288` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJW-AQ1.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJW-DR1.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJW-T11.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MJW.xdf` | `.XDF` | `73,399` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `38770-MKH-D22.bin` | `.BIN` | `524,288` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MKH-D42.bin` | `.BIN` | `524,288` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-MKN-T11.bin` | `.BIN` | `524,288` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770_MJW_D51.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770_MJW_D91.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CB1000R_38770_MFN_D01_256KB_ORI.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CB1000R_38770_MFN_F01_256KB_ORI.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CB650F_38770_MJE_D41_256KB_ORI.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CB650F_38770_MJE_G52_256KB_ORI.bin` | `.BIN` | `262,144` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CBR650R_38770_MKN_T11_512KB_ORI.bin` | `.BIN` | `524,288` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
