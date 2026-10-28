# DELPHI_DYNO_TUNES - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HARLEY_DAVIDSON_INDIAN/DELPHI_DYNO_TUNES`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `33 files` (33 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `DELPHI_DYNO_TUNES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233.ori` | **2000–2024** | 164.2 KB | `2147e2e74b8e1cf2d1f47e342778cb50` | Factory Binary Firmware Dump |
| `1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233new.ori` | **2000–2024** | 192.2 KB | `a594a4e9fef8b38aab467f23e48c27c6` | Factory Binary Firmware Dump |
| `1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233rk.ori` | **2000–2024** | 187.2 KB | `0ffa0e5089113274bdd5c102a4998da2` | Factory Binary Firmware Dump |
| `1HD1HBZ115K802247_32498-05_127_0000000201_1328.ori` | **2000–2024** | 66.4 KB | `feb93f04caa240811d5ad3bffd200eb4` | Factory Binary Firmware Dump |
| `1HD1KTC37JB676262_RadioInfo.bin` | **2000–2024** | 20 B | `53ef49e3e766ae1fff22aced897b50b0` | Factory Binary Firmware Dump |
| `1HD1KTM12FB697962_41000057_617_0004080F01_2233.ori` | **2000–2024** | 164.2 KB | `f7bd9ec56b08c8e4b406b1e02e88f509` | Factory Binary Firmware Dump |
| `1HD1KTP27LB649034_RadioInfo.bin` | **2000–2024** | 20 B | `53ef49e3e766ae1fff22aced897b50b0` | Factory Binary Firmware Dump |
| `1HD1KTP3XKB630226_RadioInfo.bin` | **2000–2024** | 20 B | `60ba11769461681a358280c08a45dcd0` | Factory Binary Firmware Dump |
| `AmericanSpeed_-_Delfi_Centurion_blue flhx.ori` | **2000–2024** | 64.4 KB | `bf64a14c3c16f2a0e3921b38bc94a649` | Factory Binary Firmware Dump |
| `BigBaggerBonzai_-_Delfi_Centurion_ed h.ori` | **2000–2024** | 164.2 KB | `69aeff041af197aa2796e7f71d167f74` | Factory Binary Firmware Dump |
| `BigBaggerBonzai_-_Delfi_Centurion_ed.ori` | **2000–2024** | 108.3 KB | `5ecd86222d24599f1345886ec065b45b` | Factory Binary Firmware Dump |
| `BigBerthaWorthit-_-_Delfi_Centurion_CenturionIntRegistration.bin` | **2000–2024** | 700 B | `adc415418ac230b7fa197511ac6f29e4` | Factory Binary Firmware Dump |
| `BigBerthaWorthit-_-_Delfi_Centurion_beeneychinswap.ori` | **2000–2024** | 164.2 KB | `b6acb177369bd521bc96b56abf8f410f` | Factory Binary Firmware Dump |
| `BigBerthaWorthit-_-_Delfi_Centurion_beeneyswap2.ori` | **2000–2024** | 164.2 KB | `733b24057aee4594df5c37a59ac9242e` | Factory Binary Firmware Dump |
| `BigBerthaWorthit-_-_Delfi_Centurion_chin.ori` | **2000–2024** | 88.2 KB | `48f9fef2ac80a6d9dbfd70ead9f507ee` | Factory Binary Firmware Dump |
| `CenturionIntRegistration.bin` | **2000–2024** | 700 B | `adc415418ac230b7fa197511ac6f29e4` | Factory Binary Firmware Dump |
| `DontFugganDieDarleeng_-_Delfi_Centurion_1HD1KTM12FB697962_41000057_617_0004080F01_2233.ori` | **2000–2024** | 164.2 KB | `f7bd9ec56b08c8e4b406b1e02e88f509` | Factory Binary Firmware Dump |
| `FatTireFelisha_-_Delfi_Centurion_1HD1HBZ115K802247_32498-05_127_0000000201_1328.ori` | **2000–2024** | 66.4 KB | `feb93f04caa240811d5ad3bffd200eb4` | Factory Binary Firmware Dump |
| `GaggBaggerGertruude_-_Delfi_Centurion_1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233.ori` | **2000–2024** | 164.2 KB | `2147e2e74b8e1cf2d1f47e342778cb50` | Factory Binary Firmware Dump |
| `GaggBaggerGertruude_-_Delfi_Centurion_1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233new.ori` | **2000–2024** | 192.2 KB | `a594a4e9fef8b38aab467f23e48c27c6` | Factory Binary Firmware Dump |
| `GaggBaggerGertruude_-_Delfi_Centurion_1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233rk.ori` | **2000–2024** | 187.2 KB | `0ffa0e5089113274bdd5c102a4998da2` | Factory Binary Firmware Dump |
| `GaggBaggerGertruude_-_Delfi_Centurion_jayder.ori` | **2000–2024** | 183.1 KB | `b5959a586ebc016e0a279c3c1beb8c2d` | Factory Binary Firmware Dump |
| `HorsePowerbySurina_-_Delfi_Centurion_rodney rg.ori` | **2000–2024** | 66.4 KB | `5d5dcf836dd961602fa02e390a66666e` | Factory Binary Firmware Dump |
| `Lil-Susie_-_Delfi_Centurion_streetglide.ori` | **2000–2024** | 66.4 KB | `65824d097744a13342b1a0d570178abf` | Factory Binary Firmware Dump |
| `beeneychinswap.ori` | **2000–2024** | 164.2 KB | `b6acb177369bd521bc96b56abf8f410f` | Factory Binary Firmware Dump |
| `beeneyswap2.ori` | **2000–2024** | 164.2 KB | `733b24057aee4594df5c37a59ac9242e` | Factory Binary Firmware Dump |
| `blue flhx.ori` | **2000–2024** | 64.4 KB | `bf64a14c3c16f2a0e3921b38bc94a649` | Factory Binary Firmware Dump |
| `chin.ori` | **2000–2024** | 88.2 KB | `48f9fef2ac80a6d9dbfd70ead9f507ee` | Factory Binary Firmware Dump |
| `ed h.ori` | **2000–2024** | 164.2 KB | `69aeff041af197aa2796e7f71d167f74` | Factory Binary Firmware Dump |
| `ed.ori` | **2000–2024** | 108.3 KB | `5ecd86222d24599f1345886ec065b45b` | Factory Binary Firmware Dump |
| `jayder.ori` | **2000–2024** | 183.1 KB | `b5959a586ebc016e0a279c3c1beb8c2d` | Factory Binary Firmware Dump |
| `rodney rg.ori` | **2000–2024** | 66.4 KB | `5d5dcf836dd961602fa02e390a66666e` | Factory Binary Firmware Dump |
| `streetglide.ori` | **2000–2024** | 66.4 KB | `65824d097744a13342b1a0d570178abf` | Factory Binary Firmware Dump |

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
