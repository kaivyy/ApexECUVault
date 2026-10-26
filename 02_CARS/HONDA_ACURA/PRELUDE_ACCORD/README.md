# PRELUDE ACCORD - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/PRELUDE_ACCORD`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `55 files` (16 binary/calibration dumps, 37 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `PRELUDE_ACCORD` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Accord & Prelude V6/I4 Engine Management Platform. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805-5A2-A160_Honda_Accord_2013_LX__LX-S__Sport_2.4L__L4_-_Gas.xdf` | `.XDF` | `106,408` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AM-A050_Honda_Accord_2014_EX__EX-L_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `133,220` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5G2-A050_Honda_Accord_2013_EX-L_3.5L_V6_-_Gas.xdf` | `.XDF` | `73,054` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5G2-A120_Honda_Accord_2015_EX-L_3.5L_V6_-_Gas.xdf` | `.XDF` | `71,841` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-A240_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,041` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-A340_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas___ECU_Honda_Accord.xdf` | `.XDF` | `5,159` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-A340_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas___ECU_Honda_Accord_2.4_16v_200Hp_KEIHIN_37820-R40-A3X_SH7058_1Mb_37805-R40-A340_37805-R40-A330_37805-R40-A320_37805-R40-A310.xdf` | `.XDF` | `5,159` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-A590_Honda_Accord_2012_LX_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,030` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-A730_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,041` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-A830_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,036` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-K030_Honda_Accord_2011_2012_LX__LX-P__SE_LX_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,048` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R41-L590_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | `.XDF` | `5,024` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R41-L630_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,041` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R41-L730_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,036` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A090_Honda_Accord_2012_LX__LX-P__SE_2.4L__L4_-_Gas___ECU_Honda_Ac.xdf` | `.XDF` | `5,223` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A090_Honda_Accord_2012_LX__LX-P__SE_2.4L__L4_-_Gas___ECU_Honda_Accord_2.4_16v_200Hp_KEIHIN_37820-R42-A0X_SH7058_1Mb_37805-R42-A090_37805-R42-A080_37805-R42-A070_37805-R42-A060_37805-R42-A050_37805-R42-A040_37805-R42-A030_37805-R42-A020.xdf` | `.XDF` | `5,223` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A140_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,076` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A140_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | `.XDF` | `5,076` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A240_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,058` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A240_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,058` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A590_Honda_Accord_2012_EX__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,052` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,076` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | `.XDF` | `5,076` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,058` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R42-A730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,058` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R43-L590_Honda_Accord_2012_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,241` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R43-L630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | `.XDF` | `5,076` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R43-L730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,058` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R44-X630_Honda_Accord_2012_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,166` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R46-X630_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | `.XDF` | `5,024` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R60-M540_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | `.XDF` | `3,904` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-A250_Honda_Accord_2003_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,467` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-A470_Honda_Accord_2007_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,467` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-A750_Honda_Accord_2005_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,467` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-L470_Honda_Accord_2006_2007_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,472` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-L750_Honda_Accord_2005_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,467` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-M550_Honda_Accord_2005_EX__LX__SE_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,475` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37820-P11-G00.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `37820-P13-Q00.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `HONDA_ACCORD_CR2_2013-2017_2.4L_K24W_EARTH_DREAMS_KEIHIN_37805-5A0-X920-M1.rwd` | `.RWD` | `2,031,698` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `P13-G00-C3.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `P13-N01-E6.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `P13.JDM.Prelude.BIN` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `P13OEMJ50AT.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `P14-A11_stock.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `PH3-0732-88-89-Accord.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `PT3_A54.BIN` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `p12-a00.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `p12-a00.rom` | `.ROM` | `32,768` bytes | Technical Calibration Asset |
| `p14-q00-c0.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `p14-q52-e4.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `p14.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `pt3-q50-83.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `pt6-j50-d2.bin` | `.BIN` | `32,768` bytes | OEM Firmware Calibration Flash Dump / Binary Package |
| `pt6-q50-97.rom` | `.ROM` | `32,768` bytes | Technical Calibration Asset |

### Subdirektori Tambahan

- **`OFFICIAL_CALIBRATION_PACKAGES/`**: Mengelola 458 aset kalibrasi lanjutan.

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
