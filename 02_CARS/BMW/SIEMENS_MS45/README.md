# SIEMENS MS45 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/SIEMENS_MS45`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `13 files` (0 binary dumps, 13 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SIEMENS_MS45` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2003–2006

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `60010000.xdf` | **2003–2006** | 1.60 MB | `c7bc1bef5c762ae84840c9b0b4d51265` | TunerPro Binary Definition Map |
| `MS45 ECU Definitions v0.1.xml` | **2003–2006** | 16.5 KB | `308e182a3e877a996f64f1fec447b0fe` | ECU / ASAP2 Calibration Map Definition |
| `MS45 ECU Definitions v0.2.TJW.xml` | **2003–2006** | 76.1 KB | `2001d5c7686696f961d2e36f1f053a1b` | ECU / ASAP2 Calibration Map Definition |
| `MS45 ECU Definitions v0.2.xml` | **2003–2006** | 36.9 KB | `0f4379f70742e7513dce3a3b46b945f5` | ECU / ASAP2 Calibration Map Definition |
| `MS45 ECU Definitions v0.3.1.xml` | **2003–2006** | 92.5 KB | `302ac150e7eb3ace65c489da6b7e05de` | ECU / ASAP2 Calibration Map Definition |
| `MS45 ECU Definitions v0.3.xml` | **2003–2006** | 81.9 KB | `5798630cecba39ea2c1341dab67307ef` | ECU / ASAP2 Calibration Map Definition |
| `MS45 ECU Definitions.xml` | **2003–2006** | 347.9 KB | `b46b3015e3babbd730a00ee1d0763922` | ECU / ASAP2 Calibration Map Definition |
| `MS45.1 457LO00S full.xml` | **2003–2006** | 1.08 MB | `2b9caf279cecc18570daf5878d75084b` | ECU / ASAP2 Calibration Map Definition |
| `MS45.1 457LO00S partial.xml` | **2003–2006** | 1.08 MB | `fdacf4bc63a45f1e8bc14ff95cb13ccf` | ECU / ASAP2 Calibration Map Definition |
| `Siemens_MS450_456BO02S_1024K.xdf` | **2003–2006** | 4.43 MB | `f5c4e7252d94ab5e2b65e314e51152de` | TunerPro Binary Definition Map |
| `Siemens_MS450_456BO02S_116K.xdf` | **2003–2006** | 4.43 MB | `fc029915f20e86768d2822bdc8b2ca9d` | TunerPro Binary Definition Map |
| `Siemens_MS451_457LO02S_1024K.xdf` | **2003–2006** | 4.57 MB | `d3e4f375aec07ba41e8d8366cb0a63b1` | TunerPro Binary Definition Map |
| `Siemens_MS451_457LO02S_116K.xdf` | **2003–2006** | 4.57 MB | `d5c88fb8148ef89ee0a27cf423cd8157` | TunerPro Binary Definition Map |

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
