# AUDI RS3 TTRS MED17 2 5TFSI DAZA - ECU Calibration Suite

**Repository Path**: `02_CARS/VAG_AUDI_VOLKSWAGEN/AUDI_RS3_TTRS_MED17_2_5TFSI_DAZA`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `8 files` (2 binary dumps, 6 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `AUDI_RS3_TTRS_MED17_2_5TFSI_DAZA` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2017–2022

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `404A_normal.xdf` | **2017–2022** | 3.35 MB | `aad012c59755ff50b60de1b4079f861f` | TunerPro Binary Definition Map |
| `404E_normal.xdf` | **2017–2022** | 6.32 MB | `bb2f80d0d05e130c4b0708b48a3cd8b9` | TunerPro Binary Definition Map |
| `404G_normal.xdf` | **2017–2022** | 3.35 MB | `aad012c59755ff50b60de1b4079f861f` | TunerPro Binary Definition Map |
| `404H_normal.xdf` | **2017–2022** | 5.46 MB | `8c1c9c3543e0f274c4e70eed0ce2afbe` | TunerPro Binary Definition Map |
| `404J_normal.xdf` | **2017–2022** | 3.32 MB | `bf1ce2a120870a9a1af81d22c3417106` | TunerPro Binary Definition Map |
| `404L_normal.xdf` | **2017–2022** | 2.77 MB | `0799325743d0af59775b7a19c308165b` | TunerPro Binary Definition Map |
| `MED17_1_62_8S0907404L__0001_STOCK.bin` | **2017–2022** | 496.0 KB | `ffb9a3977bfe74161f205c2f88cde084` | Factory Binary Firmware Dump |
| `MED17_1_62_STOCK.bin` | **2017–2022** | 496.0 KB | `094de87b6a4a54db579c9f08209e034f` | Factory Binary Firmware Dump |

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
