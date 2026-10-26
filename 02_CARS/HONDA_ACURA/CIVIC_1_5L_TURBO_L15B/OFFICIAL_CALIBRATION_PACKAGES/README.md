# HONDA CIVIC TURBO OFFICIAL CALIBRATIONS - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CIVIC_1_5L_TURBO_L15B/OFFICIAL_CALIBRATION_PACKAGES`  
**Classification**: `Binary Flash Memory & OEM Firmware Dump Suite`  
**Total Managed Assets**: `5 files` (5 binary/calibration dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `OFFICIAL_CALIBRATION_PACKAGES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Civic FC 1.5L Turbo Factory Calibration Packages. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805-5AA-A020-M1.rwd` | `.RWD` | `2,555,986` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5AM-A120-M1.rwd` | `.RWD` | `2,555,962` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5AM-A220-M1.rwd` | `.RWD` | `2,555,962` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5AN-A220-M1.rwd` | `.RWD` | `2,555,962` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5AN-AF20-M1.rwd` | `.RWD` | `2,555,962` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
