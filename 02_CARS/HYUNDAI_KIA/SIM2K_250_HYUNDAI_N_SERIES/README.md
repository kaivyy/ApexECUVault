# SIM2K_250_HYUNDAI_N_SERIES - ECU Calibration Suite

**Repository Path**: `02_CARS/HYUNDAI_KIA/SIM2K_250_HYUNDAI_N_SERIES`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `18 files` (9 binary dumps, 9 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SIM2K_250_HYUNDAI_N_SERIES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `CNNKKM___TAA.xdf` | **2000–2024** | 2.32 MB | `b91db0175f30c69b20bad65bc33760be` | TunerPro Binary Definition Map |
| `CNPNKM__FT5A.xdf` | **2000–2024** | 9.08 MB | `74b075e1bb7259c6bce0a4b55cf1b935` | TunerPro Binary Definition Map |
| `CNPNKM___T3A.xdf` | **2000–2024** | 4.72 MB | `5e1296d84d3e336eb14880cef1dfc2ce` | TunerPro Binary Definition Map |
| `CPQDDGMCXXXSDU50.xdf` | **2000–2024** | 4.70 MB | `978a94a28612493d48c962bdc4db44f9` | TunerPro Binary Definition Map |
| `CPQWDEMCXXXSDU50.xdf` | **2000–2024** | 4.84 MB | `db9416720eb6f49ce1b8973e91649570` | TunerPro Binary Definition Map |
| `CPQWDGMCXXXSDU50D.xdf` | **2000–2024** | 4.81 MB | `386b0ebd0b39d554b700c69393d28de1` | TunerPro Binary Definition Map |
| `JSNNJMK__S2A.xdf` | **2000–2024** | 2.68 MB | `094bdbdd1eebfc3e45b68e0ddd0f787a` | TunerPro Binary Definition Map |
| `JSNNKMK__S2A.xdf` | **2000–2024** | 2.68 MB | `094bdbdd1eebfc3e45b68e0ddd0f787a` | TunerPro Binary Definition Map |
| `OSPNKM___T3A.xdf` | **2000–2024** | 5.06 MB | `e792e43e5063fe2547db12e291eaa9a8` | TunerPro Binary Definition Map |
| `Original [CNNKKM___TAA].bin` | **2000–2024** | 2.50 MB | `18b3a80d4ee30a72359024cc04e7dc3d` | Factory Binary Firmware Dump |
| `Original [CNPNKM__FT5A].bin` | **2000–2024** | 2.50 MB | `fa8e82f5c93e7093a84989fdce923d85` | Factory Binary Firmware Dump |
| `Original [CNPNKM___T3A].bin` | **2000–2024** | 2.50 MB | `5fc637fa118a2c7cba3cd9a839ffbe15` | Factory Binary Firmware Dump |
| `Original [CPQDDGMCXXXSDU50].bin` | **2000–2024** | 2.63 MB | `cea0ee75701130e02dd265290459efaf` | Factory Binary Firmware Dump |
| `Original [CPQWDEMCXXXSDU50].bin` | **2000–2024** | 2.50 MB | `d5acf9672f8db1d797a58837b32d8985` | Factory Binary Firmware Dump |
| `Original [CPQWDGMCXXXSDU50D].bin` | **2000–2024** | 2.50 MB | `f412645ab38dbbbd17cdbde2f9fbb74a` | Factory Binary Firmware Dump |
| `Original [JSNNJMK__S2A].bin` | **2000–2024** | 2.50 MB | `b98d26833e8873b4c0850a671e05e511` | Factory Binary Firmware Dump |
| `Original [JSNNKMK__S2A].bin` | **2000–2024** | 2.50 MB | `9df768ad6214d2ef1ed54dfe25ecce1a` | Factory Binary Firmware Dump |
| `Original [OSPNKM___T3A].bin` | **2000–2024** | 2.50 MB | `df6d746810819071b0a64c89c80ddf2a` | Factory Binary Firmware Dump |

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
