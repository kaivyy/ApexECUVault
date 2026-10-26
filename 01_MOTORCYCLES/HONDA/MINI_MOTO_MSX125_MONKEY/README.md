# HONDA MINI MOTO MSX125 GROM MONKEY CT125 - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/MINI_MOTO_MSX125_MONKEY`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `16 files` (12 binary/calibration dumps, 4 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MINI_MOTO_MSX125_MONKEY` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Horizontal 125cc Leisure & Adventure Fleet (MSX125, Grom 125, Monkey Z125M, CT125 Hunter Cub) Keihin ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

* **Rentang Tahun / Model Year**: 2013–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `38770-K0F-A01.bin` | **2013–2024** | 96.0 KB | `b1b2d8fbdb85538f1b764e9059f0def5` | Factory Binary Firmware Dump |
| `38770-K0F-A01.xdf` | **2013–2024** | 15.5 KB | `cdffe0fc5392f14f81a4456a9e4c2f34` | TunerPro Binary Definition Map |
| `38770-K26-911.bin` | **2013–2020** | 48.0 KB | `eca31aa92cd73763dd6500174de10e0c` | Factory Binary Firmware Dump |
| `38770-K26-911.xdf` | **2013–2020** | 13.8 KB | `707232a042ceed90cd85b7aa09c88505` | TunerPro Binary Definition Map |
| `38770-K26-931.bin` | **2013–2020** | 48.0 KB | `cf324b8b009cf0f527ef34d8d6ba5021` | Factory Binary Firmware Dump |
| `38770-K26-B13.bin` | **2013–2020** | 64.0 KB | `3ce4aee4afaddf4d8ca3f194b13fc168` | Factory Binary Firmware Dump |
| `38770-K26-B13.xdf` | **2013–2020** | 12.5 KB | `5d433c3d0f453a7b4c72d425831b14e0` | TunerPro Binary Definition Map |
| `38770-K26-C31.bin` | **2013–2020** | 64.0 KB | `4ebb017f7ca9287ae5c54db3a8704106` | Factory Binary Firmware Dump |
| `38770-K26-C31.xdf` | **2013–2020** | 23.9 KB | `1d4c0cfe07e37230dd4b486fe80b2dc5` | TunerPro Binary Definition Map |
| `38770-KYT-901.bin` | **2013–2024** | 56.0 KB | `2c4b1f41ef4bb9d110cc2feaa8a6f744` | Factory Binary Firmware Dump |
| `HONDA_CT125_HUNTER_CUB_38770_K2E_T02_96KB_ORI.bin` | **2013–2024** | 96.0 KB | `9961640a253687ce909811b95a1ea5a3` | Factory Binary Firmware Dump |
| `HONDA_GROM_125_38770_K26_G01_96KB_ORI.bin` | **2013–2020** | 96.0 KB | `483437f2b5eea4afad8e424cd0713bc1` | Factory Binary Firmware Dump |
| `HONDA_MONKEY_125_38770_K0F_T01_96KB_ORI.bin` | **2013–2024** | 96.0 KB | `832da9a1bbaa020173dc66bc402b1b17` | Factory Binary Firmware Dump |
| `HONDA_MONKEY_Z125M_38770_K0F_A01_96KB_ORI.bin` | **2013–2024** | 96.0 KB | `b1b2d8fbdb85538f1b764e9059f0def5` | Factory Binary Firmware Dump |
| `HONDA_MSX125_38770_K26_901_48KB_ORI.bin` | **2013–2020** | 48.0 KB | `c273b62d40678dc3ce070963f880f9dc` | Factory Binary Firmware Dump |
| `HONDA_MSX125_SF_38770_K26_B13_64KB_ORI.bin` | **2013–2020** | 64.0 KB | `3ce4aee4afaddf4d8ca3f194b13fc168` | Factory Binary Firmware Dump |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
