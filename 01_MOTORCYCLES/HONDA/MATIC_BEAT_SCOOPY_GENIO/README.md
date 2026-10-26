# MATIC BEAT SCOOPY GENIO - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/MATIC_BEAT_SCOOPY_GENIO`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `93 files` (0 binary dumps, 93 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MATIC_BEAT_SCOOPY_GENIO` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `GENERATIONAL_30400-K1A-N01_Honda_All_New_Beat_LED_Gen_4_Smart_Key___Alarm_(2024-2026).xdf` | `.XDF` | `5,589` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_30400-K2F-N11_Honda_All_New_Scoopy_Gen_4_Facelift_(2024-2026).xdf` | `.XDF` | `5,581` bytes | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K93-N01_Honda_Scoopy_Ring_12_eSP_Gen_2_(2017-2020).xdf` | `.XDF` | `5,559` bytes | Honda Motorcycle Keihin ECU ROM `38770-K93` |
| `HONDA_30400-K0J-N01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K20J-T21_Zoomer-X_2015-2017_Zoomer-X_(2015-2020).xdf` | `.XDF` | `10,174` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K2F-N11_Scoopy-i_(2021-2024).xdf` | `.XDF` | `16,695` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K2SF-T01_CLICK160_Scoopy-i_(2013-2016).xdf` | `.XDF` | `10,164` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K2TA-T02_LEAD125_4V_Lead_125_4V_(2022-2024).xdf` | `.XDF` | `10,169` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K3MF-T01_GIONRO_125_Giorno+_125_(2023-2024).xdf` | `.XDF` | `10,169` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K93-N01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map |
| `HONDA_30400-K93-T01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | TunerPro Binary Definition Map |
| `HONDA_38770-G90-V02_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-G90` |
| `HONDA_38770-GFM-601_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-GFM` |
| `HONDA_38770-GGE-901_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-GGE` |
| `HONDA_38770-GGE-941_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-GGE` |
| `HONDA_38770-HL6-A05_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-HL6` |
| `HONDA_38770-HR6-MO2_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-HR6` |
| `HONDA_38770-K25-901_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K25` |
| `HONDA_38770-K28-A62_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K28` |
| `HONDA_38770-K2F-N01_Scoopy-i_(2021-2024).xdf` | `.XDF` | `16,695` bytes | Honda Motorcycle Keihin ECU ROM `38770-K2F` |
| `HONDA_38770-K47-M01_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K47` |
| `HONDA_38770-K53-D03_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K53` |
| `HONDA_38770-K53-DB2_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-K53` |
| `HONDA_38770-K76-M02_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K76` |
| `HONDA_38770-K76-T62_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-K76` |
| `HONDA_38770-K87-T52_Rebel_300_(2017-2024).xdf` | `.XDF` | `16,708` bytes | Honda Motorcycle Keihin ECU ROM `38770-K87` |
| `HONDA_38770-K95-A41_Honda_Generic_ECM.xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-K95` |
| `HONDA_38770-K99-B02_Honda_Generic_ECM.xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-K99` |
| `HONDA_38770-KOA-T11_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-KOA` |
| `HONDA_38770-KPG-H01_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-KPG` |
| `HONDA_38770-KTW-903_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-KTW` |
| `HONDA_38770-KTW-B02_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-KTW` |
| `HONDA_38770-KTY-H52_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-KTY` |
| `HONDA_38770-KVK-B31_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-KVK` |
| `HONDA_38770-KWT-703_Honda_Generic_ECM.xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-KWT` |
| `HONDA_38770-KYE-942_Honda_Generic_ECM.xdf` | `.XDF` | `16,696` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYE` |
| `HONDA_38770-KYJ-922_CBR250R_(2011-2014).xdf` | `.XDF` | `16,694` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYJ` |
| `HONDA_38770-KYJ-971_CBR250R_(2011-2014).xdf` | `.XDF` | `16,694` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYJ` |
| `HONDA_38770-KYJ-R11_CBR250R_(2011-2014).xdf` | `.XDF` | `16,694` bytes | Honda Motorcycle Keihin ECU ROM `38770-KYJ` |
| `HONDA_38770-KZL-C31_Spacy-i___Zoomer-X_(2012-2014).xdf` | `.XDF` | `16,709` bytes | Honda Motorcycle Keihin ECU ROM `38770-KZL` |
| `HONDA_38770-KZL-E12_Spacy-i___Zoomer-X_(2012-2014).xdf` | `.XDF` | `16,709` bytes | Honda Motorcycle Keihin ECU ROM `38770-KZL` |
| `HONDA_38770-MCG-602_Honda_Generic_ECM.xdf` | `.XDF` | `16,704` bytes | Honda Motorcycle Keihin ECU ROM `38770-MCG` |
| `HONDA_38770-MEW-D41_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MEW` |
| `HONDA_38770-MFA-D03_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFA` |
| `HONDA_38770-MFG-D02_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFG` |
| `HONDA_38770-MFM-651_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFM` |
| `HONDA_38770-MFM-702_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFM` |
| `HONDA_38770-MFN-D01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFN` |
| `HONDA_38770-MFN-F01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFN` |
| `HONDA_38770-MFR-642_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFR` |
| `HONDA_38770-MFT-642_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MFT` |
| `HONDA_38770-MGC-D32_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGC` |
| `HONDA_38770-MGE-623_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGE` |
| `HONDA_38770-MGE-D01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGE` |
| `HONDA_38770-MGE-D02_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGE` |
| `HONDA_38770-MGE-D41_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGE` |
| `HONDA_38770-MGE-F02_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGE` |
| `HONDA_38770-MGE-F11_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGE` |
| `HONDA_38770-MGF-D12_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGF` |
| `HONDA_38770-MGH-641_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGH` |
| `HONDA_38770-MGH-D21_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGH` |
| `HONDA_38770-MGH-F21_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGH` |
| `HONDA_38770-MGH-M12_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGH` |
| `HONDA_38770-MGH-N12_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGH` |
| `HONDA_38770-MGM-D11_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MGM` |
| `HONDA_38770-MJL-Y11_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MJL` |
| `HONDA_38770-MJP-DA1_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MJP` |
| `HONDA_38770-MKA-D71_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKA` |
| `HONDA_38770-MKG-N52_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKG` |
| `HONDA_38770-MKJ-D02_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-MKJ` |
| `HONDA_38770-N1A-D00_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-N1A` |
| `HONDA_38770-N1A-D11_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-N1A` |
| `HONDA_38770-NLR-B31_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-NLR` |
| `HONDA_38770-NLS-000_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | Honda Motorcycle Keihin ECU ROM `38770-NLS` |
| `Honda_38770-K0J-N01_Genio_256KB.xdf` | `.XDF` | `8,812` bytes | Honda Motorcycle Keihin ECU ROM `38770-K0J` |
| `Honda_38770-K0W-N01_ADV_256KB.xdf` | `.XDF` | `8,794` bytes | Honda Motorcycle Keihin ECU ROM `38770-K0W` |
| `Honda_38770-K15-903_CB150R_64KB.xdf` | `.XDF` | `8,005` bytes | Honda Motorcycle Keihin ECU ROM `38770-K15` |
| `Honda_38770-K15-921_All_256KB.xdf` | `.XDF` | `8,814` bytes | Honda Motorcycle Keihin ECU ROM `38770-K15` |
| `Honda_38770-K16-901_Scoopy_64KB.xdf` | `.XDF` | `8,009` bytes | Honda Motorcycle Keihin ECU ROM `38770-K16` |
| `Honda_38770-K1Z-N01_PCX_256KB.xdf` | `.XDF` | `8,798` bytes | Honda Motorcycle Keihin ECU ROM `38770-K1Z` |
| `Honda_38770-K1Z-N21_PCX_256KB.xdf` | `.XDF` | `8,788` bytes | Honda Motorcycle Keihin ECU ROM `38770-K1Z` |
| `Honda_38770-K20-901_Spacy_64KB.xdf` | `.XDF` | `7,955` bytes | Honda Motorcycle Keihin ECU ROM `38770-K20` |
| `Honda_38770-K25-601_Beat_64KB.xdf` | `.XDF` | `7,985` bytes | Honda Motorcycle Keihin ECU ROM `38770-K25` |
| `Honda_38770-K25-901_Beat_64KB.xdf` | `.XDF` | `8,005` bytes | Honda Motorcycle Keihin ECU ROM `38770-K25` |
| `Honda_38770-K2F-N01_All_256KB.xdf` | `.XDF` | `8,826` bytes | Honda Motorcycle Keihin ECU ROM `38770-K2F` |
| `Honda_38770-K41-N01_Blade_64KB.xdf` | `.XDF` | `7,963` bytes | Honda Motorcycle Keihin ECU ROM `38770-K41` |
| `Honda_38770-K44-V01_Beat_64KB.xdf` | `.XDF` | `8,005` bytes | Honda Motorcycle Keihin ECU ROM `38770-K44` |
| `Honda_38770-K46-N01_Vario_64KB.xdf` | `.XDF` | `7,973` bytes | Honda Motorcycle Keihin ECU ROM `38770-K46` |
| `Honda_38770-K56-N01_Sonic_256KB.xdf` | `.XDF` | `8,816` bytes | Honda Motorcycle Keihin ECU ROM `38770-K56` |
| `Honda_38770-K59-A11_Vario_256KB.xdf` | `.XDF` | `8,790` bytes | Honda Motorcycle Keihin ECU ROM `38770-K59` |
| `Honda_38770-K60-B11_Vario_256KB.xdf` | `.XDF` | `8,790` bytes | Honda Motorcycle Keihin ECU ROM `38770-K60` |
| `Honda_38770-K97-N01_PCX_256KB.xdf` | `.XDF` | `8,790` bytes | Honda Motorcycle Keihin ECU ROM `38770-K97` |
| `Honda_38770-KVG-V42_Vario_64KB.xdf` | `.XDF` | `7,989` bytes | Honda Motorcycle Keihin ECU ROM `38770-KVG` |

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
