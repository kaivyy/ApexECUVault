# SILVIA SR20DET 300ZX VG30DETT - ECU Calibration Suite

**Repository Path**: `02_CARS/NISSAN_INFINITI/SILVIA_SR20DET_300ZX_VG30DETT`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `58 files` (58 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SILVIA_SR20DET_300ZX_VG30DETT` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `S13_SR20DET_50F00_MT_red_top.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `S13_SR20DET_50F01_MT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `S13_SR20DET_50F05_MT_black_top.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `S13_SR20DET_50F10_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `S13_SR20DET_50F11_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `S13_SR20DET_50F15_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `S13_SR20DET_60F06_MT_TypeX.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `S13_SR20DET_60F07_TypeX.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `S13_SR20DET_60F16_TypeX.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F00_MT_red_top.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F01_MT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F05_MT_black_top.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F10_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F11_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F15_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F06_MT_TypeX.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F07_TypeX.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F16_TypeX.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_1989_NA_AT_M257ACA8.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_30P10.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P11.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P12.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P01_1991_1993_MT_EDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P06_MT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P11_AT_1992_EDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P02_MT_JDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P11_AT_TXC_661.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P12_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P13_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P14_JDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_47P10_MT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P00_1990_NA_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P12_1990_NA_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P12_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_40P01_1991_NA_MT_JDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_40P13_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_46P10_1992_AT_ADM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_46P80_1992_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_1989_NA_AT_M257ACA8.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_30P10.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_31P11.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_31P12.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_37P01_1991_1993_MT_EDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_37P06_MT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_37P11_AT_1992_EDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_41P02_MT_JDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_41P11_AT_TXC_661.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_41P12_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_41P13_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_41P14_JDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DETT_47P10_MT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DE_39P00_1990_NA_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DE_39P12_1990_NA_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DE_39P12_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DE_40P01_1991_NA_MT_JDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DE_40P13_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DE_46P10_1992_AT_ADM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Z32_VG30DE_46P80_1992_AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |

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
