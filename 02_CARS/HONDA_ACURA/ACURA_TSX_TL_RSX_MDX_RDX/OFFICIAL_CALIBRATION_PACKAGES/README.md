# OFFICIAL CALIBRATION PACKAGES - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/ACURA_TSX_TL_RSX_MDX_RDX/OFFICIAL_CALIBRATION_PACKAGES`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `56 files` (56 binary dumps, 0 definition maps)  

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
| `37805-PND-4160.rwd` | `.RWD` | `538,549` bytes | Honda Keihin Factory Calibration Package `37805-PND-4160` |
| `37805-PND-4250.rwd` | `.RWD` | `538,319` bytes | Honda Keihin Factory Calibration Package `37805-PND-4250` |
| `37805-PND-A090-M1.rwd` | `.RWD` | `123,203` bytes | Honda Keihin Factory Calibration Package `37805-PND-A090` |
| `37805-PND-A590-M1.rwd` | `.RWD` | `193,959` bytes | Honda Keihin Factory Calibration Package `37805-PND-A590` |
| `37805-PND-A660-M1.rwd` | `.RWD` | `540,569` bytes | Honda Keihin Factory Calibration Package `37805-PND-A660` |
| `37805-PNF-3050.rwd` | `.RWD` | `125,381` bytes | Honda Keihin Factory Calibration Package `37805-PNF-3050` |
| `37805-PRB-3060.rwd` | `.RWD` | `540,209` bytes | Honda Keihin Factory Calibration Package `37805-PRB-3060` |
| `37805-PRB-4250.rwd` | `.RWD` | `538,319` bytes | Honda Keihin Factory Calibration Package `37805-PRB-4250` |
| `37805-PVJ-3050.rwd` | `.RWD` | `637,869` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-3050` |
| `37805-R8A-A660-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-R8A-A660` |
| `37805-R8A-X540-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-R8A-X540` |
| `37805-RBB-A210-M1.rwd` | `.RWD` | `1,015,866` bytes | Honda Keihin Factory Calibration Package `37805-RBB-A210` |
| `37805-RBB-A710-M1.rwd` | `.RWD` | `1,015,866` bytes | Honda Keihin Factory Calibration Package `37805-RBB-A710` |
| `37805-RBJ-3090-M1.RWD` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RBJ-3090` |
| `37805-RDA-A120-M1.rwd` | `.RWD` | `376,609` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A120` |
| `37805-RDA-A240-M1.rwd` | `.RWD` | `568,159` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A240` |
| `37805-RDA-A570-M1.rwd` | `.RWD` | `523,269` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A570` |
| `37805-RDA-A620-M1.rwd` | `.RWD` | `524,029` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A620` |
| `37805-RDA-A730-M1.rwd` | `.RWD` | `568,129` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A730` |
| `37805-RDA-A850-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A850` |
| `37805-RDB-A040-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RDB-A040` |
| `37805-RDB-A120-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RDB-A120` |
| `37805-RDB-A560-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RDB-A560` |
| `37805-RJA-A840-M1.rwd` | `.RWD` | `654,689` bytes | Honda Keihin Factory Calibration Package `37805-RJA-A840` |
| `37805-RJA-A930-M1.rwd` | `.RWD` | `676,029` bytes | Honda Keihin Factory Calibration Package `37805-RJA-A930` |
| `37805-RJA-X550-M1.rwd` | `.RWD` | `654,249` bytes | Honda Keihin Factory Calibration Package `37805-RJA-X550` |
| `37805-RJE-A840-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RJE-A840` |
| `37805-RJE-A960-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RJE-A960` |
| `37805-RKG-A560-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RKG-A560` |
| `37805-RKG-A720-M1.RWD` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RKG-A720` |
| `37805-RKG-U520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RKG-U520` |
| `37805-RL5-A030-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A030` |
| `37805-RL5-A070-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A070` |
| `37805-RL5-A120-M1.RWD` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A120` |
| `37805-RL5-A560-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A560` |
| `37805-RL5-A710-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A710` |
| `37805-RL5-X020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RL5-X020` |
| `37805-RL5-X520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RL5-X520` |
| `37805-RL8-A520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RL8-A520` |
| `37805-RL8-A730-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RL8-A730` |
| `37805-RL8-X520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RL8-X520` |
| `37805-RL8-X730-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RL8-X730` |
| `37805-RP6-A640-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RP6-A640` |
| `37805-RP6-A760-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RP6-A760` |
| `37805-RP6-A840-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RP6-A840` |
| `37805-RP6-X560-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RP6-X560` |
| `37805-RRB-A140-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RRB-A140` |
| `37805-RWC-A570-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RWC-A570` |
| `37805-RWC-A620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RWC-A620` |
| `37805-RWC-A720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RWC-A720` |
| `37805-RWC-A810-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RWC-A810` |
| `37805-RYE-A590-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A590` |
| `37805-RYE-A630-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A630` |
| `37805-RYE-A750-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A750` |
| `37805-RYE-A850-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A850` |
| `37805-RYE-X580-M1.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RYE-X580` |

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
