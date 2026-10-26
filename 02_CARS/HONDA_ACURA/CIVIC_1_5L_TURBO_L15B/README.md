# CIVIC 1 5L TURBO L15B - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CIVIC_1_5L_TURBO_L15B`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `12 files` (1 binary dumps, 11 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CIVIC_1_5L_TURBO_L15B` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805-5AA-A080_Honda_Civic_2017_EX-T_1.5L_L4_-_Gas.xdf` | `.XDF` | `100,842` bytes | Honda Keihin Factory Calibration Package `37805-5AA-A080` |
| `37805-5AA-A580_Honda_Civic_2016_2017_EX-L__EX-T_1.5L_L4_-_Gas.xdf` | `.XDF` | `103,402` bytes | Honda Keihin Factory Calibration Package `37805-5AA-A580` |
| `37805-5AA-A640_Honda_Civic_2016_2017_EX-L__EX-T__Touring_1.5L_L4_-_Gas.xdf` | `.XDF` | `108,116` bytes | Honda Keihin Factory Calibration Package `37805-5AA-A640` |
| `37805-5AM-A120_Honda_Civic_2019_Si_1.5L_L4_-_Gas.xdf` | `.XDF` | `101,115` bytes | Honda Keihin Factory Calibration Package `37805-5AM-A120` |
| `37805-5AM-A220_Honda_Civic_2020_Si_1.5L_L4_-_Gas.xdf` | `.XDF` | `121,713` bytes | Honda Keihin Factory Calibration Package `37805-5AM-A220` |
| `37805-5AN-A220_Honda_Civic_2019_Sport_1.5L_L4_-_Gas__2.0L_L4_-_Gas.xdf` | `.XDF` | `98,964` bytes | Honda Keihin Factory Calibration Package `37805-5AN-A220` |
| `37805-5BF-A340_Honda_Civic_2020_Touring__Type_R_1.5L_L4_-_Gas__2.0L_L4_-_Ga.xdf` | `.XDF` | `121,164` bytes | Honda Keihin Factory Calibration Package `37805-5BF-A340` |
| `37805-5BF-A340_Honda_Civic_2020_Touring__Type_R_1.5L_L4_-_Gas__2.0L_L4_-_Gas.xdf` | `.XDF` | `121,164` bytes | Honda Keihin Factory Calibration Package `37805-5BF-A340` |
| `GENERATIONAL_37805-5AA-A640_Honda_Civic_RS_Turbo_1.5L_VTEC_2016_2021.xdf` | `.XDF` | `1,527` bytes | Honda Keihin Factory Calibration Package `37805-5AA-A640` |
| `GENERATIONAL_37805-64A-A01_CIVIC_GEN11_Honda_Civic_RS_Gen_11_VTEC_Turbo_FE___FL_(2021-2026).xdf` | `.XDF` | `5,580` bytes | TunerPro Binary Definition Map |
| `HONDA_37805-5AA-A01_CIVIC_TURBO.xdf` | `.XDF` | `12,148` bytes | TunerPro Binary Definition Map |
| `HONDA_CRV_CIVIC_TURBO_2017-2022_1.5L_L15B7_KEIHIN_37805-5LA-C940-M1.rwd` | `.RWD` | `2,031,746` bytes | Honda Keihin Factory Calibration Package `37805-5LA-C940` |

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
