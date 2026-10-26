# ImperialUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Generic/ImperialUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `35 files` (0 binary dumps, 35 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ImperialUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2015–2026

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `R0C9J8B2B_3081-080_017_002.ImperialUnits.xdf` | **2015–2026** | 973.3 KB | `fb04481bee5b4f0dcb9eab2743a31d53` | TunerPro Binary Definition Map |
| `R0C9J8D2B_3081-080_021_002.ImperialUnits.xdf` | **2015–2026** | 973.3 KB | `ad7b0c74b77e634ffe9b664eb3252780` | TunerPro Binary Definition Map |
| `R0C9J8I2B_3081-080_029_002.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `df13011e8e72d888d07e3aee1b1eecf9` | TunerPro Binary Definition Map |
| `R0C9J8I3B_3081-080_029_003.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `df13011e8e72d888d07e3aee1b1eecf9` | TunerPro Binary Definition Map |
| `R0C9J8I4B_3081-080_029_004.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `df13011e8e72d888d07e3aee1b1eecf9` | TunerPro Binary Definition Map |
| `R0C9J962B_3081-090_010_002.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `5143641a5eb6378a5538f11faf70b6d5` | TunerPro Binary Definition Map |
| `R0C9J9E3B_3081-090_020_003.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `f956ef27196bf4ca821d45cb380672ba` | TunerPro Binary Definition Map |
| `R0C9J9E4B_3081-090_020_004.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `eb4b177a8d2c4fbc6208b10c8ce13752` | TunerPro Binary Definition Map |
| `R0C9JA05B_3081-090_025_005.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `e440263ffe72bf9a990042eea819f682` | TunerPro Binary Definition Map |
| `R0C9JA15B_3081-090_030_005.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `81fc84d2ed9da297ce9b5f86eed6ae5b` | TunerPro Binary Definition Map |
| `R0C9JC05B_3081-090_050_005.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `4ad7e40957f33456308b586964f7fe27` | TunerPro Binary Definition Map |
| `R0C9JD06B_3081-090_060_006.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `1481d38a263043f3ff3dd049d9ab15bf` | TunerPro Binary Definition Map |
| `R0C9JE15B_3081-090_080_005.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `86d2fdb69d88da5c57778d99cf16be49` | TunerPro Binary Definition Map |
| `R0R96015B_7706-000_007_005.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `86cc0122444f3c8af44130b6e739dcf4` | TunerPro Binary Definition Map |
| `R0R96025B_7706-000_008_005.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `86cc0122444f3c8af44130b6e739dcf4` | TunerPro Binary Definition Map |
| `R0R9A005B_7706-000_011_005.ImperialUnits.xdf` | **2015–2026** | 973.2 KB | `21faa6a1eecc860414ed6813549128c4` | TunerPro Binary Definition Map |
| `R1C9I562B_3076-050_006_002.ImperialUnits.xdf` | **2015–2026** | 904.5 KB | `d72b59d37fedb9f027c58736b6899f21` | TunerPro Binary Definition Map |
| `R1C9J772B_3076-070_009_002.ImperialUnits.xdf` | **2015–2026** | 961.2 KB | `cfedc7671d670586037ee21d1192b35f` | TunerPro Binary Definition Map |
| `R1C9J8B2B_3076-080_017_002.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `822c18128e7554ab04bca1b123921652` | TunerPro Binary Definition Map |
| `R1C9J8B3B_3076-080_017_003.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `822c18128e7554ab04bca1b123921652` | TunerPro Binary Definition Map |
| `R1C9J8D3B_3076-080_018_003.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `822c18128e7554ab04bca1b123921652` | TunerPro Binary Definition Map |
| `R1C9J8G3B_3428-000_001_001.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `46ea4d04e58cbd7495ecb70c21cdc0f5` | TunerPro Binary Definition Map |
| `R1C9J8I2B_3076-080_029_002.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `0eb00459f7abefee8df10e399fbd42ac` | TunerPro Binary Definition Map |
| `R1C9J8I7B_3076-080_029_007.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `0eb00459f7abefee8df10e399fbd42ac` | TunerPro Binary Definition Map |
| `R1C9J962B_3076-090_010_002.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `b0d390f82cedb7105504fc9de1bf5adf` | TunerPro Binary Definition Map |
| `R1C9J9E3B_3076-090_020_003.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `90d8aa37e927aea554558b3de9c25b27` | TunerPro Binary Definition Map |
| `R1C9J9E5B_3076-090_020_005.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `84c2d4025fd8db06fc4ffcccf98b080d` | TunerPro Binary Definition Map |
| `R1C9J9E7B_3076-090_020_007.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `90d8aa37e927aea554558b3de9c25b27` | TunerPro Binary Definition Map |
| `R1C9JA05B_3076-090_025_005.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `c7af8ea90f8a658565b3ceba6954ae4c` | TunerPro Binary Definition Map |
| `R1C9JC05B_3076-090_050_005.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `78e632f4e711b87d9c067dfe53795753` | TunerPro Binary Definition Map |
| `R1C9JD06B_3076-090_060_006.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `0bda5c3719923912748840e3c0b8f900` | TunerPro Binary Definition Map |
| `R1C9JE15B_3076-090_080_005.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `6b83367db49d3ac0b4c53522fcb9f9fe` | TunerPro Binary Definition Map |
| `R1R95005B_7972-000_005_005.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `1c1fe647f5abcadde5c966caf054873f` | TunerPro Binary Definition Map |
| `R1R96015B_7972-000_007_005.ImperialUnits.xdf` | **2015–2026** | 972.7 KB | `12ee0e824a78c5680a454ee2c7beeb88` | TunerPro Binary Definition Map |
| `V0C9J6J2B_3125-065_027_002.ImperialUnits.xdf` | **2015–2026** | 824.6 KB | `1d894c207e1ad4e4dc4d17caa8a4f914` | TunerPro Binary Definition Map |

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
