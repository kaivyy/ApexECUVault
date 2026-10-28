# MSS54HP - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_MSS54_M3_CSL/03_BIN_PARTIAL_CALIBRATIONS/MSS54HP`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `42 files` (42 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MSS54HP` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2006

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `211323001601J424 (EU3 6MT).bin` | **2000–2006** | 64.0 KB | `96e091b76578c430609678cb8a4bc129` | Factory Binary Firmware Dump |
| `211323001601J429 (US 6MT non-heated DMTL).bin` | **2000–2006** | 64.0 KB | `b8c481d6c862c4ba25120d0d2562db56` | Factory Binary Firmware Dump |
| `211323001601J444 (NoEOBD 6MT).bin` | **2000–2006** | 64.0 KB | `78f1e65c2bb089b4bcff4344924fd644` | Factory Binary Firmware Dump |
| `211323001601J449 (Japan 6MT).bin` | **2000–2006** | 64.0 KB | `307da5a9a857412e18f5924f87fa0307` | Factory Binary Firmware Dump |
| `211323001601J464 (Low Compression 6MT).bin` | **2000–2006** | 64.0 KB | `e6255a0ea38b957d364904e0d33c3ef3` | Factory Binary Firmware Dump |
| `211323001601J469 (US 6MT heated DMTL).bin` | **2000–2006** | 64.0 KB | `94e676daa98fc4ba3c5d74228bb3c5bd` | Factory Binary Firmware Dump |
| `211323001601JD34 (EU3 SMG).bin` | **2000–2006** | 64.0 KB | `88ca66294562f14f5c9d7e801733b935` | Factory Binary Firmware Dump |
| `211323001601JD39 (US SMG non-heated DMTL).bin` | **2000–2006** | 64.0 KB | `3d363ad975ae959c54a844a1b59ee93c` | Factory Binary Firmware Dump |
| `211323001601JD54 (NoEOBD SMG).bin` | **2000–2006** | 64.0 KB | `7585fec3e6c900ee38268edbd53675b6` | Factory Binary Firmware Dump |
| `211323001601JD59 (Japan SMG).bin` | **2000–2006** | 64.0 KB | `d988246dfa92b22bb1cbada9859b7d1c` | Factory Binary Firmware Dump |
| `211323001601JD74 (EU3 Low Compression SMG).bin` | **2000–2006** | 64.0 KB | `3376253297257c5e3b3e75ccac1de0a5` | Factory Binary Firmware Dump |
| `211323001601JD79 (US SMG heated DMTL).bin` | **2000–2006** | 64.0 KB | `9af7979d8e506aa2dc21dfd8e9706bd2` | Factory Binary Firmware Dump |
| `211323001801J424 (EU3 6MT).bin` | **2000–2006** | 64.0 KB | `ce5831f53c5824e23dc324109efc10c0` | Factory Binary Firmware Dump |
| `211323001801J444 (NoEOBD 6MT).bin` | **2000–2006** | 64.0 KB | `426a61c7305b2a0de51be7eedf7676c7` | Factory Binary Firmware Dump |
| `211323001801J449 (Japan 6MT).bin` | **2000–2006** | 64.0 KB | `33c393a43223c4927b93efdd3ab97e88` | Factory Binary Firmware Dump |
| `211323001801J464 (Low Compression 6MT).bin` | **2000–2006** | 64.0 KB | `c8c15cca99f199b4e5b81374806226f2` | Factory Binary Firmware Dump |
| `211323001801J469 (US 6MT heated DMTL).bin` | **2000–2006** | 64.0 KB | `67bfb005979272dc2840a4134196a866` | Factory Binary Firmware Dump |
| `211323001801J489.bin` | **2000–2006** | 64.0 KB | `963ff9299dda9ab72e5f81e83dbf3b8b` | Factory Binary Firmware Dump |
| `211323001801JD34 (EU3 SMG).bin` | **2000–2006** | 64.0 KB | `d9f607e4ad79826d9046040805d204af` | Factory Binary Firmware Dump |
| `211323001801JD54 (NoEOBD SMG).bin` | **2000–2006** | 64.0 KB | `70dbd90b4820b343b2339b4c745bf459` | Factory Binary Firmware Dump |
| `211323001801JD59 (Japan SMG).bin` | **2000–2006** | 64.0 KB | `7ff08a4054eb84e7d6147444db921b1e` | Factory Binary Firmware Dump |
| `211323001801JD74 (EU3 Low Compression SMG).bin` | **2000–2006** | 64.0 KB | `75f801ff4fcf73a54a1d13782b074179` | Factory Binary Firmware Dump |
| `211323001801JD79 (US SMG heated DMTL).bin` | **2000–2006** | 64.0 KB | `8c896bbd3dc2356cb6013848bb10422a` | Factory Binary Firmware Dump |
| `211323001801JD99 (US SMG).bin` | **2000–2006** | 64.0 KB | `654f5a2d825e1aeb6ac92e66e6cef1e8` | Factory Binary Firmware Dump |
| `211323002001J424 (EU3 6MT).bin` | **2000–2006** | 64.0 KB | `3a57e6b9bfeb986458bc6cdb5ca09c18` | Factory Binary Firmware Dump |
| `211323002001J444 (NoEOBD 6MT).bin` | **2000–2006** | 64.0 KB | `598e09c576429b3f86fe922369d76c08` | Factory Binary Firmware Dump |
| `211323002001J449 (Japan 6MT).bin` | **2000–2006** | 64.0 KB | `fd2d6cb7d1dc06af8d81838fed0f726f` | Factory Binary Firmware Dump |
| `211323002001J464 (Low Compression 6MT).bin` | **2000–2006** | 64.0 KB | `070d89cc148ed9ac025eb69845e63923` | Factory Binary Firmware Dump |
| `211323002001J469 (US 6MT heated DMTL).bin` | **2000–2006** | 64.0 KB | `1d14b4024e6851976ca65ab99f0f4856` | Factory Binary Firmware Dump |
| `211323002001J484 (EU4 6MT).bin` | **2000–2006** | 64.0 KB | `78a1a80216a9c63b687f8a3866badf49` | Factory Binary Firmware Dump |
| `211323002001JD34 (EU3 SMG).bin` | **2000–2006** | 64.0 KB | `b5319745e52e9b1b1426fbf76eb78aaf` | Factory Binary Firmware Dump |
| `211323002001JD54 (NoEOBD SMG).bin` | **2000–2006** | 64.0 KB | `a6f86dcbeb38783466703ab840519437` | Factory Binary Firmware Dump |
| `211323002001JD59 (Japan SMG).bin` | **2000–2006** | 64.0 KB | `83da81bb456163a5af86c99ccf8e7357` | Factory Binary Firmware Dump |
| `211323002001JD74 (EU3 Low Compression SMG).bin` | **2000–2006** | 64.0 KB | `073df06b0994a99b024fda83750647ec` | Factory Binary Firmware Dump |
| `211323002001JD94 (EU4 SMG).bin` | **2000–2006** | 64.0 KB | `5f3481ca24ae9218cf88c629a611c5c8` | Factory Binary Firmware Dump |
| `211323002501J469 (US 6MT heated DMTL).bin` | **2000–2006** | 64.0 KB | `0f12bccd43f140a34f3e215453943d84` | Factory Binary Firmware Dump |
| `211323002501JD39 (US SMG non-heated DMTL).bin` | **2000–2006** | 64.0 KB | `9bfb9e0d317b728cd33658dfe132d29d` | Factory Binary Firmware Dump |
| `211323002501JD79 (US SMG heated DMTL).bin` | **2000–2006** | 64.0 KB | `5581e8eacc2829b5133253e73b6e8016` | Factory Binary Firmware Dump |
| `211323002701J429 (US 6MT non-heated DMTL).bin` | **2000–2006** | 64.0 KB | `172fdef9471517dda8c56245aabdf9ff` | Factory Binary Firmware Dump |
| `211323002701J469 (US 6MT heated DMTL).bin` | **2000–2006** | 64.0 KB | `bebec2988ad3989af1d05360c70fecee` | Factory Binary Firmware Dump |
| `211323002701JD39 (US SMG non-heated DMTL).bin` | **2000–2006** | 64.0 KB | `36be49e41a7b7b581d81fec018a740ef` | Factory Binary Firmware Dump |
| `211323002701JD79 (US SMG heated DMTL).bin` | **2000–2006** | 64.0 KB | `098cc0ff66d2c3031168ed615247ee6b` | Factory Binary Firmware Dump |

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
