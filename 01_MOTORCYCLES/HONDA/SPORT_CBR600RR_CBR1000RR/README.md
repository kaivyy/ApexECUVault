# HONDA CBR600RR & CBR1000RR FIREBLADE - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/SPORT_CBR600RR_CBR1000RR`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `98 files` (49 binary dumps, 49 definition maps)  

---

## 1. Technical Platform Overview

Koleksi komprehensif kalibrasi ECU OEM untuk lini supersport dan superbike Honda CBR600RR (PC37, PC40) dan CBR1000RR Fireblade (SC57, SC59, SC77, SC82). Meliputi pembacaan firmware flash biner asli pabrikan Keihin 256KB/1MB dan definisi TunerPro XDF untuk pemetaan bahan bakar PGM-FI, timing pengapian independen per silinder, kontrol katup knalpot (EXCV), dan kalibrasi pembatas putaran mesin (rev limiter).

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Keihin / Denso Multi-Cylinder Supersport ECM`
- **Arsitektur MCU & Memori**: `Renesas SH7058 / Motorola MC68HC16 / MPC500 series`
- **Protokol Diagnostik & Flashing**: `K-Line (ISO 14230 KWP2000) / HDS Proprietary / Bench Bootmode`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`, `0110C6`, `MS430069`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`, `32920-xxxxx`): Nomor resmi Denso MCU firmware flash untuk mobil dan motor.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx-xxxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **VAG Hardware / Software IDs** (misal `038906012xx`, `03G906021xx`, `8D0907558xx`): Nomor bagian resmi Volkswagen Audi Group untuk identifikasi kalibrasi mesin EDC15, EDC16, dan ME7.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2003–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `38770-MEE-612.bin` | **2003–2024** | 256.0 KB | `aecce9ae133d3dfd3bda9205f09f05ea` | Factory Binary Firmware Dump |
| `38770-MEE-622.bin` | **2003–2024** | 256.0 KB | `2742e3c741f55c578b81fea8c6fc6a6d` | Factory Binary Firmware Dump |
| `38770-MEE-F02.bin` | **2003–2024** | 256.0 KB | `cc6fdd6e9d2035cfb7af143e3642814b` | Factory Binary Firmware Dump |
| `38770-MEL-613.bin` | **2003–2024** | 256.0 KB | `a3547c584cc4e065b70ce8c98256510a` | Factory Binary Firmware Dump |
| `38770-MEL-643.bin` | **2003–2024** | 256.0 KB | `31bfcee982044e15831cfcdb5ce2a5fc` | Factory Binary Firmware Dump |
| `38770-MEL-672.bin` | **2003–2024** | 256.0 KB | `216ca37427461715240efac4ae495c6e` | Factory Binary Firmware Dump |
| `38770-MEL-772.bin` | **2003–2024** | 256.0 KB | `afe0a882abb63e22a6c1f66ecc3a00e3` | Factory Binary Firmware Dump |
| `38770-MEL-A21.bin` | **2003–2024** | 256.0 KB | `bff4a3e9c107241bb8bd649d88327993` | Factory Binary Firmware Dump |
| `38770-MEL-A22.bin` | **2003–2024** | 256.0 KB | `9a4aefc92652927b5de9de4a73dc6d71` | Factory Binary Firmware Dump |
| `38770-MEL-D01.bin` | **2003–2024** | 256.0 KB | `5317f766f02332817a51adac55950d7e` | Factory Binary Firmware Dump |
| `38770-MEL-D21.bin` | **2003–2024** | 256.0 KB | `3b5a0171e7a88090ec4465ec28426bad` | Factory Binary Firmware Dump |
| `38770-MEL-F21.bin` | **2003–2024** | 256.0 KB | `105661b8aebe610ea9789a1880c41daa` | Factory Binary Firmware Dump |
| `38770-MEL-L22.bin` | **2003–2024** | 256.0 KB | `822879077bf8bf50c3abef2a8674b2f8` | Factory Binary Firmware Dump |
| `38770-MEL.xdf` | **2003–2024** | 102.8 KB | `18eec9c7684c31c044c71c3ed5727f26` | TunerPro Binary Definition Map |
| `38770-MFJ-A02.bin` | **2003–2024** | 256.0 KB | `b061d41db86aec0e346967361250b344` | Factory Binary Firmware Dump |
| `38770-MFJ-D04.bin` | **2003–2024** | 256.0 KB | `9743fe4c0ffa263869cc6c405394ac0c` | Factory Binary Firmware Dump |
| `38770-MFJ-F03.bin` | **2003–2024** | 256.0 KB | `5de5263aa9d7767f26945e9cf85c272c` | Factory Binary Firmware Dump |
| `38770-MFL-622.bin` | **2003–2024** | 256.0 KB | `a469edb62eb524a0748be7aceaddacb7` | Factory Binary Firmware Dump |
| `38770-MFL-631.bin` | **2003–2024** | 256.0 KB | `77e25c0a36e4a69c919b33372860acd6` | Factory Binary Firmware Dump |
| `38770-MFL-644.bin` | **2003–2024** | 256.0 KB | `6dcb21f697b1a7da5b0884571536b4f6` | Factory Binary Firmware Dump |
| `38770-MFL-671.bin` | **2003–2024** | 256.0 KB | `f74c4d596481a581dcd23ac3d63f846f` | Factory Binary Firmware Dump |
| `38770-MFL-691.bin` | **2003–2024** | 256.0 KB | `d917325508447d48aa38cef35c409bc5` | Factory Binary Firmware Dump |
| `38770-MFL-702.bin` | **2003–2024** | 256.0 KB | `a9649caa83ed794ebe36a020fdc8178f` | Factory Binary Firmware Dump |
| `38770-MFL-741.bin` | **2003–2024** | 256.0 KB | `0f44e20d7dea5c95157cf41c5ebc6be0` | Factory Binary Firmware Dump |
| `38770-MFL-761.bin` | **2003–2024** | 256.0 KB | `9d08caf02fdead1e4647c3d0e73f9065` | Factory Binary Firmware Dump |
| `38770-MFL-773.bin` | **2003–2024** | 256.0 KB | `9f540444500d7f3da0c0384d10c461a6` | Factory Binary Firmware Dump |
| `38770-MFL-861.bin` | **2003–2024** | 256.0 KB | `8eb7c11f6cce6e4844896ecd56630ed6` | Factory Binary Firmware Dump |
| `38770-MFL-871.bin` | **2003–2024** | 256.0 KB | `b35a7c1edcf9c7d31c43a4545a4ad4f5` | Factory Binary Firmware Dump |
| `38770-MFL-A21.bin` | **2003–2024** | 256.0 KB | `566e5379f862e29064a7b6a61059ee73` | Factory Binary Firmware Dump |
| `38770-MFL-D21.bin` | **2003–2024** | 256.0 KB | `52dd1534dfe38eb2fddfe319b716c02c` | Factory Binary Firmware Dump |
| `38770-MFL-F21.bin` | **2003–2024** | 256.0 KB | `6ff2f8e2122134d6fdc0706730e821c9` | Factory Binary Firmware Dump |
| `38770-MFL-J21.bin` | **2003–2024** | 256.0 KB | `fc496239d752f563f05fe6756a02baf6` | Factory Binary Firmware Dump |
| `38770-MFL-J41.bin` | **2003–2024** | 256.0 KB | `06e127927748cdd87b21c6f78d6e4357` | Factory Binary Firmware Dump |
| `38770-MFL-L21.bin` | **2003–2024** | 256.0 KB | `cd5381d89fc000b0dd9c6d640a1eb754` | Factory Binary Firmware Dump |
| `38770-MGM-D11.bin` | **2003–2024** | 256.0 KB | `773d00c4f51ac9d5868d533aa3a85fe9` | Factory Binary Firmware Dump |
| `38770-MGP-A01.bin` | **2003–2024** | 256.0 KB | `f413f5bbb98943759172be4515d58a82` | Factory Binary Firmware Dump |
| `38770-MGP-A92.bin` | **2003–2024** | 256.0 KB | `328482096806497eecc516783ee3dbe8` | Factory Binary Firmware Dump |
| `38770-MGP-D01.bin` | **2003–2024** | 256.0 KB | `1f8694a9815a91e797da6a4013228cdb` | Factory Binary Firmware Dump |
| `38770-MGP-D62.bin` | **2003–2024** | 256.0 KB | `dea0de53cd2a0e7f5acb9b0c20b51ee3` | Factory Binary Firmware Dump |
| `38770-MGP-F01.bin` | **2003–2024** | 256.0 KB | `6ba0940cda716cccedcf902a6a0b2f8a` | Factory Binary Firmware Dump |
| `38770-MGP-F63.bin` | **2003–2024** | 256.0 KB | `f79fb005310ce70f0f8dd77cc02f5568` | Factory Binary Firmware Dump |
| `38770-MGP-L01.bin` | **2003–2024** | 256.0 KB | `77e7b178138477fca47d8ecbf02be622` | Factory Binary Firmware Dump |
| `38770-MJC-A01.bin` | **2003–2024** | 256.0 KB | `4a3c7f75593a162aaf1adce606590e63` | Factory Binary Firmware Dump |
| `38770-MJC-D01.bin` | **2003–2024** | 256.0 KB | `210ae00bd01f4dc1de3aa09264886d6e` | Factory Binary Firmware Dump |
| `38770-MKF-D43.bin` | **2003–2024** | 1.00 MB | `89535f291af29628a042399cf16fc71b` | Factory Binary Firmware Dump |
| `38770-MKF-D72.bin` | **2003–2024** | 1.00 MB | `536b4699bc61adc10a0210da4bf0b9c6` | Factory Binary Firmware Dump |
| `38770-MKF-L13.bin` | **2003–2024** | 1.00 MB | `7804b6309b93a05c294b8639a826f2d2` | Factory Binary Firmware Dump |
| `38770-MKF-TK2.bin` | **2003–2024** | 1.00 MB | `675d888b2463aac8d7b30ff045adab4f` | Factory Binary Firmware Dump |
| `38770-N1A-D11.bin` | **2003–2024** | 256.0 KB | `68f033b3e7f5f5aa05fce050446d095e` | Factory Binary Firmware Dump |
| `38770-NL3-750.bin` | **2003–2024** | 256.0 KB | `4480e3c59a2f0f692efaff227321cd79` | Factory Binary Firmware Dump |
| `CBR1000RR_2012_US.xdf` | **2012** | 62.1 KB | `fdd4c76d8680c68f5128286802c1b25d` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-MKR-D12_Honda_CBR1000RR_R_Fireblade_SP_SC82_2020_2026_217.5PS.xdf` | **2020–2026** | 1.8 KB | `2859e5eb41b0cce165f2ac32155e8657` | TunerPro Binary Definition Map |
| `HONDA_38770-MEE-612_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `9265cf5eae2930864a089dfc6e557f73` | TunerPro Binary Definition Map |
| `HONDA_38770-MEE-613_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `a4038a9ea09829761d88c627ce03bd75` | TunerPro Binary Definition Map |
| `HONDA_38770-MEE-622_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `c3ab6835fa8cd0b7bdcb6f32a28243b5` | TunerPro Binary Definition Map |
| `HONDA_38770-MEE-A02_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `102f59c46b983b316fa9292b6daff887` | TunerPro Binary Definition Map |
| `HONDA_38770-MEE-D01_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `7cf6ac781733931e7fd834e4478f8c5e` | TunerPro Binary Definition Map |
| `HONDA_38770-MEE-F02_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `de622769983bac580e9b632b16f64084` | TunerPro Binary Definition Map |
| `HONDA_38770-MFJ-D04_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `288a55d2842e78c85742b8de3389ec62` | TunerPro Binary Definition Map |
| `HONDA_38770-MFJ-D42_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `cb2e5e92f6e04555df638e9944339225` | TunerPro Binary Definition Map |
| `HONDA_38770-MFJ-F03_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `79dc415f1d20b2208286834501f28c6c` | TunerPro Binary Definition Map |
| `HONDA_38770-MGZ-A03_CBR500R___CB500F___CB500X_(2013-2015).xdf` | **2013–2015** | 16.3 KB | `797c7c26c709e2f6776ac0ccb4303c94` | TunerPro Binary Definition Map |
| `HONDA_38770-MGZ-C02_CBR500R___CB500F___CB500X_(2013-2015).xdf` | **2013–2015** | 16.3 KB | `fcf6ce8573be82c95cef6568ba66f972` | TunerPro Binary Definition Map |
| `HONDA_38770-MGZ-C03_CBR500R___CB500F___CB500X_(2013-2015).xdf` | **2013–2015** | 16.3 KB | `56bb7ebdb8bf68fc56bcb80811dcbfc9` | TunerPro Binary Definition Map |
| `HONDA_38770-MGZ-D02_CBR500R___CB500F___CB500X_(2013-2015).xdf` | **2013–2015** | 16.3 KB | `90e0e00935011373c82d33ee7db18730` | TunerPro Binary Definition Map |
| `HONDA_38770-MGZ-U02_CBR500R___CB500F___CB500X_(2013-2015).xdf` | **2013–2015** | 16.3 KB | `01c21cc835562dc8020817c032b53b89` | TunerPro Binary Definition Map |
| `HONDA_38770-MJC-A01_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `e69e3ff12ffff46c16a0f62a58b12e57` | TunerPro Binary Definition Map |
| `HONDA_38770-MJC-D01_Honda_Generic_ECM.xdf` | **2003–2024** | 16.3 KB | `d9c42a762ea5bc852fd011735eac876e` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-A02_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `e3703349d2c33145e6bdedde90301a16` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-BB1_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `a9f5a5fdab1ad51c212aa989f5809dbf` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-D41_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `4cf65f818d15d96ee68824ed291af46c` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-G12_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `5d906c6969e7b8d615af66bbf27630be` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-G52_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `1b0a90c91b9aabe4638052ea68bc52ab` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-HB3_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `a56188859ed34336dc8728f1d1ed565d` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-S11_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `31a30a9b64bf86975873d146ad558f92` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-T15_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `a3b216a9779a1b087e44452a0f3314d3` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-T52_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `08457a1469f26b7169dda1b39dc8bec7` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-TB1_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `3dd846c4bc9d65e3ff261edc70dd68fa` | TunerPro Binary Definition Map |
| `HONDA_38770-MJE-VB1_CBR650F___CB650F_(2014-2018).xdf` | **2014–2018** | 16.3 KB | `6f7f0436f09edfc23a761f0406180eb1` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-961_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `95aed9433e2fc5c5fb629c9ba1b3816a` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-AQ1_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `263ca76644eac03c23c3d605cddbbe16` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-B41_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `0c0f7961abd94904e8843abde92420de` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-D51_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `72e132c198d808b906a7c45da0fb21aa` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-D91_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `0a5ec1ca8df806fc3e7b08b2936495da` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-DR1_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `16f6696225773b5f77e81aef5bc030d6` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-N11_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `0c358284c7d89e2ec5895f11e7fdb4f4` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-N41_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `9b23f57ef9d7e9facaa61a91e7579070` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-NM1_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `738e8115b0790140c5b67edb2a4839fb` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-T11_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `085c074a18ff56a18dbc07e506a2d008` | TunerPro Binary Definition Map |
| `HONDA_38770-MJW-_CBR500R___CB500F___CB500X_(2016-2018).xdf` | **2016–2018** | 16.3 KB | `8fb9cf98ec6047d0055a10b30b71b82b` | TunerPro Binary Definition Map |
| `HONDA_38770-MKN-D11_CBR650R___CB650R_(2019-2024).xdf` | **2019–2024** | 16.3 KB | `3438c52e32e75dcebcd1562ce6ba273a` | TunerPro Binary Definition Map |
| `HONDA_38770-MKN-D51_CBR650R___CB650R_(2019-2024).xdf` | **2019–2024** | 16.3 KB | `6aa995e0b25878d98f5b6dd9afd54973` | TunerPro Binary Definition Map |
| `HONDA_38770-MKN-DB1_CBR650R___CB650R_(2019-2024).xdf` | **2019–2024** | 16.3 KB | `bc1e620d9281160c80c2db9da8b42544` | TunerPro Binary Definition Map |
| `HONDA_38770-MKN-HB2_CBR650R___CB650R_(2019-2024).xdf` | **2019–2024** | 16.3 KB | `fa4bab62d0a239f61006905df5b1ce4b` | TunerPro Binary Definition Map |
| `HONDA_38770-MKN-HF2_CBR650R___CB650R_(2019-2024).xdf` | **2019–2024** | 16.3 KB | `a2bcccffc82a92f6282cfaa0cb405cc6` | TunerPro Binary Definition Map |
| `HONDA_38770-MKN-L32_CBR650R___CB650R_(2019-2024).xdf` | **2019–2024** | 16.3 KB | `3f94afbc296f001cae620124c3896659` | TunerPro Binary Definition Map |
| `HONDA_38770-MKN-T11_CBR650R___CB650R_(2019-2024).xdf` | **2019–2024** | 16.3 KB | `b0311c6905308d3b8c8d21a80bddfda4` | TunerPro Binary Definition Map |
| `HONDA_38770-MKN-U11_CBR650R___CB650R_(2019-2024).xdf` | **2019–2024** | 16.3 KB | `24c4b314c1c6fb8275226f79ea05742f` | TunerPro Binary Definition Map |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro / RomRaider yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, Smoke Limiter, Torque-to-Fuel Limiter, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance, Low/High Octane Timing, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow & Boost Management**: Peta Target Boost Pressure, Wastegate Duty Cycle (WGDC / N75 Map), MAF/MAP Scaling, dan Throttle Response Curves (Driver Wish).
- **Safety Limits & Thresholds**: Rev Limiter (Hard/Soft Cut), Top Speed Limiter (Vmax), Overboost Fuel Cut, EGT (Exhaust Gas Temperature) Protection, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
