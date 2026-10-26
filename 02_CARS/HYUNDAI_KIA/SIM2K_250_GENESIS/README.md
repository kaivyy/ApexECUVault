# SIM2K 250 GENESIS - ECU Calibration Suite

**Repository Path**: `02_CARS/HYUNDAI_KIA/SIM2K_250_GENESIS`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `11 files` (10 binary dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SIM2K_250_GENESIS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2010–2016

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `HYUNDAI_SIM2K_250_TURBO_G70.xdf` | **2010–2016** | 7.5 KB | `49459dfd9b38e47912679ab611afe91e` | TunerPro Binary Definition Map |
| `SIM2K-250_606X0A5000000_GCC_FuelQuality.bin` | **2010–2016** | 2.50 MB | `7de2bfa910ffa0153cf58a971b76fc95` | Factory Binary Firmware Dump |
| `SIM2K-250_606X0A5000000_Original.bin` | **2010–2016** | 2.50 MB | `d35f24bb40df96db4958378f06d34174` | Factory Binary Firmware Dump |
| `SIM2K-250_606X1A6K00000_GCC_FuelQuality.bin` | **2010–2016** | 2.50 MB | `add9e09f2d27b3d71266b8201464918f` | Factory Binary Firmware Dump |
| `SIM2K-250_606X1A6K00000_Original.bin` | **2010–2016** | 2.50 MB | `29c2c818ad4445dcb7de23e78c42b35a` | Factory Binary Firmware Dump |
| `SIM2K-250_606Y0B4000000_GCC_FuelQuality.bin` | **2010–2016** | 2.50 MB | `6036437e1879c1a287fcccce4ab106c7` | Factory Binary Firmware Dump |
| `SIM2K-250_606Y0B4000000_Original.bin` | **2010–2016** | 2.50 MB | `9968fd8cba6e5e3accbdb828a2ca7fc2` | Factory Binary Firmware Dump |
| `SIM2K-250_606Z0D5K00000_GCC_FuelQuality.bin` | **2010–2016** | 2.50 MB | `f1af1aed8760958b1168697b0bf44642` | Factory Binary Firmware Dump |
| `SIM2K-250_606Z0D5K00000_Original.bin` | **2010–2016** | 2.50 MB | `bfac155aee17f2d6724503eff2644e37` | Factory Binary Firmware Dump |
| `SIM2K-250_6H6N090000000_GCC_FuelQuality.bin` | **2010–2016** | 2.50 MB | `64664ffc449ed904d8e873da6cbb4417` | Factory Binary Firmware Dump |
| `SIM2K-250_6H6N090000000_Original.bin` | **2010–2016** | 2.50 MB | `0c03a7d1d42ada2d965311539730b53f` | Factory Binary Firmware Dump |

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
