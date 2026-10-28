# VOLVO_LH_JETRONIC - ECU Calibration Suite

**Repository Path**: `02_CARS/VOLVO_SAAB/VOLVO_LH_JETRONIC`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `17 files` (8 binary dumps, 9 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `VOLVO_LH_JETRONIC` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `0227400208_2227355740_EZK116.bin` | **2000–2024** | 32.0 KB | `c990ca22b7298c3e1ffb4be3498462b1` | Factory Binary Firmware Dump |
| `0280-000-560.BIN` | **2000–2024** | 32.0 KB | `a5d6f19f0197b180279220da1a01be0e` | Factory Binary Firmware Dump |
| `0280-000-913.BIN` | **2000–2024** | 32.0 KB | `a8b749312dd509083a46d235a0591ab8` | Factory Binary Firmware Dump |
| `0280-000-937.BIN` | **2000–2024** | 32.0 KB | `77dd7926bbf4e96f4d5c84fe30ef2ff1` | Factory Binary Firmware Dump |
| `0280-000-954.BIN` | **2000–2024** | 32.0 KB | `a7ee63b62a8c27820018b85eb8a2d04e` | Factory Binary Firmware Dump |
| `0280-000-962.BIN` | **2000–2024** | 32.0 KB | `aced46ff3dd6671e65f30221fbe65bbf` | Factory Binary Firmware Dump |
| `Bensin 984 chip 1 037 358 931.bin` | **2000–2024** | 32.0 KB | `da50f84b31fd0fb26e1921d7de80f371` | Factory Binary Firmware Dump |
| `Volvo_556.xdf` | **2000–2024** | 8.6 KB | `4e93076613a1524add8e97ee10caaaf8` | TunerPro Binary Definition Map |
| `Volvo_560.xdf` | **2000–2024** | 8.4 KB | `ee23511ef143e130171b1818c6303823` | TunerPro Binary Definition Map |
| `Volvo_913.xdf` | **2000–2024** | 10.9 KB | `e34bc384fe96f4f70b75043783336d89` | TunerPro Binary Definition Map |
| `Volvo_954_LH2.4.xdf` | **2000–2024** | 10.4 KB | `eb0c61620d74a2f105ee425d31d155cf` | TunerPro Binary Definition Map |
| `Volvo_962.xdf` | **2000–2024** | 9.6 KB | `06527829d32aa08980389feb24b71577` | TunerPro Binary Definition Map |
| `Volvo_EZK_208.xdf` | **2000–2024** | 12.7 KB | `3dd816f0a5e72a52ca64f10979c76c48` | TunerPro Binary Definition Map |
| `Volvo_LH22_511.xdf` | **2000–2024** | 4.0 KB | `bd27658f8d7bc79f7f5a5ad238c109a0` | TunerPro Binary Definition Map |
| `Volvo_LH22_554.xdf` | **2000–2024** | 5.2 KB | `66136499f03c8a884b3954ad9a749513` | TunerPro Binary Definition Map |
| `Volvo_LH24_937.xdf` | **2000–2024** | 9.0 KB | `9a4b7d1894974fd9c6bf081774eb13ec` | TunerPro Binary Definition Map |
| `lh2.2 NA 511.BIN` | **2000–2024** | 4.0 KB | `c78d51ee419ab6fa10719d12a93f5265` | Factory Binary Firmware Dump |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi yang tersedia, struktur kalibrasi mencakup parameter esensial:
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
