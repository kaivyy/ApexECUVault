# MSS54 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_MSS54_M3_CSL/03_BIN_PARTIAL_CALIBRATIONS/MSS54`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `37 files` (37 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MSS54` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `211322000701J404.bin` | **2000–2006** | 32.0 KB | `cf069c06b1d747571dbe3bd2dd5903c6` | Factory Binary Firmware Dump |
| `211322000701J409.bin` | **2000–2006** | 32.0 KB | `2d7b2827125d09a09631eca4c1e24521` | Factory Binary Firmware Dump |
| `211322000701QD04.bin` | **2000–2006** | 32.0 KB | `37b44bbb4a00f0ce40264e0fd29b6e4e` | Factory Binary Firmware Dump |
| `211322000701QD09.bin` | **2000–2006** | 32.0 KB | `4e334fc013b1f9843d96ecf4f179e341` | Factory Binary Firmware Dump |
| `211322001501J424 (EU3 6MT).bin` | **2000–2006** | 32.0 KB | `796a1e707e1d9b0d8549a09b6169182a` | Factory Binary Firmware Dump |
| `211322001501J444 (NoEOBD 6MT).bin` | **2000–2006** | 32.0 KB | `af8b03abaab4360d079fed5b0edc2e57` | Factory Binary Firmware Dump |
| `211322001501J449 (Japan 6MT).bin` | **2000–2006** | 32.0 KB | `a0458c0597f45b940d9f8665d8d883bd` | Factory Binary Firmware Dump |
| `211322001501J464 (Low Compression 6MT).bin` | **2000–2006** | 32.0 KB | `5243fc0b991fc5375066a8b899be8fc5` | Factory Binary Firmware Dump |
| `211322001501J4E9.bin` | **2000–2006** | 32.0 KB | `bf57c35a0cf4b8a9dc9eb330e28caa44` | Factory Binary Firmware Dump |
| `211322001501J4G9.bin` | **2000–2006** | 32.0 KB | `746a98264f1d271570fe3b7829ad5c0b` | Factory Binary Firmware Dump |
| `211322001501JD34 (EU3 SMG).bin` | **2000–2006** | 32.0 KB | `249cdf5f73bc2770ff6bdb696cf174a6` | Factory Binary Firmware Dump |
| `211322001501JD54 (NoEOBD SMG).bin` | **2000–2006** | 32.0 KB | `642d042d2951f70e632c61151a06f72f` | Factory Binary Firmware Dump |
| `211322001501JD59 (Japan SMG).bin` | **2000–2006** | 32.0 KB | `3e8013f84401c6d4223428da56ac1426` | Factory Binary Firmware Dump |
| `211322001501JD74 (EU3 Low Compression SMG).bin` | **2000–2006** | 32.0 KB | `748b7c0e8aee81982a015a98f1dcfef0` | Factory Binary Firmware Dump |
| `211322001501JDD9 (US SMG).bin` | **2000–2006** | 32.0 KB | `ca4d05384c09dc6722d23d3cf1f13146` | Factory Binary Firmware Dump |
| `211322001501JDF9 (US SMG).bin` | **2000–2006** | 32.0 KB | `10ab216f1d4655334325bd29426d64e6` | Factory Binary Firmware Dump |
| `211322001701JD34 (EU3 SMG).bin` | **2000–2006** | 32.0 KB | `d6b6504cf2f281f1f67ccd65acebb246` | Factory Binary Firmware Dump |
| `211322002101J424 (EU3 6MT).bin` | **2000–2006** | 32.0 KB | `6e6ab25de1f67129be04dde6df56d33d` | Factory Binary Firmware Dump |
| `211322002101J444 (NoEOBD 6MT).bin` | **2000–2006** | 32.0 KB | `a2a54c08d89596bbf65e6d26c3aa17ba` | Factory Binary Firmware Dump |
| `211322002101J449 (Japan 6MT).bin` | **2000–2006** | 32.0 KB | `058f0cb68ea6208f59a7945ec34088ab` | Factory Binary Firmware Dump |
| `211322002101J464 (Low Compression 6MT).bin` | **2000–2006** | 32.0 KB | `7f84e668f04be3275ebbd186e9819b02` | Factory Binary Firmware Dump |
| `211322002101J469 (US 6MT heated DMTL).bin` | **2000–2006** | 32.0 KB | `edb35cf30ae97f2b5967bb8bdbb5cf62` | Factory Binary Firmware Dump |
| `211322002101JD34 (EU3 SMG).bin` | **2000–2006** | 32.0 KB | `6fb86d4bad81b41ffea0fd7fe40f1b0f` | Factory Binary Firmware Dump |
| `211322002101JD54 (NoEOBD SMG).bin` | **2000–2006** | 32.0 KB | `76b838de2c109669d37d33a2c22ac218` | Factory Binary Firmware Dump |
| `211322002101JD59 (Japan SMG).bin` | **2000–2006** | 32.0 KB | `7cf1a1c69ee7b6389d12829f01130f9e` | Factory Binary Firmware Dump |
| `211322002101JD74 (EU3 Low Compression SMG).bin` | **2000–2006** | 32.0 KB | `861c68c6c20926dc3af02bb18d46984b` | Factory Binary Firmware Dump |
| `211322002101Q424 (EU Z3M).bin` | **2000–2006** | 32.0 KB | `ab152372029bb24b181e78763c239a91` | Factory Binary Firmware Dump |
| `211322002101Q444 (NoEOBD Z3M).bin` | **2000–2006** | 32.0 KB | `715e3ff4ad2c22c9a91479cc3bf5feba` | Factory Binary Firmware Dump |
| `211322002101Q449 (Japan Low Compression Z3M).bin` | **2000–2006** | 32.0 KB | `30d6221993241c1692e264596525b0c4` | Factory Binary Firmware Dump |
| `211322002101Q464 (Low Compression Z3M).bin` | **2000–2006** | 32.0 KB | `d9110340dad2c097b2fe91231ef7a254` | Factory Binary Firmware Dump |
| `211322002601JD39 (US SMG non-heated DMTL).bin` | **2000–2006** | 32.0 KB | `f29eb89a221087055112b2628f6292b2` | Factory Binary Firmware Dump |
| `211322002601JD79 (US SMG heated DMTL).bin` | **2000–2006** | 32.0 KB | `e649c5fd26803643f5ed6bd5cc0eaa98` | Factory Binary Firmware Dump |
| `211322002801J429 (US 6MT non-heated DMTL).bin` | **2000–2006** | 32.0 KB | `3f05fd1f085d2ffc7a9638e693bf3ead` | Factory Binary Firmware Dump |
| `211322002801J469 (US 6MT heated DMTL).bin` | **2000–2006** | 32.0 KB | `584872b53de3eb103fe9f5984a4069af` | Factory Binary Firmware Dump |
| `211322002801JD39 (US SMG non-heated DMTL).bin` | **2000–2006** | 32.0 KB | `815233c002f9478c3695a522de3167f7` | Factory Binary Firmware Dump |
| `211322002801JD79 (US SMG heated DMTL).bin` | **2000–2006** | 32.0 KB | `265c5d828f365e3a879072190d780eb9` | Factory Binary Firmware Dump |
| `211322002801Q429 (US Z3M).bin` | **2000–2006** | 32.0 KB | `1b4fe91c349bbb431fe7bfc87f75189c` | Factory Binary Firmware Dump |

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
