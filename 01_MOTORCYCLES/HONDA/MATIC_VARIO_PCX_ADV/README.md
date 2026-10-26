# MATIC VARIO PCX ADV - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/MATIC_VARIO_PCX_ADV`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `33 files` (0 binary dumps, 33 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MATIC_VARIO_PCX_ADV` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `GENERATIONAL_38770-K0W-NA1_Honda_All_New_ADV_160_eSP+_2022_2025.xdf` | `.XDF` | `2,539` bytes | Honda Motorcycle Keihin ECU ROM `38770-K0W` |
| `GENERATIONAL_38770-K1ZG-N21_Honda_All_New_PCX_160_eSP+_Gen_4_2021_2025.xdf` | `.XDF` | `2,546` bytes | Honda Motorcycle Keihin ECU ROM `38770-K1Z` |
| `GENERATIONAL_38770-K2SA-N01_Honda_All_New_Vario_160___Click_160_2022_2025.xdf` | `.XDF` | `2,549` bytes | Honda Motorcycle Keihin ECU ROM `38770-K2S` |
| `GENERATIONAL_38770-K59-A11_Honda_Vario_150_Gen_1_LED_eSP_(2015-2017).xdf` | `.XDF` | `5,563` bytes | Honda Motorcycle Keihin ECU ROM `38770-K59` |
| `GENERATIONAL_38770-K59-A71_Honda_All_New_Vario_150_Gen_2_Keyless_(2018-2022).xdf` | `.XDF` | `5,573` bytes | Honda Motorcycle Keihin ECU ROM `38770-K59` |
| `GENERATIONAL_38770-K60-B01_Honda_Vario_125_Gen_2_LED_eSP_(2015-2017).xdf` | `.XDF` | `5,567` bytes | Honda Motorcycle Keihin ECU ROM `38770-K60` |
| `GENERATIONAL_38770-K60-B61_Honda_All_New_Vario_125_Gen_3_(2018-2022).xdf` | `.XDF` | `5,563` bytes | Honda Motorcycle Keihin ECU ROM `38770-K60` |
| `GENERATIONAL_38770-KZR-601_Honda_Vario_125_Gen_1_Bohlam___Helm-in_(2012-2014).xdf` | `.XDF` | `5,572` bytes | Honda Motorcycle Keihin ECU ROM `38770-KZR` |
| `HONDA_30400-K0WF-T01_ADV150_2017-2019_ADV_150___ADV_160_(2019-2024).xdf` | `.XDF` | `10,181` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K0WF-T01_ADV150_ADV_150___ADV_160_(2019-2024).xdf` | `.XDF` | `10,171` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K0WM-TA1_ADV160_ADV_150___ADV_160_(2019-2024).xdf` | `.XDF` | `10,171` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K1ZF-T01_PCX160_NOABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | `.XDF` | `10,179` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K1ZF-T11_PCX160ABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | `.XDF` | `10,176` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K1ZP-T51_PCX160_NOABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | `.XDF` | `10,179` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K1ZP-T71_PCX160_ABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | `.XDF` | `10,177` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K2VH-T11_CLICK125_2023_Click_125i_(2023-2024).xdf` | `.XDF` | `10,171` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K36F-T01_PCX150_2014-2015_PCX_150_(2014-2017).xdf` | `.XDF` | `10,171` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K36S-T31__PCX150_2016-2017_PCX_150_(2014-2017).xdf` | `.XDF` | `10,172` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K46-N21_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K46-N31_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K46-NA1_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K59K-T11_Click150_2018-2020_Click_150i_(2018-2022).xdf` | `.XDF` | `10,176` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K60F-T01_Click125_2014-2015_Click_125i_LED_(2018-2022).xdf` | `.XDF` | `10,180` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K60S-T71_Click125_2016-2017_Click_125i_LED_(2018-2022).xdf` | `.XDF` | `10,180` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K97F-T_PCX150_2017-2019_PCX_150_Smart_Key_(2018-2020).xdf` | `.XDF` | `10,181` bytes | TunerPro Binary Definition Map |
| `HONDA_38770-K46-N01_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K46` |
| `HONDA_38770-KVG-V42_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-KVG` |
| `HONDA_38770-MKH-C02_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKH` |
| `HONDA_38770-MKH-C03_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKH` |
| `HONDA_38770-MKH-D01_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKH` |
| `HONDA_38770-MKH-D22_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKH` |
| `HONDA_38770-MKH-D23_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKH` |
| `HONDA_38770-MKH-D42_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | `.XDF` | `16,717` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKH` |

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
