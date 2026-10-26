# XDFS - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/OBD1_TBI_TPI_LT1/XDFS`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `50 files` (0 binary dumps, 50 definition maps)  

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

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `0D_tpv4_v200.xdf` | `.XDF` | `994,579` bytes | TunerPro Binary Definition Map |
| `0D_tpv5_v250.xdf` | `.XDF` | `1,359,231` bytes | TunerPro Binary Definition Map |
| `0E_tpv4_v200.xdf` | `.XDF` | `868,853` bytes | TunerPro Binary Definition Map |
| `0E_tpv5_v250.xdf` | `.XDF` | `1,188,602` bytes | TunerPro Binary Definition Map |
| `1C.xdf` | `.XDF` | `33,643` bytes | TunerPro Binary Definition Map |
| `1D.xdf` | `.XDF` | `69,665` bytes | TunerPro Binary Definition Map |
| `1F.xdf` | `.XDF` | `60,575` bytes | TunerPro Binary Definition Map |
| `1FA.xdf` | `.XDF` | `97,875` bytes | TunerPro Binary Definition Map |
| `24.xdf` | `.XDF` | `60,907` bytes | TunerPro Binary Definition Map |
| `24A.xdf` | `.XDF` | `66,468` bytes | TunerPro Binary Definition Map |
| `2E.xdf` | `.XDF` | `148,312` bytes | TunerPro Binary Definition Map |
| `2E_tpv5.xdf` | `.XDF` | `399,423` bytes | TunerPro Binary Definition Map |
| `31.xdf` | `.XDF` | `70,759` bytes | TunerPro Binary Definition Map |
| `31_tpv5_v250.xdf` | `.XDF` | `1,188,595` bytes | TunerPro Binary Definition Map |
| `32.xdf` | `.XDF` | `64,603` bytes | TunerPro Binary Definition Map |
| `32B.xdf` | `.XDF` | `54,466` bytes | TunerPro Binary Definition Map |
| `3A.xdf` | `.XDF` | `61,197` bytes | TunerPro Binary Definition Map |
| `42.xdf` | `.XDF` | `105,884` bytes | TunerPro Binary Definition Map |
| `4E.xdf` | `.XDF` | `87,274` bytes | TunerPro Binary Definition Map |
| `58ASunbird.xdf` | `.XDF` | `79,321` bytes | TunerPro Binary Definition Map |
| `58SyTy.xdf` | `.XDF` | `307,509` bytes | TunerPro Binary Definition Map |
| `5B4.xdf` | `.XDF` | `78,080` bytes | TunerPro Binary Definition Map |
| `5B5.xdf` | `.XDF` | `68,361` bytes | TunerPro Binary Definition Map |
| `5B6.xdf` | `.XDF` | `110,743` bytes | TunerPro Binary Definition Map |
| `5B_TPV5.xdf` | `.XDF` | `250,313` bytes | TunerPro Binary Definition Map |
| `61v3.xdf` | `.XDF` | `121,590` bytes | TunerPro Binary Definition Map |
| `62.xdf` | `.XDF` | `59,856` bytes | TunerPro Binary Definition Map |
| `6D.xdf` | `.XDF` | `91,943` bytes | TunerPro Binary Definition Map |
| `6E.xdf` | `.XDF` | `103,510` bytes | TunerPro Binary Definition Map |
| `83A.xdf` | `.XDF` | `41,467` bytes | TunerPro Binary Definition Map |
| `85.xdf` | `.XDF` | `77,251` bytes | TunerPro Binary Definition Map |
| `88.xdf` | `.XDF` | `87,319` bytes | TunerPro Binary Definition Map |
| `8B.xdf` | `.XDF` | `103,783` bytes | TunerPro Binary Definition Map |
| `8E.xdf` | `.XDF` | `52,889` bytes | TunerPro Binary Definition Map |
| `8F.xdf` | `.XDF` | `590,724` bytes | TunerPro Binary Definition Map |
| `8F_v2.xdf` | `.XDF` | `434,742` bytes | TunerPro Binary Definition Map |
| `94.xdf` | `.XDF` | `52,190` bytes | TunerPro Binary Definition Map |
| `99.xdf` | `.XDF` | `50,069` bytes | TunerPro Binary Definition Map |
| `A1.xdf` | `.XDF` | `243,996` bytes | TunerPro Binary Definition Map |
| `A1_tpv4.xdf` | `.XDF` | `174,190` bytes | TunerPro Binary Definition Map |
| `A1_tpv5.xdf` | `.XDF` | `721,848` bytes | TunerPro Binary Definition Map |
| `DA2.xdf` | `.XDF` | `41,062` bytes | TunerPro Binary Definition Map |
| `DA3.xdf` | `.XDF` | `142,628` bytes | TunerPro Binary Definition Map |
| `DF.xdf` | `.XDF` | `89,311` bytes | TunerPro Binary Definition Map |
| `E6_tpv4_v200.xdf` | `.XDF` | `991,341` bytes | TunerPro Binary Definition Map |
| `E6_tpv5_v250.xdf` | `.XDF` | `1,355,081` bytes | TunerPro Binary Definition Map |
| `E8.xdf` | `.XDF` | `101,976` bytes | TunerPro Binary Definition Map |
| `EE.xdf` | `.XDF` | `141,787` bytes | TunerPro Binary Definition Map |
| `F0.xdf` | `.XDF` | `63,374` bytes | TunerPro Binary Definition Map |
| `T31.xdf` | `.XDF` | `134,160` bytes | TunerPro Binary Definition Map |

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
