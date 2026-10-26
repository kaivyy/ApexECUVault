# SAAB TRIONIC LH - ECU Calibration Suite

**Repository Path**: `02_CARS/VOLVO_SAAB/SAAB_TRIONIC_LH`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `8 files` (3 binary dumps, 5 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SAAB_TRIONIC_LH` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: OEM Production

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `0 280 000 944_LH242.bin` | **OEM Production** | 32.0 KB | `53cee307d4ac9cd4127e3c00b152a1f8` | Factory Binary Firmware Dump |
| `0 280 000 948_LH24.bin` | **OEM Production** | 32.0 KB | `8eed3efe1b09daf904c29bcd5edc4916` | Factory Binary Firmware Dump |
| `SAAB9000 ORIGINAL579.bin` | **OEM Production** | 32.0 KB | `f2c76615a85eef2a820a8dc59f27882c` | Factory Binary Firmware Dump |
| `SaabLH241_579.xdf` | **OEM Production** | 22.7 KB | `40ea871535cb347aa3fc0e649b03328f` | TunerPro Binary Definition Map |
| `SaabLH242_944_900sNA.xdf` | **OEM Production** | 11.2 KB | `cd7817fac689279835457a4c71992845` | TunerPro Binary Definition Map |
| `SaabLH24_585_582_586.xdf` | **OEM Production** | 18.0 KB | `bd011bc7ad34aa947cb720db9094efc4` | TunerPro Binary Definition Map |
| `SaabLH24_948.xdf` | **OEM Production** | 17.8 KB | `4fd421b8bb30960e0bb59cb910b32318` | TunerPro Binary Definition Map |
| `Saab_LH22_538.xdf` | **OEM Production** | 5.0 KB | `13998a31e456efa7425c5e0dc76e482d` | TunerPro Binary Definition Map |

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
