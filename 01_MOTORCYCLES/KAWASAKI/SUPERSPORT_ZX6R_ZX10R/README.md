# SUPERSPORT ZX6R ZX10R - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/KAWASAKI/SUPERSPORT_ZX6R_ZX10R`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `5 files` (0 binary dumps, 5 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SUPERSPORT_ZX6R_ZX10R` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2004–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `GENERATIONAL_21175-0744_Kawasaki_Ninja_ZX_6R_636_Gen_4_2013_2018_131PS.xdf` | **2013–2018** | 1.8 KB | `f291a39d3eb61d748227374d31e5b2d2` | TunerPro Binary Definition Map |
| `GENERATIONAL_21175-0822_Kawasaki_Ninja_ZX_10R_Gen_4_2011_2015_200PS.xdf` | **2011–2015** | 1.8 KB | `26a4dfff03d821d31b907ade6a970901` | TunerPro Binary Definition Map |
| `GENERATIONAL_21175-1153_Kawasaki_Ninja_ZX_10R_Gen_5___RR_2016_2020_203PS.xdf` | **2016–2020** | 1.8 KB | `54af0a97867beb2ef09fbd7b2dc1ca3c` | TunerPro Binary Definition Map |
| `GENERATIONAL_21175-1636_Kawasaki_All_New_Ninja_ZX_10R_Gen_6_Facelift_2021_2026_203PS.xdf` | **2021–2026** | 1.8 KB | `0b813e2e76028b21a7747eb2072dffee` | TunerPro Binary Definition Map |
| `KAWASAKI_21175-0920_Kawasaki_Ninja_ZX-6R_636_(ZX636R).xdf` | **2004–2024** | 9.4 KB | `b1c61e9dafb3ba602a1234d3e80f6c3b` | TunerPro Binary Definition Map |

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
