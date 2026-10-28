# MUSTANG_FALCON_XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/FORD/MUSTANG_FALCON_XDFS`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `19 files` (4 binary dumps, 15 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MUSTANG_FALCON_XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `6DFC.bin` | **2000–2024** | 256.0 KB | `2767e7e30e0652a9e795cfb5b409e982` | Factory Binary Firmware Dump |
| `6DFD.bin` | **2000–2024** | 256.0 KB | `cb30e24470eb6d6725792135e5d906d4` | Factory Binary Firmware Dump |
| `6DGC.bin` | **2000–2024** | 256.0 KB | `113db590ff6234de01d3ef3df75bd96d` | Factory Binary Firmware Dump |
| `6DGD.bin` | **2000–2024** | 256.0 KB | `90bbde737a318cdfcbb352e22e14c868` | Factory Binary Firmware Dump |
| `CBAZA.xdf` | **2000–2024** | 309.9 KB | `dc4628312362aa97968951d40fc5891d` | TunerPro Binary Definition Map |
| `CDAN4.xdf` | **2000–2024** | 168.7 KB | `5e134df0c835951cd23c969d405d9d6c` | TunerPro Binary Definition Map |
| `CRAJ0.xdf` | **2000–2024** | 210.7 KB | `00a2acf2a4905fd93bf8c95119e4148e` | TunerPro Binary Definition Map |
| `GUF1.xdf` | **2000–2024** | 481.7 KB | `32e206fb24fe927cf56cdf1acd4e9f79` | TunerPro Binary Definition Map |
| `GUFA.xdf` | **2000–2024** | 483.4 KB | `28d3c5bdf66182cff4b39850ebd44814` | TunerPro Binary Definition Map |
| `GUFB.xdf` | **2000–2024** | 485.1 KB | `f5b62ef9f570031f3f6f79cd05f58e79` | TunerPro Binary Definition Map |
| `HWAD3.xdf` | **2000–2024** | 43.1 KB | `9299466a21a1d47cdcfcfc831dd60337` | TunerPro Binary Definition Map |
| `IAW045_06.xdf` | **2000–2024** | 38.7 KB | `08427cd629463934008d86803e9e076f` | TunerPro Binary Definition Map |
| `IAW045_L01.xdf` | **2000–2024** | 39.1 KB | `35dacdb6094f23237b1def5e86a483db` | TunerPro Binary Definition Map |
| `L8edited1.0.xdf` | **2000–2024** | 73.0 KB | `dc3049c4a7ecc85e10cb063d3f15706a` | TunerPro Binary Definition Map |
| `LUX0.xdf` | **2000–2024** | 365.5 KB | `af55aa33baf0c13abedfebb4be45a3cf` | TunerPro Binary Definition Map |
| `N4AGB.xdf` | **2000–2024** | 68.0 KB | `8f4ba768f3f2166bc94447714611b829` | TunerPro Binary Definition Map |
| `NVMG8.xdf` | **2000–2024** | 402.2 KB | `2b4cff99e5ae3571d05a455074577895` | TunerPro Binary Definition Map |
| `P8_research_ver2.0.xdf` | **2000–2024** | 133.8 KB | `13513b416889c1c1e5c3c07d373f3b70` | TunerPro Binary Definition Map |
| `T23B.xdf` | **2000–2024** | 216.3 KB | `d538b0867b73e1afeff6f807f6c228e8` | TunerPro Binary Definition Map |

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
