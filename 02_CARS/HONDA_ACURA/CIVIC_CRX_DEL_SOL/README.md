# CIVIC_CRX_DEL_SOL - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CIVIC_CRX_DEL_SOL`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `34 files` (34 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CIVIC_CRX_DEL_SOL` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1988–2000

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `303stock-P07-D15Z1.bin` | **1988–2000** | 32.0 KB | `d6dd4447fb8a03ad590e8c99f73ad058` | Factory Binary Firmware Dump |
| `317P28-G02-317.bin` | **1988–2000** | 32.0 KB | `1f19363633928c6de9924ea07d619a2d` | Factory Binary Firmware Dump |
| `327stock-P28auto.bin` | **1988–2000** | 32.0 KB | `21ce5cd331bd6dc280d24c873ea5a408` | Factory Binary Firmware Dump |
| `37820-P28-L50.bin` | **1988–2000** | 32.0 KB | `0c3d023bbafe66737be7bdc609ac8038` | Factory Binary Firmware Dump |
| `Civ328ex.bin` | **1988–2000** | 48.0 KB | `eb6b8cbde8b0273af8f68bae40eb74f7` | Factory Binary Firmware Dump |
| `Civ409ex.bin` | **1988–2000** | 48.0 KB | `8921140d8bf9bdc7b483691e2a140e65` | Factory Binary Firmware Dump |
| `Civ471hx.bin` | **1988–2000** | 48.0 KB | `422ab5f5ca5ed8f525a356f1a6fdef02` | Factory Binary Firmware Dump |
| `JDMP30_932_311code.bin` | **1988–2000** | 32.0 KB | `5908c371829e31bb063d36c07643a60c` | Factory Binary Firmware Dump |
| `OKI_P30.BIN` | **1988–2000** | 64.0 KB | `085cd4fb63be2490b928bae47956b1aa` | Factory Binary Firmware Dump |
| `P07-225--.bin` | **1988–2000** | 32.0 KB | `dc05136bf8db72727f3e1dabf9924f8d` | Factory Binary Firmware Dump |
| `P07-900-262MCU.bin` | **1988–2000** | 32.0 KB | `8b6e680af52cb1e6da426c1c769c229b` | Factory Binary Firmware Dump |
| `P08-001-237.bin` | **1988–2000** | 32.0 KB | `5922763665fb28ac0f1d16c7964668ae` | Factory Binary Firmware Dump |
| `P08-900AT.bin` | **1988–2000** | 32.0 KB | `fcb15e625afd689e1e176b6ceccb7a6f` | Factory Binary Firmware Dump |
| `P28-230.bin` | **1988–2000** | 32.0 KB | `b195802e78440afb9b54d13b93092dc9` | Factory Binary Firmware Dump |
| `P30USDMCivicD16Y8203.BIN` | **1988–2000** | 32.0 KB | `569a4893fbb945b1ecaabe33d8db4d5b` | Factory Binary Firmware Dump |
| `P30_G00_209_EDM.bin` | **1988–2000** | 32.0 KB | `024963da241d63f031b95ddf172259e8` | Factory Binary Firmware Dump |
| `PM6-A09-65.bin` | **1988–2000** | 17.0 KB | `0f604953c5b5c9b1397370e9a1afc0ef` | Factory Binary Firmware Dump |
| `STOCK-PM6.bin` | **1988–2000** | 32.0 KB | `3f3a974071ce4db7cfa240ab8475e82b` | Factory Binary Firmware Dump |
| `Stock_P30-901_AT.bin` | **1988–2000** | 32.0 KB | `d1f10e324f1ca1363ee715532b9bea2a` | Factory Binary Firmware Dump |
| `d16a8_stock.BIN` | **1988–2000** | 32.0 KB | `5f1d1086c5c52f1350fe2d14bf5b6eb6` | Factory Binary Firmware Dump |
| `orgasm_p28.bin` | **1988–2000** | 32.0 KB | `04828f6f92ef329c60d7345314743660` | Factory Binary Firmware Dump |
| `p05-USDM-231.bin` | **1988–2000** | 32.0 KB | `04dad6c089c1a7c58b5ca013eea13276` | Factory Binary Firmware Dump |
| `p06-301.bin` | **1988–2000** | 32.0 KB | `f5ce8bccf7dad248ec25bf590c9bbd3c` | Factory Binary Firmware Dump |
| `p06-import-only.bin` | **1988–2000** | 32.0 KB | `2c1af6d8d5af757145521578c9df6816` | Factory Binary Firmware Dump |
| `p06-q00-314.bin` | **1988–2000** | 32.0 KB | `dd26dbb335385fa52083db2482a355c7` | Factory Binary Firmware Dump |
| `p07-g01-218.bin` | **1988–2000** | 32.0 KB | `da5999e3a3db965227668fbed357f8a2` | Factory Binary Firmware Dump |
| `p07-g01-252.bin` | **1988–2000** | 32.0 KB | `e52a045ac65fab0e7666fd8d8a8c8047` | Factory Binary Firmware Dump |
| `p08-911-243.bin` | **1988–2000** | 32.0 KB | `e5585298f3e8376d10e698ea1209183e` | Factory Binary Firmware Dump |
| `p08-n01-283.bin` | **1988–2000** | 32.0 KB | `de890d2a9937ab924872fec8d1b778ae` | Factory Binary Firmware Dump |
| `p28-q50-315.bin` | **1988–2000** | 32.0 KB | `274c6d1ce78ec8c6f2c12de944c5b3fa` | Factory Binary Firmware Dump |
| `p30-010-244MCU-extensionG8.bin` | **1988–2000** | 31.2 KB | `507809b191089616af10682da0d3a602` | Factory Binary Firmware Dump |
| `p30-900JDM-AT.bin` | **1988–2000** | 32.0 KB | `b35c0513533cb6053188f42867a5c188` | Factory Binary Firmware Dump |
| `p30-j00-240.bin` | **1988–2000** | 32.0 KB | `e4c067a77766b30b448c8d8f399c4776` | Factory Binary Firmware Dump |
| `pm6ng_stable.bin` | **1988–2000** | 32.0 KB | `a042605ef346210bb76decaf788fe701` | Factory Binary Firmware Dump |

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
