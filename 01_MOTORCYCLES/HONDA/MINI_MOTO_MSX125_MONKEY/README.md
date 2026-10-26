# HONDA MINI MOTO MSX125 GROM MONKEY CT125 - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/MINI_MOTO_MSX125_MONKEY`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `16 files` (12 binary/calibration dumps, 4 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MINI_MOTO_MSX125_MONKEY` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Horizontal 125cc Leisure & Adventure Fleet (MSX125, Grom 125, Monkey Z125M, CT125 Hunter Cub) Keihin ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `38770-K0F-A01.bin` | `.BIN` | `98,304` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-K0F-A01.xdf` | `.XDF` | `15,911` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `38770-K26-911.bin` | `.BIN` | `49,152` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-K26-911.xdf` | `.XDF` | `14,097` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `38770-K26-931.bin` | `.BIN` | `49,152` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-K26-B13.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-K26-B13.xdf` | `.XDF` | `12,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `38770-K26-C31.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `38770-K26-C31.xdf` | `.XDF` | `24,483` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `38770-KYT-901.bin` | `.BIN` | `57,344` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_CT125_HUNTER_CUB_38770_K2E_T02_96KB_ORI.bin` | `.BIN` | `98,304` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_GROM_125_38770_K26_G01_96KB_ORI.bin` | `.BIN` | `98,304` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_MONKEY_125_38770_K0F_T01_96KB_ORI.bin` | `.BIN` | `98,304` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_MONKEY_Z125M_38770_K0F_A01_96KB_ORI.bin` | `.BIN` | `98,304` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_MSX125_38770_K26_901_48KB_ORI.bin` | `.BIN` | `49,152` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_MSX125_SF_38770_K26_B13_64KB_ORI.bin` | `.BIN` | `65,536` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
