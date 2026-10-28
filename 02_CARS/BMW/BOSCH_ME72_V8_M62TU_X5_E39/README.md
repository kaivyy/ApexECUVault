# BOSCH_ME72_V8_M62TU_X5_E39 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/BOSCH_ME72_V8_M62TU_X5_E39`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `13 files` (8 binary dumps, 5 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `BOSCH_ME72_V8_M62TU_X5_E39` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1998–2004

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `5A01_1999_540i_DME72_64K_DUMP.bin` | **1999** | 64.0 KB | `b510dc32f18a603290fd76b504fc2a77` | Factory Binary Firmware Dump |
| `5a01.smalltable.winfkptest.bin` | **1998–2004** | 64.0 KB | `0098ab96b9854e39b040f31ace83342a` | Factory Binary Firmware Dump |
| `5a01.withsmalltables.bin` | **1998–2004** | 64.0 KB | `00295dfdedaa115201ba1aebb1047a40` | Factory Binary Firmware Dump |
| `5a01_7539336.bin` | **1998–2004** | 64.0 KB | `22e6f59279d052c9505361a1c9af67bb` | Factory Binary Firmware Dump |
| `6902.6901_64kb.bin` | **1998–2004** | 64.0 KB | `2ad41416aaff86343179e347ed617484` | Factory Binary Firmware Dump |
| `E5A0_000.a2l` | **1998–2004** | 3.95 MB | `a5db741e481530c58b4c576fad38685f` | ASAM ASAP2 ECU Description File |
| `E650_000.a2l` | **1998–2004** | 3.45 MB | `764c6a53a64faffc6ba97fc13986ff69` | ASAM ASAP2 ECU Description File |
| `Me7.2_m62tub44_e53.bin` | **1998–2004** | 64.0 KB | `a0fd5eb233c3557f1f485c89d86f6d0c` | Factory Binary Firmware Dump |
| `Stage 2 X5 4.6is.Bin` | **1998–2004** | 64.0 KB | `07ca43476a21a1ecc3db87576fb310bc` | Factory Binary Firmware Dump |
| `X5dam.ols` | **1998–2004** | 1.51 MB | `e2bf27cbdc8056847f8d1e1ae339c938` | WinOLS Project Workspace |
| `e18_000.dam` | **1998–2004** | 1.31 MB | `2a13b056713f3747833044f58f48021b` | WinOLS DAMOS Definition Map |
| `e18_0001.dam` | **1998–2004** | 1.32 MB | `a90ad4590fd82c419b27269b7d790a03` | WinOLS DAMOS Definition Map |
| `x5.bin` | **1998–2004** | 64.0 KB | `a97d69fd007d83fc3159681e5fcd875a` | Factory Binary Firmware Dump |

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
