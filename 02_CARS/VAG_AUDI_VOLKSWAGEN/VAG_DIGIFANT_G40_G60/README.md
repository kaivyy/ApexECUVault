# VAG_DIGIFANT_G40_G60 - ECU Calibration Suite

**Repository Path**: `02_CARS/VAG_AUDI_VOLKSWAGEN/VAG_DIGIFANT_G40_G60`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `27 files` (18 binary dumps, 9 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `VAG_DIGIFANT_G40_G60` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1988–1995

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `G40_EubelTuningInGifhorn1995_MinorFuelTimingChanges_BoostCutRemoval_IdleIgnition.BIN` | **1995** | 32.0 KB | `b087e9145ee7e845170f1212dc0406d6` | Factory Binary Firmware Dump |
| `G40_Mk2_StockEprom.BIN` | **1988–1995** | 32.0 KB | `850a8115213f1e378f5d104f293732bd` | Factory Binary Firmware Dump |
| `G40_Mk2_StockEprom.xdf` | **1988–1995** | 18.2 KB | `770f01aa4742df8591f1762b41bd177d` | TunerPro Binary Definition Map |
| `G40_Pitstop_SNS_NoLag_250ccMinInj_7800Rev_AdvIgn_DecFuel72pcDuty.BIN` | **1988–1995** | 32.0 KB | `74fcdfe56695d13a13283eaf51db48a0` | Factory Binary Firmware Dump |
| `G40_Pitstop_SNS_NoLag_7800RevLimit_AdvIgn_IncFuel88pcDuty.BIN` | **1988–1995** | 32.0 KB | `a056503ee2c35f515f680f304971ceec` | Factory Binary Firmware Dump |
| `G40_StockEprom.BIN` | **1988–1995** | 32.0 KB | `5fa2b4c8e2ed78c2cb352fda4a49ede8` | Factory Binary Firmware Dump |
| `G40_StockEprom_with7kRevLimit.BIN` | **1988–1995** | 32.0 KB | `c00210fcafc0bc7eb200edce4b5d2019` | Factory Binary Firmware Dump |
| `G40_StockEprom_withWOTidleLambdaMods.BIN` | **1988–1995** | 32.0 KB | `1fb7b65bbef0015091a59380898e6ddc` | Factory Binary Firmware Dump |
| `G40_XDF_BETA_DirectFromEcuConnections.xdf` | **1988–1995** | 54.6 KB | `276e1388a5c58c0ad6c38e58f5714b07` | TunerPro Binary Definition Map |
| `G40_XDF_YOU54F.xdf` | **1988–1995** | 71.1 KB | `ba9a61530caf4409343243ac81ac332a` | TunerPro Binary Definition Map |
| `G40_XDF_YOU54F_withPatches.xdf` | **1988–1995** | 74.0 KB | `753fe2ae3073bb0ba93027e2ea9e8087` | TunerPro Binary Definition Map |
| `G60 6636 X3 timing bin-ISV boost & no lambda.bin` | **1988–1995** | 32.0 KB | `43fdef17095f4089e724e79da1388182` | Factory Binary Firmware Dump |
| `G60 Single Timing Map01.xdf` | **1988–1995** | 118.8 KB | `bc71b95fe9652afa2c0cffcd79b188ae` | TunerPro Binary Definition Map |
| `G60_1_ignition_map.xdf` | **1988–1995** | 97.3 KB | `ded6b004b5a2bb57e466a2ccd5e6eb1e` | TunerPro Binary Definition Map |
| `KRTURBO.BIN` | **1988–1995** | 32.0 KB | `1cbfe69875c2836530c6e1a52f317dba` | Factory Binary Firmware Dump |
| `PASSG60.BIN` | **1988–1995** | 32.0 KB | `889dc98df8ec41eb25b7949bbf509eb4` | Factory Binary Firmware Dump |
| `STAGE 5 G60.BIN` | **1988–1995** | 32.0 KB | `bcf9c8acc41a18f3a497e1d8f1722dc2` | Factory Binary Firmware Dump |
| `Saab900T16_Bosch403.BIN` | **1988–1995** | 32.0 KB | `d5e2029e3fdf96b059c2519ab9cbe316` | Factory Binary Firmware Dump |
| `Stock G60 Single Ignition Map.BIN` | **1988–1995** | 32.0 KB | `4120071750a1fcc7bd168bde50f097f4` | Factory Binary Firmware Dump |
| `Stock G60 Three ignition maps.bin` | **1988–1995** | 32.0 KB | `b6a425bd3be51763a0d3e0ec3c82a8c1` | Factory Binary Firmware Dump |
| `Theibach RS G60 mit 27c512 gelesen.bin` | **1988–1995** | 32.0 KB | `0b53a1ba5b54939ef8a7f6628d1e4664` | Factory Binary Firmware Dump |
| `TunerPro RT v5 - G60 3 Ignition Map (Marc G60T 2014).xdf` | **2014** | 79.2 KB | `c5e77712b15c8cbb50ae16d13f5864fd` | TunerPro Binary Definition Map |
| `VW 1.3 G40 Digifant-WINOLS-YOU54F.ols` | **1988–1995** | 103.9 KB | `c213d35775f6e8945971549ac1134e18` | WinOLS Project Workspace |
| `VW 1.8T G60 Digifant 037997022B - WINOLS.ols` | **1988–1995** | 57.7 KB | `26f072899b84a8961a854c823e30e493` | WinOLS Project Workspace |
| `corradoSLS.BIN` | **1988–1995** | 32.0 KB | `117ed6deef20eae56fd15afb5d26b40c` | Factory Binary Firmware Dump |
| `limited_16v_G60.BIN` | **1988–1995** | 32.0 KB | `fb9fdfd87443f234bfa73d5a919ba2e0` | Factory Binary Firmware Dump |
| `vw6636.bin` | **1988–1995** | 32.0 KB | `2e5b172c3283cb842ca8f25a56f5ba38` | Factory Binary Firmware Dump |

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
