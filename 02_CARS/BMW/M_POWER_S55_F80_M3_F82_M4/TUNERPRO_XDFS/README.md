# TUNERPRO_XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/TUNERPRO_XDFS`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `13 files` (0 binary dumps, 13 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `TUNERPRO_XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2014–2020

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `00000D07596401.xdf` | **2014–2020** | 1.12 MB | `54ecc9ce7f7887341ef0024d0efb1d8a` | TunerPro Binary Definition Map |
| `00000E2B3B0A01.xdf` | **2014–2020** | 1021.2 KB | `2a1dfa71bd836d7a926179936ebaeb8d` | TunerPro Binary Definition Map |
| `00000FEF81A001.xdf` | **2014–2020** | 1.21 MB | `83f1f282b0239d12ac198c9dba23aea8` | TunerPro Binary Definition Map |
| `00001A841D1401.xdf` | **2014–2020** | 1.57 MB | `0a91d5aa1c18f041b51c2168bc6f17fa` | TunerPro Binary Definition Map |
| `00001A841D2801.xdf` | **2014–2020** | 1.56 MB | `b4a403f71993964061f2e73b7596863f` | TunerPro Binary Definition Map |
| `00001C41279601.xdf` | **2014–2020** | 1.21 MB | `85cfb2ad737aa42bfcfb8efb1050e1c6` | TunerPro Binary Definition Map |
| `000021571D8202.xdf` | **2014–2020** | 1.38 MB | `04f0ae0563997b3bfcdfb684ee4ad731` | TunerPro Binary Definition Map |
| `000021571DAA01.xdf` | **2014–2020** | 1.40 MB | `122abda26161d631f7c47e4bf1b3d34d` | TunerPro Binary Definition Map |
| `000021571DBE01.xdf` | **2014–2020** | 1.40 MB | `9650d306df275b381cfff6c43d77c00a` | TunerPro Binary Definition Map |
| `00002DF2132801.xdf` | **2014–2020** | 1.32 MB | `f5d6913ee2ecc1bcb137a42a96c7560e` | TunerPro Binary Definition Map |
| `00005BA8134601.xdf` | **2014–2020** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |
| `00005BA8135001.xdf` | **2014–2020** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |
| `00005BA8135A01.xdf` | **2014–2020** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |

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
