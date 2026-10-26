# PRELUDE ACCORD - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/PRELUDE_ACCORD`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `51 files` (14 binary dumps, 37 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `PRELUDE_ACCORD` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805-5A2-A160_Honda_Accord_2013_LX__LX-S__Sport_2.4L__L4_-_Gas.xdf` | `.XDF` | `106,408` bytes | Honda Keihin Factory Calibration Package `37805-5A2-A160` |
| `37805-5AM-A050_Honda_Accord_2014_EX__EX-L_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `133,220` bytes | Honda Keihin Factory Calibration Package `37805-5AM-A050` |
| `37805-5G2-A050_Honda_Accord_2013_EX-L_3.5L_V6_-_Gas.xdf` | `.XDF` | `73,054` bytes | Honda Keihin Factory Calibration Package `37805-5G2-A050` |
| `37805-5G2-A120_Honda_Accord_2015_EX-L_3.5L_V6_-_Gas.xdf` | `.XDF` | `71,841` bytes | Honda Keihin Factory Calibration Package `37805-5G2-A120` |
| `37805-R40-A240_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,041` bytes | Honda Keihin Factory Calibration Package `37805-R40-A240` |
| `37805-R40-A340_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas___ECU_Honda_Accord.xdf` | `.XDF` | `5,159` bytes | Honda Keihin Factory Calibration Package `37805-R40-A340` |
| `37805-R40-A340_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas___ECU_Honda_Accord_2.4_16v_200Hp_KEIHIN_37820-R40-A3X_SH7058_1Mb_37805-R40-A340_37805-R40-A330_37805-R40-A320_37805-R40-A310.xdf` | `.XDF` | `5,159` bytes | Honda Keihin Factory Calibration Package `37805-R40-A340` |
| `37805-R40-A590_Honda_Accord_2012_LX_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,030` bytes | Honda Keihin Factory Calibration Package `37805-R40-A590` |
| `37805-R40-A730_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,041` bytes | Honda Keihin Factory Calibration Package `37805-R40-A730` |
| `37805-R40-A830_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,036` bytes | Honda Keihin Factory Calibration Package `37805-R40-A830` |
| `37805-R40-K030_Honda_Accord_2011_2012_LX__LX-P__SE_LX_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,048` bytes | Honda Keihin Factory Calibration Package `37805-R40-K030` |
| `37805-R41-L590_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | `.XDF` | `5,024` bytes | Honda Keihin Factory Calibration Package `37805-R41-L590` |
| `37805-R41-L630_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,041` bytes | Honda Keihin Factory Calibration Package `37805-R41-L630` |
| `37805-R41-L730_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,036` bytes | Honda Keihin Factory Calibration Package `37805-R41-L730` |
| `37805-R42-A090_Honda_Accord_2012_LX__LX-P__SE_2.4L__L4_-_Gas___ECU_Honda_Ac.xdf` | `.XDF` | `5,223` bytes | Honda Keihin Factory Calibration Package `37805-R42-A090` |
| `37805-R42-A090_Honda_Accord_2012_LX__LX-P__SE_2.4L__L4_-_Gas___ECU_Honda_Accord_2.4_16v_200Hp_KEIHIN_37820-R42-A0X_SH7058_1Mb_37805-R42-A090_37805-R42-A080_37805-R42-A070_37805-R42-A060_37805-R42-A050_37805-R42-A040_37805-R42-A030_37805-R42-A020.xdf` | `.XDF` | `5,223` bytes | Honda Keihin Factory Calibration Package `37805-R42-A090` |
| `37805-R42-A140_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,076` bytes | Honda Keihin Factory Calibration Package `37805-R42-A140` |
| `37805-R42-A140_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | `.XDF` | `5,076` bytes | Honda Keihin Factory Calibration Package `37805-R42-A140` |
| `37805-R42-A240_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,058` bytes | Honda Keihin Factory Calibration Package `37805-R42-A240` |
| `37805-R42-A240_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,058` bytes | Honda Keihin Factory Calibration Package `37805-R42-A240` |
| `37805-R42-A590_Honda_Accord_2012_EX__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,052` bytes | Honda Keihin Factory Calibration Package `37805-R42-A590` |
| `37805-R42-A630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,076` bytes | Honda Keihin Factory Calibration Package `37805-R42-A630` |
| `37805-R42-A630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | `.XDF` | `5,076` bytes | Honda Keihin Factory Calibration Package `37805-R42-A630` |
| `37805-R42-A730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,058` bytes | Honda Keihin Factory Calibration Package `37805-R42-A730` |
| `37805-R42-A730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | `.XDF` | `5,058` bytes | Honda Keihin Factory Calibration Package `37805-R42-A730` |
| `37805-R43-L590_Honda_Accord_2012_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,241` bytes | Honda Keihin Factory Calibration Package `37805-R43-L590` |
| `37805-R43-L630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | `.XDF` | `5,076` bytes | Honda Keihin Factory Calibration Package `37805-R43-L630` |
| `37805-R43-L730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,058` bytes | Honda Keihin Factory Calibration Package `37805-R43-L730` |
| `37805-R44-X630_Honda_Accord_2012_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | `.XDF` | `5,166` bytes | Honda Keihin Factory Calibration Package `37805-R44-X630` |
| `37805-R46-X630_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | `.XDF` | `5,024` bytes | Honda Keihin Factory Calibration Package `37805-R46-X630` |
| `37805-R60-M540_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | `.XDF` | `3,904` bytes | Honda Keihin Factory Calibration Package `37805-R60-M540` |
| `37805-RCA-A250_Honda_Accord_2003_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,467` bytes | Honda Keihin Factory Calibration Package `37805-RCA-A250` |
| `37805-RCA-A470_Honda_Accord_2007_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,467` bytes | Honda Keihin Factory Calibration Package `37805-RCA-A470` |
| `37805-RCA-A750_Honda_Accord_2005_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,467` bytes | Honda Keihin Factory Calibration Package `37805-RCA-A750` |
| `37805-RCA-L470_Honda_Accord_2006_2007_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,472` bytes | Honda Keihin Factory Calibration Package `37805-RCA-L470` |
| `37805-RCA-L750_Honda_Accord_2005_EX_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,467` bytes | Honda Keihin Factory Calibration Package `37805-RCA-L750` |
| `37805-RCA-M550_Honda_Accord_2005_EX__LX__SE_3.0L__V6_-_Gas.xdf` | `.XDF` | `4,475` bytes | Honda Keihin Factory Calibration Package `37805-RCA-M550` |
| `37820-P11-G00.bin` | `.BIN` | `32,768` bytes | Honda OBD1/OBD2 ECU Hardware Code `37820-P11` |
| `37820-P13-Q00.bin` | `.BIN` | `32,768` bytes | Honda OBD1/OBD2 ECU Hardware Code `37820-P13` |
| `HONDA_ACCORD_CR2_2013-2017_2.4L_K24W_EARTH_DREAMS_KEIHIN_37805-5A0-X920-M1.rwd` | `.RWD` | `2,031,698` bytes | Honda Keihin Factory Calibration Package `37805-5A0-X920` |
| `P13-G00-C3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `P13-N01-E6.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `P13OEMJ50AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `P14-A11_stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `PH3-0732-88-89-Accord.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p12-a00.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p14-q00-c0.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p14-q52-e4.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p14.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `pt3-q50-83.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `pt6-j50-d2.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance, Low/High Octane Timing, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow & Boost Management**: Peta Target Boost Pressure, Wastegate Duty Cycle (WGDC), MAF/MAP Scaling, dan Throttle Response Curves.
- **Safety Limits & Thresholds**: Rev Limiter (Hard/Soft Cut), Top Speed Limiter (Vmax), Overboost Fuel Cut, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
