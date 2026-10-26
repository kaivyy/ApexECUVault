# HONDA L15 OFFICIAL CALIBRATIONS - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/JAZZ_CITY_MOBILIO_BRV_L15/OFFICIAL_CALIBRATION_PACKAGES`  
**Classification**: `Binary Flash Memory & OEM Firmware Dump Suite`  
**Total Managed Assets**: `21 files` (14 binary/calibration dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `OFFICIAL_CALIBRATION_PACKAGES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Jazz, City, Mobilio, BR-V 1.5L L15 Series Factory Calibration Packages. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805-55A-F130-M1.rwd` | `.RWD` | `2,031,722` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-55D-M050-M8.rwd` | `.RWD` | `1,048,701` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-58R-T530-M1.rwd` | `.RWD` | `2,031,722` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-58R-U550-M1.rwd` | `.RWD` | `2,031,770` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5A4-H540-M1.rwd` | `.RWD` | `2,031,746` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5A4-H540-M1.rwd.gz` | `.GZ` | `883,234` bytes | Technical Calibration Asset |
| `37805-5A4-H640-M1.rwd` | `.RWD` | `2,031,746` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5A4-H640-M1.rwd.gz` | `.GZ` | `883,241` bytes | Technical Calibration Asset |
| `37805-5EA-K030-M1.rwd` | `.RWD` | `2,031,722` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5EA-K220-M1.rwd` | `.RWD` | `2,031,698` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-5EA-K540-M1.rwd` | `.RWD` | `2,031,746` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-RB0-3050.RWD` | `.RWD` | `1,016,010` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-RB0-3050.RWD.gz` | `.GZ` | `286,352` bytes | Technical Calibration Asset |
| `37805-RB0-4050-M1.RWD` | `.RWD` | `1,015,890` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-RB0-4050-M1.RWD.gz` | `.GZ` | `303,031` bytes | Technical Calibration Asset |
| `37805-RB0-9660-M1.rwd` | `.RWD` | `1,015,890` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-RB0-9660-M1.rwd.gz` | `.GZ` | `323,218` bytes | Technical Calibration Asset |
| `37805-RB0-E030-M1.rwd` | `.RWD` | `1,015,914` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-RB0-E030-M1.rwd.gz` | `.GZ` | `300,974` bytes | Technical Calibration Asset |
| `37805-RB0-J030-M1.rwd` | `.RWD` | `1,015,890` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37805-RB0-J030-M1.rwd.gz` | `.GZ` | `323,138` bytes | Technical Calibration Asset |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
