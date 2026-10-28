# SILVIA_SR20DET_300ZX_VG30DETT - ECU Calibration Suite

**Repository Path**: `02_CARS/NISSAN_INFINITI/SILVIA_SR20DET_300ZX_VG30DETT`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `84 files` (84 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SILVIA_SR20DET_300ZX_VG30DETT` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `S13_SR20DET_50F00_MT_red_top.bin` | **2000–2024** | 32.0 KB | `331c675160d4b3a2f8e6c2fc7643c70b` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F01_MT.bin` | **2000–2024** | 32.0 KB | `ed637f93635ab118fba7a530af15b468` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F05_MT_black_top.bin` | **2000–2024** | 32.0 KB | `dd65894d26d7b081ce2138ae7f4e52b6` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F10_AT.bin` | **2000–2024** | 32.0 KB | `c5c53a6a5724e98b36b37a4fa2eb0df4` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F11_AT.bin` | **2000–2024** | 32.0 KB | `c6de968d6c92d05fa8f29d3d864a535a` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F15_AT.bin` | **2000–2024** | 32.0 KB | `4890359a20d053b80d122a3ebc4b8ece` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F06_MT_TypeX.bin` | **2000–2024** | 32.0 KB | `5ff40c110fa7bc294942198a79bc1067` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F07_TypeX.bin` | **2000–2024** | 32.0 KB | `fa1ffcb7f80b833c34df801ec5033a7d` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F16_TypeX.bin` | **2000–2024** | 32.0 KB | `e0218e51b46b0957f3403bdbecb4efb1` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F00_MT_red_top.bin` | **2000–2024** | 32.0 KB | `331c675160d4b3a2f8e6c2fc7643c70b` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F01_MT.bin` | **2000–2024** | 32.0 KB | `ed637f93635ab118fba7a530af15b468` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F05_MT_black_top.bin` | **2000–2024** | 32.0 KB | `dd65894d26d7b081ce2138ae7f4e52b6` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F10_AT.bin` | **2000–2024** | 32.0 KB | `c5c53a6a5724e98b36b37a4fa2eb0df4` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F11_AT.bin` | **2000–2024** | 32.0 KB | `c6de968d6c92d05fa8f29d3d864a535a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F15_AT.bin` | **2000–2024** | 32.0 KB | `4890359a20d053b80d122a3ebc4b8ece` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F06_MT_TypeX.bin` | **2000–2024** | 32.0 KB | `5ff40c110fa7bc294942198a79bc1067` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F07_TypeX.bin` | **2000–2024** | 32.0 KB | `fa1ffcb7f80b833c34df801ec5033a7d` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F16_TypeX.bin` | **2000–2024** | 32.0 KB | `e0218e51b46b0957f3403bdbecb4efb1` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_1989_NA_AT_M257ACA8.bin` | **1989** | 32.0 KB | `634969617a539295be2a95bac8f13cf3` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_30P10.bin` | **2000–2024** | 32.0 KB | `c675735fade59ef7e66faeadd2e00e24` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P02_1990_MT_FED.BIN` | **1990** | 32.0 KB | `bc726e7565cd9ae3b6c7ba651364e784` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P03_1990_MT_FED.BIN` | **1990** | 32.0 KB | `97c50fa61263428c981e600dec6ce313` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P08_1990_MT_CALI.BIN` | **1990** | 32.0 KB | `bb9668c388d54882c605eddcd38d03fe` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P11.bin` | **2000–2024** | 32.0 KB | `6a4885cf061d8f7452ff441f5eea6acd` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P12.bin` | **2000–2024** | 32.0 KB | `c7e984bdc4864426799ec4e9695f09aa` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P01_1991_1993_MT_EDM.bin` | **1991–1993** | 32.0 KB | `7fca8db92cbbc9f811923a370def1d83` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P06_MT.bin` | **2000–2024** | 32.0 KB | `a6a655c1e5587c05d8b510a99831de58` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P11_AT_1992_EDM.bin` | **1992** | 32.0 KB | `9c8edf0efb04ddfa4645048e94d04526` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P01_AT_1990_JDM_M4.BIN` | **1990** | 32.0 KB | `123fd911b8e8d6d6308da239401a17a9` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P02_MT_JDM.bin` | **2000–2024** | 32.0 KB | `2917c557091a9df4d97428ffe38f5a09` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P03_MT_JDM.BIN` | **2000–2024** | 32.0 KB | `76f4afd37d040a861963b9db48425d35` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P04_MT_1991_JDM.BIN` | **1991** | 32.0 KB | `4fb4d51f776d68259de427305eca1a7a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P11_AT_TXC_661.bin` | **2000–2024** | 32.0 KB | `bfee693253557eef52f53b33d6ff81ac` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P12_AT.bin` | **2000–2024** | 32.0 KB | `80b92e376e3da858b42b9288c8212599` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P13_AT.bin` | **2000–2024** | 32.0 KB | `8277b6aeb51ce560e4a949cace0979f7` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P14_JDM.bin` | **2000–2024** | 32.0 KB | `7d15b18850f72c9a3d401cad2ebcb0dd` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P60_MT_1992.BIN` | **1992** | 32.0 KB | `4409df9b429e02f268e7d654c4f15529` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P70_MT.BIN` | **2000–2024** | 32.0 KB | `a0d4f6a1884d5d0b465573e37b0fa905` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_47P10_MT.bin` | **2000–2024** | 32.0 KB | `d698dd4a383c96dc5cdcd890b53cfc08` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_48P01_MT_1991.BIN` | **1991** | 32.0 KB | `af4656fd08c4c8c9f0451d56c7ebb126` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_48P76.BIN` | **2000–2024** | 32.0 KB | `2de0ea0c9ce88fc649eb238df57d9c70` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_30P00_1990_NA_MT_FED.BIN` | **1990** | 32.0 KB | `decdee3ae2db76af59e9f12576e774a8` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_30P60_1990_NA_MT_FED.BIN` | **1990** | 32.0 KB | `4edc4bbcf0bbcfe5f83842393a5ec6c3` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_30P75_1991_NA_AT.BIN` | **1991** | 32.0 KB | `b6e807523ca68acbaf215223e430b8ce` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P00_1990_NA_AT.bin` | **1990** | 32.0 KB | `3287d5ece0ee82c4626c91dcc74fc90c` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P12_1990_NA_AT.bin` | **1990** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P12_AT.bin` | **2000–2024** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_40P01_1991_NA_MT_JDM.bin` | **1991** | 32.0 KB | `9ccebd22f09f29afe03615984cbf2add` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_40P13_AT.bin` | **2000–2024** | 32.0 KB | `c8b592bf26ed5128eb8b8b8c19fc4fa6` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_46P10_1992_AT_ADM.bin` | **1992** | 32.0 KB | `83f20f9d6b2f4e827cf80a5bfdbbf644` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_46P80_1992_AT.bin` | **1992** | 32.0 KB | `c65c5518813167583ccf898840eab84e` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_1989_NA_AT_M257ACA8.bin` | **1989** | 32.0 KB | `634969617a539295be2a95bac8f13cf3` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_30P10.bin` | **2000–2024** | 32.0 KB | `c675735fade59ef7e66faeadd2e00e24` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P02_1990_MT_FED.BIN` | **1990** | 32.0 KB | `bc726e7565cd9ae3b6c7ba651364e784` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P03_1990_MT_FED.BIN` | **1990** | 32.0 KB | `97c50fa61263428c981e600dec6ce313` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P08_1990_MT_CALI.BIN` | **1990** | 32.0 KB | `bb9668c388d54882c605eddcd38d03fe` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P11.bin` | **2000–2024** | 32.0 KB | `6a4885cf061d8f7452ff441f5eea6acd` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P12.bin` | **2000–2024** | 32.0 KB | `c7e984bdc4864426799ec4e9695f09aa` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P01_1991_1993_MT_EDM.bin` | **1991–1993** | 32.0 KB | `7fca8db92cbbc9f811923a370def1d83` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P06_MT.bin` | **2000–2024** | 32.0 KB | `a6a655c1e5587c05d8b510a99831de58` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P11_AT_1992_EDM.bin` | **1992** | 32.0 KB | `9c8edf0efb04ddfa4645048e94d04526` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P01_AT_1990_JDM_M4.BIN` | **1990** | 32.0 KB | `123fd911b8e8d6d6308da239401a17a9` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P02_MT_JDM.bin` | **2000–2024** | 32.0 KB | `2917c557091a9df4d97428ffe38f5a09` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P03_MT_JDM.BIN` | **2000–2024** | 32.0 KB | `76f4afd37d040a861963b9db48425d35` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P04_MT_1991_JDM.BIN` | **1991** | 32.0 KB | `4fb4d51f776d68259de427305eca1a7a` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P11_AT_TXC_661.bin` | **2000–2024** | 32.0 KB | `bfee693253557eef52f53b33d6ff81ac` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P12_AT.bin` | **2000–2024** | 32.0 KB | `80b92e376e3da858b42b9288c8212599` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P13_AT.bin` | **2000–2024** | 32.0 KB | `8277b6aeb51ce560e4a949cace0979f7` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P14_JDM.bin` | **2000–2024** | 32.0 KB | `7d15b18850f72c9a3d401cad2ebcb0dd` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P60_MT_1992.BIN` | **1992** | 32.0 KB | `4409df9b429e02f268e7d654c4f15529` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P70_MT.BIN` | **2000–2024** | 32.0 KB | `a0d4f6a1884d5d0b465573e37b0fa905` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_47P10_MT.bin` | **2000–2024** | 32.0 KB | `d698dd4a383c96dc5cdcd890b53cfc08` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_48P01_MT_1991.BIN` | **1991** | 32.0 KB | `af4656fd08c4c8c9f0451d56c7ebb126` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_48P76.BIN` | **2000–2024** | 32.0 KB | `2de0ea0c9ce88fc649eb238df57d9c70` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P00_1990_NA_MT_FED.BIN` | **1990** | 32.0 KB | `decdee3ae2db76af59e9f12576e774a8` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P60_1990_NA_MT_FED.BIN` | **1990** | 32.0 KB | `4edc4bbcf0bbcfe5f83842393a5ec6c3` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P75_1991_NA_AT.BIN` | **1991** | 32.0 KB | `b6e807523ca68acbaf215223e430b8ce` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P00_1990_NA_AT.bin` | **1990** | 32.0 KB | `3287d5ece0ee82c4626c91dcc74fc90c` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P12_1990_NA_AT.bin` | **1990** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P12_AT.bin` | **2000–2024** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `Z32_VG30DE_40P01_1991_NA_MT_JDM.bin` | **1991** | 32.0 KB | `9ccebd22f09f29afe03615984cbf2add` | Factory Binary Firmware Dump |
| `Z32_VG30DE_40P13_AT.bin` | **2000–2024** | 32.0 KB | `c8b592bf26ed5128eb8b8b8c19fc4fa6` | Factory Binary Firmware Dump |
| `Z32_VG30DE_46P10_1992_AT_ADM.bin` | **1992** | 32.0 KB | `83f20f9d6b2f4e827cf80a5bfdbbf644` | Factory Binary Firmware Dump |
| `Z32_VG30DE_46P80_1992_AT.bin` | **1992** | 32.0 KB | `c65c5518813167583ccf898840eab84e` | Factory Binary Firmware Dump |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi yang tersedia, struktur kalibrasi mencakup parameter esensial:
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
