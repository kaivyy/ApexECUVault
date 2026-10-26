# LS V8 P01 P59 - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/LS_V8_P01_P59`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `37 files` (0 binary dumps, 37 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `LS_V8_P01_P59` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `12202088 - 2001 512k.xdf` | **2001** | 617.5 KB | `f100e3a728d6b40bd1da32c831cfb3be` | TunerPro Binary Definition Map |
| `12202088_release.xdf` | **OEM Production** | 617.5 KB | `f100e3a728d6b40bd1da32c831cfb3be` | TunerPro Binary Definition Map |
| `12208322 - 2001 512k.xdf` | **2001** | 617.5 KB | `0742ffff2c2ca927c638c6f546073edd` | TunerPro Binary Definition Map |
| `12208322_release.xdf` | **1999–2002 (P01)** | 617.5 KB | `0742ffff2c2ca927c638c6f546073edd` | TunerPro Binary Definition Map |
| `12209203_release.xdf` | **OEM Production** | 588.1 KB | `b706e5a686283cbf25f9cd2dda54f58f` | TunerPro Binary Definition Map |
| `12212156_release.xdf` | **1999–2002 (P01)** | 588.1 KB | `56f1f73f8e4306b4d97913a794f5ef3f` | TunerPro Binary Definition Map |
| `12216125_TCS.xdf` | **OEM Production** | 695 B | `7b84d08b2d44a8cdbc61132ef9e7909d` | TunerPro Binary Definition Map |
| `12587603_RC1.xdf` | **2003–2007 (P59)** | 782.7 KB | `7ca8ac43e3015035e137d442666d4001` | TunerPro Binary Definition Map |
| `12587603_release.xdf` | **2003–2007 (P59)** | 617.2 KB | `d2d3d2bfc08a93161fd0d4fa5ed0fb6d` | TunerPro Binary Definition Map |
| `12592433_Beta_metric.xdf` | **OEM Production** | 583.9 KB | `0a29a6bc893c2d5d60ffb31e5809a1de` | TunerPro Binary Definition Map |
| `12592433_beta_imperial.xdf` | **OEM Production** | 590.8 KB | `a166279e5ea2ecf2ec91b861afa8de34` | TunerPro Binary Definition Map |
| `12592618_alpha.xdf` | **2003–2007 (P59)** | 26.8 KB | `e57fc5aec165a391b5e266e6985c2a20` | TunerPro Binary Definition Map |
| `Lean Cruise.xdf` | **OEM Production** | 2.0 KB | `332f189f9f987843c41fdabcdcf70e16` | TunerPro Binary Definition Map |
| `No Password - 12587603_release.xdf` | **2003–2007 (P59)** | 616.9 KB | `e833ffd09b7dca11c86475bab3874365` | TunerPro Binary Definition Map |
| `No Password - OS12212156 - 2002 512kB PCM - v5_old.xdf` | **2002** | 1.21 MB | `a2b8e6f719b6e34af1bfbd89f745c772` | TunerPro Binary Definition Map |
| `No Password - Operating System 12202088 - 512Kb PCM - 2001 model year.xdf` | **2001** | 606.3 KB | `38261c012eced48a87ef11f19ca6f09a` | TunerPro Binary Definition Map |
| `No Password - Operating System 12208322 - 512Kb PCM - 2001 model year.xdf` | **2001** | 606.3 KB | `d9d3003710592f136071be47bc7460eb` | TunerPro Binary Definition Map |
| `No Password - Operating System 12209203 - 512Kb PCM - 2002 model year.xdf` | **2002** | 603.6 KB | `51dea8e533753ce283f406a2e8d73dff` | TunerPro Binary Definition Map |
| `No Password - Operating System 12216125 - 512Kb PCM - 2002 model year - 5.3L Flex Fuel and 8.1L engines.xdf` | **2002** | 628.3 KB | `6ee55c6014c0a2f29b83e7bded617567` | TunerPro Binary Definition Map |
| `No Password - Operating System 12221588 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | **2001** | 608.6 KB | `b75ab649d73afa51f44fb4b71d9669b8` | TunerPro Binary Definition Map |
| `No Password - Operating System 12225074 - 512Kb PCM - 2001 to 2004 Holden model years.xdf` | **2001** | 603.7 KB | `02fdca5b4b10ef01b508198b6afc9f35` | TunerPro Binary Definition Map |
| `No Password - Operating System 12593358 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | **2001** | 608.6 KB | `5bb6674aacd66dcf843d904594fcf181` | TunerPro Binary Definition Map |
| `No Password - XDF for Operating System 12202088 - 2001 512Kb PCM - Version 5.xdf` | **2001** | 617.2 KB | `43349e6f23d5d37726adf4f634bad2c3` | TunerPro Binary Definition Map |
| `No Password - XDF for Operating System 12208322 - 2001 512Kb PCM - Version 5.xdf` | **2001** | 617.2 KB | `0a6661d4585dde4ed86f9d260f9dcbd5` | TunerPro Binary Definition Map |
| `No Password - __Operating System 12212156 - 512Kb PCM - 2002 model year.xdf` | **2002** | 603.6 KB | `01e0be704ae2073779165d4f49e74957` | TunerPro Binary Definition Map |
| `OS12212156 - 2002 512kB PCM - v5_old.xdf` | **2002** | 1.21 MB | `8861bf342852f70c17ec097633ed23bf` | TunerPro Binary Definition Map |
| `OS12212156 - 2002 512kB PCM - v6 - no password.xdf` | **2002** | 1.61 MB | `88b2c67ba7c2599cfdf84b8dc74977f9` | TunerPro Binary Definition Map |
| `Operating System 12202088 - 512Kb PCM - 2001 model year.xdf` | **2001** | 606.6 KB | `f99672c71efb506d01f650e959b73950` | TunerPro Binary Definition Map |
| `Operating System 12208322 - 512Kb PCM - 2001 model year.xdf` | **2001** | 606.6 KB | `30fe386c867d20e46ff002f8d2931f32` | TunerPro Binary Definition Map |
| `Operating System 12209203 - 512Kb PCM - 2002 model year.xdf` | **2002** | 603.9 KB | `adf7d7a532e9ced7f51b13b64b86d6e4` | TunerPro Binary Definition Map |
| `Operating System 12216125 - 512Kb PCM - 2002 model year - 5.3L Flex Fuel and 8.1L engines.xdf` | **2002** | 628.6 KB | `ec2b10127f423bd88429374760601a3f` | TunerPro Binary Definition Map |
| `Operating System 12221588 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | **2001** | 608.9 KB | `a94e18aeeb905b253062fcf73bf5804c` | TunerPro Binary Definition Map |
| `Operating System 12225074 - 512Kb PCM - 2001 to 2004 Holden model years.xdf` | **2001** | 604.0 KB | `f089a954397bfb542df9aea77691acde` | TunerPro Binary Definition Map |
| `Operating System 12593358 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | **2001** | 608.9 KB | `15bf8b94a214a8a9c11ec0922cf10f7a` | TunerPro Binary Definition Map |
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
