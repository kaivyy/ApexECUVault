# XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/LS_V8_P01_P59/XDFS`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `35 files` (0 binary dumps, 35 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `XDFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1989–2006

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `12202088 - 2001 512k.xdf` | **2001** | 617.5 KB | `f100e3a728d6b40bd1da32c831cfb3be` | TunerPro Binary Definition Map |
| `12208322 - 2001 512k.xdf` | **2001** | 617.5 KB | `0742ffff2c2ca927c638c6f546073edd` | TunerPro Binary Definition Map |
| `12209203 - 2002 512k V1.xdf` | **2002** | 588.1 KB | `b706e5a686283cbf25f9cd2dda54f58f` | TunerPro Binary Definition Map |
| `12212156 - 2002 512k V1.xdf` | **2002** | 588.1 KB | `56f1f73f8e4306b4d97913a794f5ef3f` | TunerPro Binary Definition Map |
| `12216125_TCS.xdf` | **1989–2006** | 695 B | `7b84d08b2d44a8cdbc61132ef9e7909d` | TunerPro Binary Definition Map |
| `12587603 - 2004 1mb.xdf` | **2004** | 782.7 KB | `7ca8ac43e3015035e137d442666d4001` | TunerPro Binary Definition Map |
| `12592433-imperial.xdf` | **1989–2006** | 604.7 KB | `306a247281aebb94e518e5cc43972fd8` | TunerPro Binary Definition Map |
| `12592433-metric.xdf` | **1989–2006** | 597.7 KB | `ac7d67a9da799047e4921457247ca6d5` | TunerPro Binary Definition Map |
| `No Password - OS12212156 - 2002 512kB PCM - v5_old.xdf` | **2002** | 1.21 MB | `c4989670035ca4edee4cb2e87f4c7427` | TunerPro Binary Definition Map |
| `No Password - Operating System 12202088 - 512Kb PCM - 2001 model year.xdf` | **2001** | 606.3 KB | `e0e2725eb85329fb2fa5262998d3b217` | TunerPro Binary Definition Map |
| `No Password - Operating System 12208322 - 512Kb PCM - 2001 model year.xdf` | **2001** | 606.3 KB | `27c61d6fefe65a4da3d973b9392e3879` | TunerPro Binary Definition Map |
| `No Password - Operating System 12209203 - 512Kb PCM - 2002 model year.xdf` | **2002** | 603.6 KB | `ba259701aa5918fe1acc3ba29931de88` | TunerPro Binary Definition Map |
| `No Password - Operating System 12216125 - 512Kb PCM - 2002 model year - 5.3L Flex Fuel and 8.1L engines.xdf` | **2002** | 628.3 KB | `8d83c2bdaf00aec95378160e8a0325a7` | TunerPro Binary Definition Map |
| `No Password - Operating System 12221588 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | **2001** | 608.6 KB | `b8cd1d61d82f330d2be75ee2e70922b0` | TunerPro Binary Definition Map |
| `No Password - Operating System 12225074 - 512Kb PCM - 2001 to 2004 Holden model years.xdf` | **2001** | 603.7 KB | `62c4b2e7e74d0d6ce54926abb0c6cc6b` | TunerPro Binary Definition Map |
| `No Password - Operating System 12587603 - 1Mb PCM - 2004 model year.xdf` | **2004** | 616.9 KB | `5be466e0bbbe39b09d50b6ec9db8d4fc` | TunerPro Binary Definition Map |
| `No Password - Operating System 12593358 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | **2001** | 608.6 KB | `fa07afad7ceb4baef8e77e081ae9a6e9` | TunerPro Binary Definition Map |
| `No Password - XDF for Operating System 12202088 - 2001 512Kb PCM - Version 5.xdf` | **2001** | 617.2 KB | `7d4f3a6b8a88828442916eedbfa93cf9` | TunerPro Binary Definition Map |
| `No Password - XDF for Operating System 12208322 - 2001 512Kb PCM - Version 5.xdf` | **2001** | 617.2 KB | `c448a3d75a732a7d27b89cad027416f1` | TunerPro Binary Definition Map |
| `No Password - __Operating System 12212156 - 512Kb PCM - 2002 model year.xdf` | **2002** | 603.6 KB | `6bcb31ae3745e55182809607d97931e4` | TunerPro Binary Definition Map |
| `OS12212156 - 2002 512kB PCM - v5_old.xdf` | **2002** | 1.21 MB | `8861bf342852f70c17ec097633ed23bf` | TunerPro Binary Definition Map |
| `OS12212156 - 2002 512kB PCM - v6 - no password.xdf` | **2002** | 1.61 MB | `88b2c67ba7c2599cfdf84b8dc74977f9` | TunerPro Binary Definition Map |
| `Operating System 12202088 - 512Kb PCM - 2001 model year.xdf` | **2001** | 606.6 KB | `f99672c71efb506d01f650e959b73950` | TunerPro Binary Definition Map |
| `Operating System 12208322 - 512Kb PCM - 2001 model year.xdf` | **2001** | 606.6 KB | `30fe386c867d20e46ff002f8d2931f32` | TunerPro Binary Definition Map |
| `Operating System 12209203 - 512Kb PCM - 2002 model year.xdf` | **2002** | 603.9 KB | `adf7d7a532e9ced7f51b13b64b86d6e4` | TunerPro Binary Definition Map |
| `Operating System 12216125 - 512Kb PCM - 2002 model year - 5.3L Flex Fuel and 8.1L engines.xdf` | **2002** | 628.6 KB | `ec2b10127f423bd88429374760601a3f` | TunerPro Binary Definition Map |
| `Operating System 12221588 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | **2001** | 608.9 KB | `a94e18aeeb905b253062fcf73bf5804c` | TunerPro Binary Definition Map |
| `Operating System 12225074 - 512Kb PCM - 2001 to 2004 Holden model years.xdf` | **2001** | 604.0 KB | `f089a954397bfb542df9aea77691acde` | TunerPro Binary Definition Map |
| `Operating System 12587603 - 1Mb PCM - 2004 model year.xdf` | **2004** | 617.2 KB | `d2d3d2bfc08a93161fd0d4fa5ed0fb6d` | TunerPro Binary Definition Map |
| `Operating System 12593358 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | **2001** | 608.9 KB | `15bf8b94a214a8a9c11ec0922cf10f7a` | TunerPro Binary Definition Map |
| `P01_512Kb_Experimental-Need_Testing_OS_12202088_12202088 - 2001 512k.xdf` | **2001** | 617.5 KB | `f100e3a728d6b40bd1da32c831cfb3be` | TunerPro Binary Definition Map |
| `P01_512Kb_Experimental-Need_Testing_OS_12208322_12208322 - 2001 512k.xdf` | **2001** | 617.5 KB | `0742ffff2c2ca927c638c6f546073edd` | TunerPro Binary Definition Map |
| `XDF for Operating System 12202088 - 2001 512Kb PCM - Version 5.xdf` | **2001** | 617.5 KB | `db3d7c39bf507e36e295fba1693340c4` | TunerPro Binary Definition Map |
| `XDF for Operating System 12208322 - 2001 512Kb PCM - Version 5.xdf` | **2001** | 617.5 KB | `76021fa42e3ba278d27cc2bce687f670` | TunerPro Binary Definition Map |
| `~~Operating System 12212156 - 512Kb PCM - 2002 model year.xdf` | **2002** | 603.9 KB | `e21ac6618d05b41a41621a153e421d40` | TunerPro Binary Definition Map |

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
