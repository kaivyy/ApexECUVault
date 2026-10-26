# BRIO 1.2L L12B - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/BRIO_1_2L_L12B`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `3 files` (2 binary/calibration dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `BRIO_1_2L_L12B` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Brio 1.2L i-VTEC (L12B) Keihin Engine Management Platform. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

* **Rentang Tahun / Model Year**: OEM Production

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `37805-RSJ-E010-M1.rwd` | **OEM Production** | 992.1 KB | `6bc97aa2b565ffc974c872a34a72ad00` | Factory Binary Firmware Dump |
| `37805-RSJ-E210-M1.rwd` | **OEM Production** | 992.1 KB | `01c9492e98557e1e90f817cccd7c1e13` | Factory Binary Firmware Dump |
| `HONDA_37805-RSJ-J51_BRIO.xdf` | **OEM Production** | 11.8 KB | `7c01901fcafa966d4892da7349d88752` | TunerPro Binary Definition Map |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
