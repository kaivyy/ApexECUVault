# SIEMENS_MS43 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/SIEMENS_MS43`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `39 files` (19 binary dumps, 20 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SIEMENS_MS43` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `4323T110.A2L` | **2000–2006** | 1.55 MB | `72bc27a5276c77e7ff4f4d4fd7a1da78` | ASAM ASAP2 ECU Description File |
| `43250010.A2L` | **2000–2006** | 1.55 MB | `ca2eec6cff9ee3fc396fd47eb660ebc4` | ASAM ASAP2 ECU Description File |
| `75181111.bin` | **2000–2006** | 512.0 KB | `cbb44997c374a208a69d74db55499a81` | Factory Binary Firmware Dump |
| `MS43 ECU Definitions.xml` | **2000–2006** | 501.7 KB | `3fbffadae49da2579d0b4304fab58f36` | ECU / XML Calibration Map Definition |
| `MS43 logger_METRIC_EN_v1.0.0 - ext load.xml` | **2000–2006** | 61.4 KB | `7456c4fde0fc45ef80b23bbb2f3318d1` | ECU / XML Calibration Map Definition |
| `MS43 logger_METRIC_EN_v1.0.0.xml` | **2000–2006** | 63.3 KB | `a0480f4b0131bad132eeaa189e19328d` | ECU / XML Calibration Map Definition |
| `Siemens_MS43_MS430037_ENG_512K_v1.16.xdf` | **2000–2006** | 3.16 MB | `39aa2118fc25922b1d7f6bfb8862e11b` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430037_ENG_64K_v1.16.xdf` | **2000–2006** | 3.16 MB | `d56059ac08e66b012b946aaae9eed8e2` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430055_ENG_512K_v1.16.xdf` | **2000–2006** | 3.34 MB | `64010ecc11144ecf2bf179730a57a643` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430055_ENG_64K_v1.16.xdf` | **2000–2006** | 3.34 MB | `f487ad319c0c4aefcce5e1cc9b02fd9b` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430056_ENG_512K_v1.16.xdf` | **2000–2006** | 3.35 MB | `ad8a8554eb172a4bf335ef4e79a5f580` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430056_ENG_64K_v1.16.xdf` | **2000–2006** | 3.35 MB | `214ff239fbff9cceee4b72b63c303122` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430064_ENG_512K_v1.16.xdf` | **2000–2006** | 3.40 MB | `ea7a79a2544f2457040b76ab6d860627` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430064_ENG_64K_v1.16.xdf` | **2000–2006** | 3.40 MB | `185f72de927af4fd7963467a07916078` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430066_ENG_512K_v1.16.xdf` | **2000–2006** | 3.45 MB | `fcce5093a7d621f4a81da367831290d7` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430066_ENG_64K_v1.16.xdf` | **2000–2006** | 3.45 MB | `b13b98d40264d6a158a07b0091199a98` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430069_E36Z3_M54B30_EU4_LHD.bin` | **2000–2006** | 512.0 KB | `b93a6675b398a6bc8dcc732549c2e60b` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E39_M54B25_EU4_LHD.bin` | **2000–2006** | 512.0 KB | `7c4e471d443bc2055c83b05dd38f8c80` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E39_M54B30_EU4_LHD.bin` | **2000–2006** | 512.0 KB | `5197fec31152da5de4f22d39074d8b28` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E39_M54B30_US.bin` | **2000–2006** | 512.0 KB | `75c410b9c3659a22cb92c2be5ae76684` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_Compact_M54B25_EU4_LHD.bin` | **2000–2006** | 512.0 KB | `eecf6335d69142189145b5d2cfbe036c` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M52TUB28_EU4_LHD.bin` | **2000–2006** | 512.0 KB | `7e921d9fa1e7c288c99bbb8aa5cba433` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B22_EU4_LHD.bin` | **2000–2006** | 512.0 KB | `a474d2fbd7bbb1f076a769ab2029199c` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B22_EU4_RHD.bin` | **2000–2006** | 512.0 KB | `01f76d3da8eb648a733d5d14da0f2f1d` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B25_EU4_LHD.bin` | **2000–2006** | 512.0 KB | `58258b4b68c930c2c8a70dc70b297b88` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B25_EU4_RHD.bin` | **2000–2006** | 512.0 KB | `4ebd5f21bdac7ce8b535ef1ab3c495de` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B25_US.bin` | **2000–2006** | 512.0 KB | `318ea6f5c9c971b48eede0196973a7e0` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B30_EU2_LHD.bin` | **2000–2006** | 512.0 KB | `1308a402af223aa825395df6af1d4a97` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B30_EU2_RHD.bin` | **2000–2006** | 512.0 KB | `af86cf1fcae8af46909564b97ec0cb71` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B30_EU4_LHD.bin` | **2000–2006** | 512.0 KB | `49417e0f6515524be45073cf0d5d45b7` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B30_EU4_RHD.bin` | **2000–2006** | 512.0 KB | `309fccfad0d412a9f4ff09af341862d4` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E46_M54B30_US.bin` | **2000–2006** | 512.0 KB | `d70b06a1023c6a91dbbfc0bdda60c315` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E53_M54B30_EU4.bin` | **2000–2006** | 512.0 KB | `c8c491f997325464272c5d5ff391f1a2` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_E53_M54B30_US.bin` | **2000–2006** | 512.0 KB | `681f9e1fc39fa1f702ceb450a3ebfdaa` | Factory Binary Firmware Dump |
| `Siemens_MS43_MS430069_ENG_512K_v1.16.xdf` | **2000–2006** | 3.46 MB | `4097caa745dab52b30a2db724f51df77` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430069_ENG_64K_v1.16.xdf` | **2000–2006** | 3.46 MB | `d4de4a07963a2bd9adb90d64f80e0140` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430069_ExtendedLoad_ENG_512K_v1.16.xdf` | **2000–2006** | 3.46 MB | `21882f07dd6d4ac064f4cc7d608a1816` | TunerPro Binary Definition Map |
| `Siemens_MS43_MS430069_ExtendedLoad_ENG_64K_v1.16.xdf` | **2000–2006** | 3.46 MB | `929bad2913fe0b9c0bb9bdbc35a8bb3d` | TunerPro Binary Definition Map |
| `ms43.ols` | **2000–2006** | 1.99 MB | `5df0bb0ee14d0085f30c9d74f39e7075` | WinOLS Project Workspace |

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
