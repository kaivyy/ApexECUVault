# UNDERBONE SONIC GTR SUPRA WAVE - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/UNDERBONE_SONIC_GTR_SUPRA_WAVE`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `77 files` (0 binary dumps, 77 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `UNDERBONE_SONIC_GTR_SUPRA_WAVE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `GENERATIONAL_38770-K56-N11_Honda_Supra_GTR_150___Winner_150_Gen_1_2016_2019.xdf` | `.XDF` | `2,553` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `GENERATIONAL_38770-K56-V01_Honda_Supra_GTR_150_Facelift___Winner_X_Gen_2_2020_2025.xdf` | `.XDF` | `2,560` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `HONDA_38770-K03-H01_Wave_110i_(2019-2020).xdf` | `.XDF` | `16,700` bytes | Honda Motorcycle Keihin ECU ROM `38770-K03` |
| `HONDA_38770-K03-N32_Wave_110i_(2019-2020).xdf` | `.XDF` | `16,700` bytes | Honda Motorcycle Keihin ECU ROM `38770-K03` |
| `HONDA_38770-K03-T61_Wave_110i_(2019-2020).xdf` | `.XDF` | `16,700` bytes | Honda Motorcycle Keihin ECU ROM `38770-K03` |
| `HONDA_38770-K0G-962_Super_Cub_110_Pro.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K0G` |
| `HONDA_38770-K1M-T01_Wave_110i_AT.xdf` | `.XDF` | `16,691` bytes | Honda Motorcycle Keihin ECU ROM `38770-K1M` |
| `HONDA_38770-K2J-T01_Wave_110i___Super_Cub_(2021-2024).xdf` | `.XDF` | `16,712` bytes | Honda Motorcycle Keihin ECU ROM `38770-K2J` |
| `HONDA_38770-K2J-TH1_Wave_110i___Super_Cub_(2021-2024).xdf` | `.XDF` | `16,712` bytes | Honda Motorcycle Keihin ECU ROM `38770-K2J` |
| `HONDA_38770-K3F-T01_Wave_125i_(2023-2024).xdf` | `.XDF` | `16,700` bytes | Honda Motorcycle Keihin ECU ROM `38770-K3F` |
| `HONDA_38770-K41-N01_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K41` |
| `HONDA_38770-K56-M01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `HONDA_38770-K56-M91_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `HONDA_38770-K56-N01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `HONDA_38770-K56-N11_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `HONDA_38770-K56-NJ1_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `HONDA_38770-K56-V01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `HONDA_38770-K56-V51_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | `.XDF` | `16,718` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `HONDA_38770-K58-N41_Wave_110i___Wave_125i_(2020-2022).xdf` | `.XDF` | `16,712` bytes | Honda Motorcycle Keihin ECU ROM `38770-K58` |
| `HONDA_38770-K58-T81_Wave_110i___Wave_125i_(2020-2022).xdf` | `.XDF` | `16,712` bytes | Honda Motorcycle Keihin ECU ROM `38770-K58` |
| `HONDA_38770-K58-TC2_Wave_110i___Wave_125i_(2020-2022).xdf` | `.XDF` | `16,712` bytes | Honda Motorcycle Keihin ECU ROM `38770-K58` |
| `HONDA_38770-K73-M41_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-K73` |
| `HONDA_38770-K73-M62_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-K73` |
| `HONDA_38770-K73-T32_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-K73` |
| `HONDA_38770-K73-T61_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-K73` |
| `HONDA_38770-K73-TC2_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-K73` |
| `HONDA_38770-K73-V42_Wave_125i_LED_(2018-2022).xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-K73` |
| `HONDA_38770-KWW-642_Wave_110i_(2009-2018).xdf` | `.XDF` | `16,700` bytes | Honda Motorcycle Keihin ECU ROM `38770-KWW` |
| `HONDA_38770-KWW-643_Wave_110i_(2009-2018).xdf` | `.XDF` | `16,700` bytes | Honda Motorcycle Keihin ECU ROM `38770-KWW` |
| `HONDA_38770-KYZ-713_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYZ` |
| `HONDA_38770-KYZ-T03_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYZ` |
| `HONDA_38770-KYZ-T41_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYZ` |
| `HONDA_38770-KYZ-V21_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYZ` |
| `HONDA_38770-KYZ-V71_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | `.XDF` | `16,719` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYZ` |
| `HONDA_38770-KZV-A61_Dream_Super_Cub_110_(2013-2017).xdf` | `.XDF` | `16,710` bytes | Honda Motorcycle Keihin ECU ROM `38770-KZV` |
| `HONDA_38770-MEL-613_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MEL-622_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MEL-643_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MEL-A21_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MEL-A22_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MEL-D01_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MEL-D21_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MEL-F21_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MEL-L22_CBR1000RR_Fireblade_(2004-2007).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEL` |
| `HONDA_38770-MFL-622_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-644_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-671_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-691_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-702_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-741_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-761_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-773_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-861_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-871_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-A21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-D21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-F21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-J21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-J41_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MFL-L21_CBR1000RR_Fireblade_(2008-2011).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFL` |
| `HONDA_38770-MGP-A01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MGP-A92_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MGP-D01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MGP-D62_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MGP-F01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MGP-F63_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MGP-J01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MGP-L01_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MGP-T42_CBR1000RR_Fireblade_(2012-2016).xdf` | `.XDF` | `16,706` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGP` |
| `HONDA_38770-MKF-A22_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKF` |
| `HONDA_38770-MKF-D43_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKF` |
| `HONDA_38770-MKF-D72_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKF` |
| `HONDA_38770-MKF-H11_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKF` |
| `HONDA_38770-MKF-L13_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,711` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKF` |
| `HONDA_38770-MKFA-A22_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,712` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKF` |
| `HONDA_38770-MKFA-D72_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,712` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKF` |
| `HONDA_38770-MKFA-DK2_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | `.XDF` | `16,712` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKF` |

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
