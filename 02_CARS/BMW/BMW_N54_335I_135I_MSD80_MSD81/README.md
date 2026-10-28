# BMW_N54_335I_135I_MSD80_MSD81 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/BMW_N54_335I_135I_MSD80_MSD81`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `47 files` (34 binary dumps, 13 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `BMW_N54_335I_135I_MSD80_MSD81` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2006–2010

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `37EIRD05.hex` | **2006–2010** | 616.1 KB | `124467ff87d4d379433fa8be66c2f884` | Intel HEX Calibration Firmware |
| `568313_D.org.bin` | **2006–2010** | 249.8 KB | `1247ec230b65acc7afa396af3b3f7253` | Factory Binary Firmware Dump |
| `568317_D.org.bin` | **2006–2010** | 249.8 KB | `c53dc9ded4094ca6e0cc230803d02230` | Factory Binary Firmware Dump |
| `568319_D.org.bin` | **2006–2010** | 249.8 KB | `6c871dc5f94e586f7b018b2c6fe06e21` | Factory Binary Firmware Dump |
| `568863_D.org.bin` | **2006–2010** | 249.8 KB | `1e6625d504c43d1caf405653ed272c21` | Factory Binary Firmware Dump |
| `568865_D.org.bin` | **2006–2010** | 249.8 KB | `3655bd621a48a8b03fcab6989ac30771` | Factory Binary Firmware Dump |
| `568867_D.org.bin` | **2006–2010** | 249.8 KB | `d8764ed4cf1dd92a2c117eec99ccd608` | Factory Binary Firmware Dump |
| `568869_D.org.bin` | **2006–2010** | 249.8 KB | `6298a624636ef707e13254c0e077e45f` | Factory Binary Firmware Dump |
| `571553_D.org.bin` | **2006–2010** | 249.8 KB | `e957f09f5cfd3f81a4259381337ecc2f` | Factory Binary Firmware Dump |
| `571555_D.org.bin` | **2006–2010** | 249.8 KB | `886ce63033d2b0d25877ed11e8e8daf0` | Factory Binary Firmware Dump |
| `571557_D.org.bin` | **2006–2010** | 249.8 KB | `0de7c18372b1743e217037516ce10ad2` | Factory Binary Firmware Dump |
| `571559_D.org.bin` | **2006–2010** | 249.8 KB | `bad5db5f7fbdf82022d389fd4bc6d6ae` | Factory Binary Firmware Dump |
| `571561_D.org.bin` | **2006–2010** | 249.8 KB | `f018b92abb57eac79f69e0878def4b6e` | Factory Binary Firmware Dump |
| `571563_D.org.bin` | **2006–2010** | 249.8 KB | `39c1aa6e387d7fb854c94aca12eba0be` | Factory Binary Firmware Dump |
| `571565_D.org.bin` | **2006–2010** | 249.8 KB | `f172be97c32b536710bdec0e049d63b2` | Factory Binary Firmware Dump |
| `571567_D.org.bin` | **2006–2010** | 249.8 KB | `b70742d272ca49e6728504bf80fc0e71` | Factory Binary Firmware Dump |
| `571569_D.org.bin` | **2006–2010** | 249.8 KB | `15a3640a638d485c4e2d0c41d835ab18` | Factory Binary Firmware Dump |
| `571571_D.org.bin` | **2006–2010** | 249.8 KB | `948f65873edb407884fa8ba45dc2f6b8` | Factory Binary Firmware Dump |
| `571573_D.org.bin` | **2006–2010** | 249.8 KB | `b5612084cd41a6746476ec7042284f52` | Factory Binary Firmware Dump |
| `571575_D.org.bin` | **2006–2010** | 249.8 KB | `b5d830256e06a8c47e6b473b964f003d` | Factory Binary Firmware Dump |
| `571577_D.org.bin` | **2006–2010** | 249.8 KB | `cc21f3e93066a54e884b46b48ff0ec3e` | Factory Binary Firmware Dump |
| `571579_D.org.bin` | **2006–2010** | 249.8 KB | `2d2af3fdb9d489f038d3c9445e734498` | Factory Binary Firmware Dump |
| `571581_D.org.bin` | **2006–2010** | 249.8 KB | `6ed8e8ca26b3a157585149faf6ed69aa` | Factory Binary Firmware Dump |
| `791I200S.a2l` | **2006–2010** | 25.42 MB | `d06c55a3280e269ae8734fc8aed004fc` | ASAM ASAP2 ECU Description File |
| `80B37E0E.a2l` | **2006–2010** | 18.51 MB | `55ee25fd2841ba389f9bae9983b0e18f` | ASAM ASAP2 ECU Description File |
| `80B37I0E.a2l` | **2006–2010** | 18.50 MB | `be4c6f3c3c8568f26967526f4cf03d7c` | ASAM ASAP2 ECU Description File |
| `BMW_E90-E91, DAM_335i Turbo___5E62_.ols` | **2006–2010** | 6.02 MB | `51c13a93c68bc18cc8b47a5e668aab3e` | WinOLS Project Workspace |
| `I200S5X0 _791I200S_.hex` | **2006–2010** | 716.8 KB | `e815104038e38b83766a21341430f675` | Intel HEX Calibration Firmware |
| `I8A0S.xdf` | **2006–2010** | 1.06 MB | `fe61acf4f2f17fc29c0a6958ed7bba38` | TunerPro Binary Definition Map |
| `I8A0S_Legacy.xdf` | **2006–2010** | 674.8 KB | `824388ff095dbd1a4175a5a138605327` | TunerPro Binary Definition Map |
| `I8A0S_MapSwitchBase.bin` | **2006–2010** | 2.00 MB | `8a86b378007d508f7e6aef99199c0787` | Factory Binary Firmware Dump |
| `I8A0S_original.bin` | **2006–2010** | 2.00 MB | `b13d862b98e7ab3a9db9630287ca8f89` | Factory Binary Firmware Dump |
| `IJE0S.xdf` | **2006–2010** | 1.07 MB | `b60c3320fb71f2cdbcc799254f147c9c` | TunerPro Binary Definition Map |
| `IJE0S_Legacy.xdf` | **2006–2010** | 732.7 KB | `313401cf2e1166f02ff32ff6b75efe63` | TunerPro Binary Definition Map |
| `IJE0S_MapSwitchBase.bin` | **2006–2010** | 2.00 MB | `814231afd91ba2f09881d63be02d42f8` | Factory Binary Firmware Dump |
| `IJE0S_original.bin` | **2006–2010** | 2.00 MB | `0ece9d8f4e611dfea47c74862e5ce273` | Factory Binary Firmware Dump |
| `IKM0S.xdf` | **2006–2010** | 1.04 MB | `cc4f9f2c99c35d1e30f7b2235ec7c539` | TunerPro Binary Definition Map |
| `IKM0S_Legacy.xdf` | **2006–2010** | 695.1 KB | `a5442dd4d1093777fa5751417bc8ac75` | TunerPro Binary Definition Map |
| `IKM0S_MapSwitchBase.bin` | **2006–2010** | 2.00 MB | `dcea457d33a487d7ca4c20abbd4bf8b3` | Factory Binary Firmware Dump |
| `IKM0S_original.bin` | **2006–2010** | 2.00 MB | `83e0137005894071e935178d5cca44c0` | Factory Binary Firmware Dump |
| `INA0S.xdf` | **2006–2010** | 1.05 MB | `7d38bd739c8fac807d960708afaee9b6` | TunerPro Binary Definition Map |
| `INA0S_Legacy.xdf` | **2006–2010** | 718.1 KB | `ee528627452b0fd78dc4d31ed283ee90` | TunerPro Binary Definition Map |
| `INA0S_MapSwitchBase.bin` | **2006–2010** | 2.00 MB | `c2ffb0415b9d01a3d0c321db5bb9738c` | Factory Binary Firmware Dump |
| `INA0S_original.bin` | **2006–2010** | 2.00 MB | `09c7e7fad5ac497358ba1a85a24141c7` | Factory Binary Firmware Dump |
| `MSD 85 335I DAMOS.ols` | **2006–2010** | 6.20 MB | `a878f64c9f70701f83ee39fe37a396de` | WinOLS Project Workspace |
| `MSD80.bin` | **2006–2010** | 2.00 MB | `f8bfb226f4df5994808fe1d548762b08` | Factory Binary Firmware Dump |
| `WinOLS (1008.ols (Original) - ).bin` | **2006–2010** | 512.0 KB | `c0ee9869a128e7be13eb60bd770429f5` | Factory Binary Firmware Dump |

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
