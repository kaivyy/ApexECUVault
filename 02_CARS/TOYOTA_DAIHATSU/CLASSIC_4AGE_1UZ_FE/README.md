# CLASSIC_4AGE_1UZ_FE - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/CLASSIC_4AGE_1UZ_FE`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `51 files` (50 binary dumps, 1 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CLASSIC_4AGE_1UZ_FE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1984–1998

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `Copy of cap.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `GENERATIONAL_Toyota_4AGE_1UZFE_Denso_Classic.xdf` | **1984–1998** | 2.9 KB | `bddf521416401b71840dfcaec721a709` | TunerPro Binary Definition Map |
| `REMAP_STAGE1_Copy_of_cap.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_RAMtest.bin` | **1984–1998** | 1.0 KB | `82f389b63d815dc9bc6216c6b85abd70` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_Superbootloader+1uzbootcopy.bin` | **1984–1998** | 4.0 KB | `d820308444b1a29b9c2361335a773e9a` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_bigloaderF000.bin` | **1984–1998** | 4.0 KB | `9c79504c952cd0816139518cb0523eaf` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_bigloaderfromtiny.bin` | **1984–1998** | 1.0 KB | `5adbed7940e1556947d3cbb15cb51bd3` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_cap.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_cap1-151801-0642.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_cap2-151801-2860.bin` | **1984–1998** | 4.0 KB | `13e01ace0769cbe66c6b9a18541f8df7` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_cap_D151802-0442.bin` | **1984–1998** | 16.0 KB | `69331008563e7944a6f85bae0baeee1e` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_copytiny.bin` | **1984–1998** | 32.0 KB | `2f001f8abc14c07d4cf8cf90b3dc0010` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_reader.bin` | **1984–1998** | 32.0 KB | `c58d2aec4282fc0577d4bb5bb832f029` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_reader6301v1.bin` | **1984–1998** | 32.0 KB | `5e2b0fd4995b9d10fdf40d381c9e29c8` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_replacement.bin` | **1984–1998** | 4.0 KB | `730b18dd9113295f1fc522d7dc737284` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_test.bin` | **1984–1998** | 32.0 KB | `046c646188880f99d56e82669916340e` | Factory Binary Firmware Dump |
| `REMAP_STAGE1_tinyloader.bin` | **1984–1998** | 87 B | `24b601691e762b54a6fe6b62501a0533` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Copy_of_cap.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_RAMtest.bin` | **1984–1998** | 1.0 KB | `82f389b63d815dc9bc6216c6b85abd70` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Superbootloader+1uzbootcopy.bin` | **1984–1998** | 4.0 KB | `d820308444b1a29b9c2361335a773e9a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_bigloaderF000.bin` | **1984–1998** | 4.0 KB | `9c79504c952cd0816139518cb0523eaf` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_bigloaderfromtiny.bin` | **1984–1998** | 1.0 KB | `5adbed7940e1556947d3cbb15cb51bd3` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_cap.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_cap1-151801-0642.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_cap2-151801-2860.bin` | **1984–1998** | 4.0 KB | `13e01ace0769cbe66c6b9a18541f8df7` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_cap4.bin` | **1984–1998** | 4.1 KB | `fb05ac59c3a9afac045275d33aae1d5e` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_cap_D151802-0442.bin` | **1984–1998** | 16.0 KB | `69331008563e7944a6f85bae0baeee1e` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_cap_d151803-1320.bin` | **1984–1998** | 16.0 KB | `23dff67450800c6865d00c31db080320` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_cap_d151803-9260.bin` | **1984–1998** | 16.0 KB | `4ab634575fe8737e26b955ea48c6baeb` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_cap_d151804-8081.bin` | **1984–1998** | 16.0 KB | `f164bdbacfe86df9a168ca75240ef83e` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_copytiny.bin` | **1984–1998** | 32.0 KB | `2f001f8abc14c07d4cf8cf90b3dc0010` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_hacked9260.bin` | **1984–1998** | 16.0 KB | `499a5182c02bf81c982c7992d03a2068` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_reader.bin` | **1984–1998** | 32.0 KB | `c58d2aec4282fc0577d4bb5bb832f029` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_reader6301v1.bin` | **1984–1998** | 32.0 KB | `5e2b0fd4995b9d10fdf40d381c9e29c8` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_replacement.bin` | **1984–1998** | 4.0 KB | `730b18dd9113295f1fc522d7dc737284` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_test.bin` | **1984–1998** | 32.0 KB | `046c646188880f99d56e82669916340e` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_tinyloader.bin` | **1984–1998** | 87 B | `24b601691e762b54a6fe6b62501a0533` | Factory Binary Firmware Dump |
| `Superbootloader+1uzbootcopy.bin` | **1984–1998** | 4.0 KB | `d820308444b1a29b9c2361335a773e9a` | Factory Binary Firmware Dump |
| `cap D151802-0442.bin` | **1984–1998** | 16.0 KB | `69331008563e7944a6f85bae0baeee1e` | Factory Binary Firmware Dump |
| `cap d151803-1320.bin` | **1984–1998** | 16.0 KB | `23dff67450800c6865d00c31db080320` | Factory Binary Firmware Dump |
| `cap d151803-9260.bin` | **1984–1998** | 16.0 KB | `4ab634575fe8737e26b955ea48c6baeb` | Factory Binary Firmware Dump |
| `cap d151804-8081.bin` | **1984–1998** | 16.0 KB | `f164bdbacfe86df9a168ca75240ef83e` | Factory Binary Firmware Dump |
| `cap.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `cap1-151801-0642.bin` | **1984–1998** | 4.0 KB | `c4ecfacb0d17c6c5bf14ff8b9a2f089c` | Factory Binary Firmware Dump |
| `cap2-151801-2860.bin` | **1984–1998** | 4.0 KB | `13e01ace0769cbe66c6b9a18541f8df7` | Factory Binary Firmware Dump |
| `cap4.bin` | **1984–1998** | 4.1 KB | `fb05ac59c3a9afac045275d33aae1d5e` | Factory Binary Firmware Dump |
| `hacked9260.bin` | **1984–1998** | 16.0 KB | `499a5182c02bf81c982c7992d03a2068` | Factory Binary Firmware Dump |
| `reader.bin` | **1984–1998** | 32.0 KB | `c58d2aec4282fc0577d4bb5bb832f029` | Factory Binary Firmware Dump |
| `reader6301v1.bin` | **1984–1998** | 32.0 KB | `5e2b0fd4995b9d10fdf40d381c9e29c8` | Factory Binary Firmware Dump |
| `replacement.bin` | **1984–1998** | 4.0 KB | `730b18dd9113295f1fc522d7dc737284` | Factory Binary Firmware Dump |
| `test.bin` | **1984–1998** | 32.0 KB | `046c646188880f99d56e82669916340e` | Factory Binary Firmware Dump |

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
