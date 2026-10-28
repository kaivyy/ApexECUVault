# M_POWER_MSS60_M3_V8 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_MSS60_M3_V8`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `19 files` (14 binary dumps, 5 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `M_POWER_MSS60_M3_V8` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2007–2013

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `BMW M3 - SIEMENS MSS60.ols` | **2007–2013** | 3.72 MB | `7b703832b6985f6cf843c576b6fc4a9d` | WinOLS Project Workspace |
| `IGN_E90_BG11_ECE_HS_008 _530_2_ign_4.hex` | **2007–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_ECE_HS_009 _530_3_ign_.hex` | **2007–2013** | 5.11 MB | `247a98e2367b0443c1231d7a61602f52` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_ECE_HS_009 _530_3_ign__1.hex` | **2007–2013** | 5.11 MB | `247a98e2367b0443c1231d7a61602f52` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_008 _530_2_ign.hex` | **2007–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_008 _530_2_ign_1.hex` | **2007–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_011 _530_3_2710_ign_1.hex` | **2007–2013** | 5.11 MB | `553690b2f051ba0f87128c4f3cc13764` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_011 _530_3_2710_ign_2.hex` | **2007–2013** | 5.11 MB | `b5e7a7ec47530bd6d65d114d2744d732` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_ECE_HS_008 _530_2_inj_4.hex` | **2007–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_ECE_HS_009 _530_3_inj_.hex` | **2007–2013** | 5.11 MB | `e9ccb7c7a970aac780a21e1bb1eaa5e4` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_ECE_HS_009 _530_3_inj__1.hex` | **2007–2013** | 5.11 MB | `e9ccb7c7a970aac780a21e1bb1eaa5e4` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_008 _530_2_inj.hex` | **2007–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_008 _530_2_inj_1.hex` | **2007–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_011 _530_3_2710_inj_1.hex` | **2007–2013** | 5.11 MB | `be9ef94f82f46babd2f6eccf16b2b13c` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_011 _530_3_2710_inj_2.hex` | **2007–2013** | 5.11 MB | `be9ef94f82f46babd2f6eccf16b2b13c` | Intel HEX Calibration Firmware |
| `WinOLS (BMW E90  V8 4.0-4.2 (Original) als Prozessor - zündung moment).ols` | **2007–2013** | 2.90 MB | `a1fad124dbab76d0bf0ee34acf9469bc` | WinOLS Project Workspace |
| `WinOLS (BMW E90-E91 (Lambda_kat_vmx.sm1) als Prozessor - lambda ).ols` | **2007–2013** | 3.67 MB | `921bfadcdebb613bc10fd8c01fbc336e` | WinOLS Project Workspace |
| `ign.a2l` | **2007–2013** | 3.00 MB | `60868050e5271b20634816729a858e78` | ASAM ASAP2 ECU Description File |
| `inj.a2l` | **2007–2013** | 3.99 MB | `1ad46d85e8b34d60e8a7c9ed30da6bbc` | ASAM ASAP2 ECU Description File |

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
