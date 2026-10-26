# JAZZ CITY MOBILIO BRV L15 - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/JAZZ_CITY_MOBILIO_BRV_L15`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `13 files` (0 binary/calibration dumps, 13 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `JAZZ_CITY_MOBILIO_BRV_L15` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Jazz, City, Mobilio, BR-V 1.5L L15 Engine Management Platform. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

* **Rentang Tahun / Model Year**: 2008–2021

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `37805-RD1-X520_Honda_Fit_1.4_16v_SH7058_1Mb.xdf` | **2008–2021** | 4.4 KB | `5194796b09e2fb0d78bae16e889c220f` | TunerPro Binary Definition Map |
| `37805-RME-A220_Honda_Fit_2008_Base__Sport_1.5L__L4_-_Gas.xdf` | **2008** | 164.4 KB | `19999a2b5dcb1d6385f1cf3c85adb206` | TunerPro Binary Definition Map |
| `37805-RME-A520_Honda_Fit_2007_Base__Sport_1.5L__L4_-_Gas.xdf` | **2007** | 3.3 KB | `de27f3391fe20313a190adc0263a4911` | TunerPro Binary Definition Map |
| `37805-RME-A690_Honda_Fit_2007_Base_1.5L__L4_-_Gas.xdf` | **2007** | 3.3 KB | `3820751ea9cb0c63517424968d00e887` | TunerPro Binary Definition Map |
| `37805-RME-A720_Honda_Fit_2008_Base_1.5L__L4_-_Gas.xdf` | **2008** | 3.3 KB | `2547f797235849723b1452653fb9edec` | TunerPro Binary Definition Map |
| `37805-RME-A890_Honda_Fit_2007_Sport_1.5L__L4_-_Gas.xdf` | **2007** | 3.3 KB | `552c51391baf3642202284cc91f19838` | TunerPro Binary Definition Map |
| `37805-RME-C220_Honda_Fit_2008_Sport_1.5L__L4_-_Gas.xdf` | **2008** | 3.3 KB | `ebd37128ab058249f52dcb6219f34a40` | TunerPro Binary Definition Map |
| `37805-RP3-3060_Honda_Fit_2009_Base__Sport_1.5L__L4_-_Gas.xdf` | **2009** | 4.4 KB | `a761212ce470bb96cd0e23b90efa7e41` | TunerPro Binary Definition Map |
| `37805-RP3-4050_Honda_Fit_2009_Base_1.5L__L4_-_Gas.xdf` | **2009** | 4.4 KB | `0e73a0edb114780c1a457fd03b46c950` | TunerPro Binary Definition Map |
| `37805-RP3-A170_Honda_Fit_2009_2010_Sport_1.5L__L4_-_Gas.xdf` | **2009–2010** | 4.4 KB | `378c0b3c3226344fd5864ba75212e3e0` | TunerPro Binary Definition Map |
| `37805-RP3-A770_Honda_Fit_2012_2013_Base__Sport_1.5L__L4_-_Gas.xdf` | **2012–2013** | 4.4 KB | `d88b75c028f8f2ab3eba17948ac2216c` | TunerPro Binary Definition Map |
| `37805-RP6-A560_Honda_Fit_2012_2013_Sport_1.5L__L4_-_Gas.xdf` | **2012–2013** | 7.6 KB | `47fe6f60e2910f3c230b1bb604e039d8` | TunerPro Binary Definition Map |
| `HONDA_37805-5A4-J81_JAZZ_GK5.xdf` | **2008–2021** | 11.9 KB | `0d5c74b19221cb45ea40bd66fb310dc0` | TunerPro Binary Definition Map |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
