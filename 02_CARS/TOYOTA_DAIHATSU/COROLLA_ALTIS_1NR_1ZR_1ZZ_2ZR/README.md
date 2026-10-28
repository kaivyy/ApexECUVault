# COROLLA_ALTIS_1NR_1ZR_1ZZ_2ZR - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/COROLLA_ALTIS_1NR_1ZR_1ZZ_2ZR`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `13 files` (13 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `COROLLA_ALTIS_1NR_1ZR_1ZZ_2ZR` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2001–2022

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `89663-02023.bin` | **2001–2022** | 320.0 KB | `5ddef7c2ce9c5abbefa2cb8777628d13` | Factory Binary Firmware Dump |
| `89663-02161.bin` | **2001–2022** | 320.0 KB | `d1ae6fb54e61566ae61e4056154def06` | Factory Binary Firmware Dump |
| `89663-02162.bin` | **2001–2022** | 320.0 KB | `dcbe18885ef74606548a923362f147b5` | Factory Binary Firmware Dump |
| `89663-02172.bin` | **2001–2022** | 320.0 KB | `bb4c9d3fb90a71d01256df472084d983` | Factory Binary Firmware Dump |
| `89663-02173.bin` | **2001–2022** | 320.0 KB | `aa21e2bea3f428607d36e113fc6167dc` | Factory Binary Firmware Dump |
| `89663-02241.bin` | **2001–2022** | 368.0 KB | `9bc2041a3ec839cfd9c8017fd72d77ff` | Factory Binary Firmware Dump |
| `89663-02270.bin` | **2001–2022** | 368.0 KB | `d1f80cabcd6dd3a2cf2be553de6f1e8e` | Factory Binary Firmware Dump |
| `89663-02482.bin` | **2001–2022** | 496.0 KB | `2dd339b573686fbc28c6698133ba16bf` | Factory Binary Firmware Dump |
| `89663-02502.bin` | **2001–2022** | 496.0 KB | `69b5ac8f844408bc29de9180f4c4e603` | Factory Binary Firmware Dump |
| `89663-02661.bin` | **2001–2022** | 736.0 KB | `d8cc949db374e6eea05971f1892a1efc` | Factory Binary Firmware Dump |
| `89663-02E73.bin` | **2001–2022** | 992.0 KB | `01c750bb362506d8026022a952303b60` | Factory Binary Firmware Dump |
| `89663-02J13.bin` | **2001–2022** | 736.0 KB | `4206fdd3371c26cdeee436b3c26d6c24` | Factory Binary Firmware Dump |
| `89663-02J22.bin` | **2001–2022** | 736.0 KB | `3d4a843cdf1faf04d594e6aa9f62ea05` | Factory Binary Firmware Dump |

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
