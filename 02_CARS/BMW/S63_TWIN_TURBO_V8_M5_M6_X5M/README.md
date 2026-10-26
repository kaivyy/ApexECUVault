# S63 TWIN TURBO V8 M5 M6 X5M - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/S63_TWIN_TURBO_V8_M5_M6_X5M`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `28 files` (14 binary dumps, 14 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `S63_TWIN_TURBO_V8_M5_M6_X5M` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `000010CA3B8C01.xdf` | **OEM Production** | 637.8 KB | `861268aff0abe27b2e1e1c0a106039aa` | TunerPro Binary Definition Map |
| `000010CA3B8C01_original.bin` | **OEM Production** | 4.00 MB | `0dd83e918f3df32d04c462b535ea0d9e` | Factory Binary Firmware Dump |
| `000010CA598C01.xdf` | **OEM Production** | 630.3 KB | `40b2fb3ad1d325d622f69ae1027eaa8a` | TunerPro Binary Definition Map |
| `000010CA598C01_original.bin` | **OEM Production** | 4.00 MB | `9cfe95ad86ad74f8151117a24d8f3c7f` | Factory Binary Firmware Dump |
| `00004ACF0A3204.xdf` | **OEM Production** | 652.5 KB | `e45669d4d52dc60cb6bcc2d4276c0bd1` | TunerPro Binary Definition Map |
| `00004ACF0A3204_original.bin` | **OEM Production** | 8.00 MB | `1559258c9e0f7fd228e6efa5a999e9c7` | Factory Binary Firmware Dump |
| `00004ACF147803.xdf` | **OEM Production** | 658.1 KB | `597d4bfdc8ad2fb5efc492f2482aa481` | TunerPro Binary Definition Map |
| `00004ACF147803_original.bin` | **OEM Production** | 8.00 MB | `4503527b93e6ce592a9b8595622830ab` | Factory Binary Firmware Dump |
| `00004ACF1E6E05.xdf` | **OEM Production** | 652.7 KB | `2af11ea732261b5db6d559bf829bf15f` | TunerPro Binary Definition Map |
| `00004ACF1E6E05_original.bin` | **OEM Production** | 8.00 MB | `d0427f59c1135ea4ad7d48258455c94b` | Factory Binary Firmware Dump |
| `00004ACF1E7805.xdf` | **OEM Production** | 652.7 KB | `d6dc97ead974b74fd3ccac0d6d8a7934` | TunerPro Binary Definition Map |
| `00004ACF1E7805_original.bin` | **OEM Production** | 8.00 MB | `7f18fe0e6354407fbdf2b5a7133bd19f` | Factory Binary Firmware Dump |
| `00004ACF1E9605.xdf` | **OEM Production** | 652.7 KB | `8169ad83c416affb11fc9e7850783ad2` | TunerPro Binary Definition Map |
| `00004ACF1E9605_original.bin` | **OEM Production** | 8.00 MB | `d768576241ff96359ae416d0d9d181f5` | Factory Binary Firmware Dump |
| `00004ACF1EA006.xdf` | **OEM Production** | 652.7 KB | `81e91047b1b1716abec60567ff716733` | TunerPro Binary Definition Map |
| `00004ACF1EA006_original.bin` | **OEM Production** | 8.00 MB | `11c6ca46da75524b22523e50ab677bb4` | Factory Binary Firmware Dump |
| `00004ACF1EAA05.xdf` | **OEM Production** | 652.7 KB | `4df2808f53aa64558113ba51af40cc51` | TunerPro Binary Definition Map |
| `00004ACF1EAA05_original.bin` | **OEM Production** | 8.00 MB | `975835652e81499e12b19290df85279a` | Factory Binary Firmware Dump |
| `00004ACF1EB405.xdf` | **OEM Production** | 652.7 KB | `722a52dae76eede311b47d0656f023a1` | TunerPro Binary Definition Map |
| `00004ACF1EB405_original.bin` | **OEM Production** | 8.00 MB | `9aebadd1dc558eb08cfe0998d774af8e` | Factory Binary Firmware Dump |
| `00004ACF286E05.xdf` | **OEM Production** | 674.0 KB | `2609741adfc5c4b7d4d2312736597cfa` | TunerPro Binary Definition Map |
| `00004ACF286E05_original.bin` | **OEM Production** | 8.00 MB | `53973a1ccd7cc1f76a2a62f4ea60c224` | Factory Binary Firmware Dump |
| `00004ACF287806.xdf` | **OEM Production** | 674.0 KB | `5ef31f1d7441b1f631707ffee1a08f4e` | TunerPro Binary Definition Map |
| `00004ACF287806_original.bin` | **OEM Production** | 8.00 MB | `4ba04ce3d33efc8b5778600ead64a118` | Factory Binary Firmware Dump |
| `00004ACF288205.xdf` | **OEM Production** | 674.0 KB | `8009651bb5cd1a1471b66ee685baba4b` | TunerPro Binary Definition Map |
| `00004ACF288205_original.bin` | **OEM Production** | 8.00 MB | `cc01cfde49cb1b81baf5b87bdbafd43e` | Factory Binary Firmware Dump |
| `00004ACF289605.xdf` | **OEM Production** | 674.0 KB | `91f1f262280ee2dc0736a85c484b837c` | TunerPro Binary Definition Map |
| `00004ACF289605_original.bin` | **OEM Production** | 8.00 MB | `4d3d4d8ac5a72be4042a9648e209b05e` | Factory Binary Firmware Dump |

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
