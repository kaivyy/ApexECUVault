# BOSCH_ME9_VALVETRONIC_N42_N46_N62 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/BOSCH_ME9_VALVETRONIC_N42_N46_N62`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `14 files` (3 binary dumps, 11 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `BOSCH_ME9_VALVETRONIC_N42_N46_N62` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2001–2010

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `6m661411.A2L` | **2001–2010** | 11.24 MB | `eb4ccf01310c0c984f85fa5ae683f2d1` | ASAM ASAP2 ECU Description File |
| `715c360b.a2l` | **2001–2010** | 5.83 MB | `7abf783e062afc75d876576259a9f716` | ASAM ASAP2 ECU Description File |
| `715c4000_r2.a2l` | **2001–2010** | 5.83 MB | `593380f375e0506d566032e185c9edf0` | ASAM ASAP2 ECU Description File |
| `715c4500.a2l` | **2001–2010** | 5.84 MB | `a4a9151a25f65232f63808504bd59fa1` | ASAM ASAP2 ECU Description File |
| `725D601B.a2l` | **2001–2010** | 8.84 MB | `a0d357ffa984ef52d42b6e57b6a23ebb` | ASAM ASAP2 ECU Description File |
| `770115XE.BIN` | **2001–2010** | 1.00 MB | `fa99f575833b2b32b5a66220668ae2cd` | Factory Binary Firmware Dump |
| `770115XE.a2l` | **2001–2010** | 4.18 MB | `d8dba884908075609874440ca9ed60c4` | ASAM ASAP2 ECU Description File |
| `770115XE_alt.a2l` | **2001–2010** | 3.98 MB | `7155ad8562bc86f2060463d2ae7665cb` | ASAM ASAP2 ECU Description File |
| `BMW ME9.ols` | **2001–2010** | 3.30 MB | `a04df59f33e78768e967327be72f7b52` | WinOLS Project Workspace |
| `WinOLS (545i   7180A560B BMW E60-E61 (Original) ).ols` | **2001–2010** | 2.72 MB | `d68aa26df0bb069a5918bd327a87291d` | WinOLS Project Workspace |
| `WinOLS (BMW E46 (Original) - 368248).bin` | **2001–2010** | 1.00 MB | `fa99f575833b2b32b5a66220668ae2cd` | Factory Binary Firmware Dump |
| `WinOLS (BMW E46 (Original) - 368248).kp` | **2001–2010** | 129.9 KB | `3d567aaa0507431c90b3efb482c4e085` | WinOLS Map Definition Pack |
| `WinOLS (BMW E60-E61 (Original) - 7180A560B).bin` | **2001–2010** | 128.0 KB | `a0ac9d2de8f9a472ff45120791fe72a7` | Factory Binary Firmware Dump |
| `WinOLS (BMW E60-E61 (Original) - 7180A560B).kp` | **2001–2010** | 250.9 KB | `772b92c7f38dcb0f5221dddae6af0be6` | WinOLS Map Definition Pack |

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
