# OFFICIAL CALIBRATION PACKAGES - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CRV_HRV_SUVS_ODYSSEY/OFFICIAL_CALIBRATION_PACKAGES`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `44 files` (44 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `OFFICIAL_CALIBRATION_PACKAGES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `37805-PPA-3060.rwd` | `.RWD` | `194,091` bytes | Honda Keihin Factory Calibration Package `37805-PPA-3060` |
| `37805-PPA-3070.rwd` | `.RWD` | `194,113` bytes | Honda Keihin Factory Calibration Package `37805-PPA-3070` |
| `37805-PPA-4080.rwd` | `.RWD` | `590,389` bytes | Honda Keihin Factory Calibration Package `37805-PPA-4080` |
| `37805-PPA-4090.rwd` | `.RWD` | `590,389` bytes | Honda Keihin Factory Calibration Package `37805-PPA-4090` |
| `37805-PPA-4270.rwd` | `.RWD` | `588,729` bytes | Honda Keihin Factory Calibration Package `37805-PPA-4270` |
| `37805-PPA-4350.rwd` | `.RWD` | `588,789` bytes | Honda Keihin Factory Calibration Package `37805-PPA-4350` |
| `37805-PPA-K120-M1.rwd` | `.RWD` | `588,379` bytes | Honda Keihin Factory Calibration Package `37805-PPA-K120` |
| `37805-PVJ-3060.rwd` | `.RWD` | `637,869` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-3060` |
| `37805-PVJ-A820-M1.rwd` | `.RWD` | `656,389` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-A820` |
| `37805-PVJ-X530-M1.rwd` | `.RWD` | `637,289` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-X530` |
| `37805-PZD-3060.rwd` | `.RWD` | `522,719` bytes | Honda Keihin Factory Calibration Package `37805-PZD-3060` |
| `37805-PZD-3070.rwd` | `.RWD` | `522,719` bytes | Honda Keihin Factory Calibration Package `37805-PZD-3070` |
| `37805-PZD-3090.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-PZD-3090` |
| `37805-PZD-4050.rwd` | `.RWD` | `532,799` bytes | Honda Keihin Factory Calibration Package `37805-PZD-4050` |
| `37805-PZD-4170.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-PZD-4170` |
| `37805-PZD-A480-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-PZD-A480` |
| `37805-PZD-A590-M1.rwd` | `.RWD` | `534,979` bytes | Honda Keihin Factory Calibration Package `37805-PZD-A590` |
| `37805-PZD-A690-M1.rwd` | `.RWD` | `534,979` bytes | Honda Keihin Factory Calibration Package `37805-PZD-A690` |
| `37805-PZD-A720-M1.rwd` | `.RWD` | `536,539` bytes | Honda Keihin Factory Calibration Package `37805-PZD-A720` |
| `37805-PZD-A820-M1.rwd` | `.RWD` | `536,539` bytes | Honda Keihin Factory Calibration Package `37805-PZD-A820` |
| `37805-REX-X540-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-REX-X540` |
| `37805-REZ-A570-M1.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-REZ-A570` |
| `37805-RGL-A020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RGL-A020` |
| `37805-RGL-A570-M1.rwd` | `.RWD` | `637,929` bytes | Honda Keihin Factory Calibration Package `37805-RGL-A570` |
| `37805-RGL-A730-M1.rwd` | `.RWD` | `646,519` bytes | Honda Keihin Factory Calibration Package `37805-RGL-A730` |
| `37805-RGL-A840-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RGL-A840` |
| `37805-RGL-A930-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RGL-A930` |
| `37805-RGL-K720-M1.rwd` | `.RWD` | `645,109` bytes | Honda Keihin Factory Calibration Package `37805-RGL-K720` |
| `37805-RGM-A750-M1.rwd` | `.RWD` | `676,349` bytes | Honda Keihin Factory Calibration Package `37805-RGM-A750` |
| `37805-RGM-A840-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RGM-A840` |
| `37805-RGW-A060-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RGW-A060` |
| `37805-RGW-A960-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RGW-A960` |
| `37805-RJA-A630-M1.rwd` | `.RWD` | `676,029` bytes | Honda Keihin Factory Calibration Package `37805-RJA-A630` |
| `37805-RJE-K720-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RJE-K720` |
| `37805-RME-A180-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RME-A180` |
| `37805-RN0-A630-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RN0-A630` |
| `37805-RN0-A770-M1.RWD` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RN0-A770` |
| `37805-RN0-A830-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RN0-A830` |
| `37805-RN0-A970-M1.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RN0-A970` |
| `37805-RV0-A650-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RV0-A650` |
| `37805-RV0-A780-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RV0-A780` |
| `37805-RV0-X580-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RV0-X580` |
| `37805-RZA-A570-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RZA-A570` |
| `37805-RZA-A770-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RZA-A770` |

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
