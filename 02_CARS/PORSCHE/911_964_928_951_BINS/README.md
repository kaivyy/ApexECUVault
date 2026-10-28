# 911_964_928_951_BINS - ECU Calibration Suite

**Repository Path**: `02_CARS/PORSCHE/911_964_928_951_BINS`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `10 files` (10 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `911_964_928_951_BINS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1984–1994

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `0280 002 506_89_90_928GT.bin` | **1989–1990** | 16.0 KB | `a42f8772f60b5349d465505f92808e21` | Factory Binary Firmware Dump |
| `1992_964C2_181240302612004.bin` | **1992** | 32.0 KB | `4a80379710ad06693272201065435fd1` | Factory Binary Firmware Dump |
| `84 Carrera OE EUR 1267355099.BIN` | **1984** | 2.0 KB | `06ef03234fc31811452f6b858a6da12e` | Factory Binary Firmware Dump |
| `84 Carrera OE USA 1267355102.BIN` | **1984** | 2.0 KB | `42da250a6baea01947a93d296a2e9b01` | Factory Binary Firmware Dump |
| `86 Carrera OE EUR 1267355027.BIN` | **1986** | 4.0 KB | `838570336bf5296e7fcccf58bc0b61f1` | Factory Binary Firmware Dump |
| `86 Carrera OE USA 1267355180.BIN` | **1986** | 4.0 KB | `a93082beaf43be3062ceea3eb718d600` | Factory Binary Firmware Dump |
| `87 Carrera OE USA 1267355236.BIN` | **1987** | 4.0 KB | `65e847abf81cd3b82d1ef666c9513aca` | Factory Binary Firmware Dump |
| `Porsche951DME24pin.bin` | **1984–1994** | 4.0 KB | `b1f78205c945d31bb8aade9a93ed3291` | Factory Binary Firmware Dump |
| `Porsche951DME28pin.BIN` | **1984–1994** | 8.0 KB | `ea9d6a82002b68d0b03229c535ce6c4b` | Factory Binary Firmware Dump |
| `gt-91_0280.002.509.bin` | **1984–1994** | 32.0 KB | `98b96e6d79eb8f8f31219aac0967ac65` | Factory Binary Firmware Dump |

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
