# M_POWER_S58_G80_M3_M4 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_S58_G80_M3_M4`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `80 files` (20 binary dumps, 60 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `M_POWER_S58_G80_M3_M4` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2020–2026

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `00005C640A6405.xdf` | **2020–2026** | 1.69 MB | `f37f25825c1854a9c68b26dbb548b6ee` | TunerPro Binary Definition Map |
| `00005C640A6405_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `72fb6006adfc84bd0e6e5b9f5ce93531` | Factory Binary Firmware Dump |
| `00005C640A6405_original.bin` | **2020–2026** | 8.00 MB | `413ef2ea35bf2f8a9560be18c0b8a065` | Factory Binary Firmware Dump |
| `00005C640A8205.xdf` | **2020–2026** | 1.69 MB | `e237ffb7e6c289a103bc05da7fe6f62e` | TunerPro Binary Definition Map |
| `00005C640A8205_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `f94ff9727a90e2b113713db4c89310c3` | Factory Binary Firmware Dump |
| `00005C640A8205_original.bin` | **2020–2026** | 8.00 MB | `053c85be20c53a7d593652fb25ac1532` | Factory Binary Firmware Dump |
| `00005C640A8C05.xdf` | **2020–2026** | 1.69 MB | `a5465ab38095c5646f69a951e0001805` | TunerPro Binary Definition Map |
| `00005C640A8C05_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `435e360a3eb44ef3e74bf1832662b1f7` | Factory Binary Firmware Dump |
| `00005C640A8C05_original.bin` | **2020–2026** | 8.00 MB | `223accd1ce8a97dec730d9836e7474b3` | Factory Binary Firmware Dump |
| `00005C64143206.xdf` | **2020–2026** | 1.76 MB | `4bfd87533165d6ecc9cf8eb17f3a39b3` | TunerPro Binary Definition Map |
| `00005C64143206_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `51447faf15bf67eb45d8e5844886efc5` | Factory Binary Firmware Dump |
| `00005C64143206_original.bin` | **2020–2026** | 8.00 MB | `470f636a9a5288589b1f55b903032a60` | Factory Binary Firmware Dump |
| `00005C64143C05.xdf` | **2020–2026** | 1.76 MB | `5f799f68ce160b207cf749513c87e300` | TunerPro Binary Definition Map |
| `00005C64143C05_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `b05cc5d0afe6253bfbd455ca9fc605d8` | Factory Binary Firmware Dump |
| `00005C64143C05_original.bin` | **2020–2026** | 8.00 MB | `c7aa1bbea27d1fea729a48a1b435f3aa` | Factory Binary Firmware Dump |
| `00005C64144606.xdf` | **2020–2026** | 1.76 MB | `3f67811e99a11dc4d686e0306a68d5cf` | TunerPro Binary Definition Map |
| `00005C64144606_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `859217e5b3ba6f7b947aa45ecafdf1bf` | Factory Binary Firmware Dump |
| `00005C64144606_original.bin` | **2020–2026** | 8.00 MB | `e30e45f760c56ebcff7c294b849d1057` | Factory Binary Firmware Dump |
| `00005C64145007.xdf` | **2020–2026** | 1.76 MB | `176f147d12e9f78f92d676b2a6a88831` | TunerPro Binary Definition Map |
| `00005C64145007_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `6617de3edaed9738a5e1a4b47402352c` | Factory Binary Firmware Dump |
| `00005C64145007_original.bin` | **2020–2026** | 8.00 MB | `653aa4aa9180db06d4f67e6c264d0d42` | Factory Binary Firmware Dump |
| `00005C64145A05.xdf` | **2020–2026** | 1.76 MB | `7725c2f599c5e973654012b11ede36b8` | TunerPro Binary Definition Map |
| `00005C64145A05_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `54d192922938f0edb88df4e1a6111554` | Factory Binary Firmware Dump |
| `00005C64145A05_original.bin` | **2020–2026** | 8.00 MB | `9ddb66cac815e50a561c84787994b10b` | Factory Binary Firmware Dump |
| `00005C64146E06.xdf` | **2020–2026** | 1.76 MB | `02683e28672df56ae1883c222f217ebb` | TunerPro Binary Definition Map |
| `00005C64146E06_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `41987a16d4b1c0452700e117d79e69fe` | Factory Binary Firmware Dump |
| `00005C64146E06_original.bin` | **2020–2026** | 8.00 MB | `a99a70969cd9ca3bdeaaa7642d397ae2` | Factory Binary Firmware Dump |
| `00005C64148205.xdf` | **2020–2026** | 1.76 MB | `efa2ae816574669ef29bfbfc9b175e19` | TunerPro Binary Definition Map |
| `00005C64148205_MapSwitchBase.bin` | **2020–2026** | 8.00 MB | `62af65c2a9415559f1a38cc2c4594516` | Factory Binary Firmware Dump |
| `00005C64148205_original.bin` | **2020–2026** | 8.00 MB | `d171672a58de7d6609219f59c20c4d00` | Factory Binary Firmware Dump |
| `00005C64148706.xdf` | **2020–2026** | 1.76 MB | `efa2ae816574669ef29bfbfc9b175e19` | TunerPro Binary Definition Map |
| `00005C6414C808.xdf` | **2020–2026** | 1.76 MB | `06f9b298264de065581b707f7d0eb1cb` | TunerPro Binary Definition Map |
| `F4C9G577B_5c64-010_090_007.a2l` | **2020–2026** | 397.8 KB | `052f4bc11c818ea6bfa84e0b6894b75c` | ASAM ASAP2 ECU Description File |
| `F4C9G577B_5c64-010_090_007_v7.3.1.a2l` | **2020–2026** | 910.4 KB | `05a759e9dc2c7734c353c812cf75f360` | ASAM ASAP2 ECU Description File |
| `F4C9G577B_5c64-010_090_007_v7.3.3.a2l` | **2020–2026** | 910.1 KB | `f202cbd2df1fad6597c2787d1c60fc15` | ASAM ASAP2 ECU Description File |
| `F4C9G577B_5c64-010_090_007_v7.3.a2l` | **2020–2026** | 843.1 KB | `a46477b80683a237cdfb33776dfc1c33` | ASAM ASAP2 ECU Description File |
| `F4C9G595B_5c64-010_100_005.a2l` | **2020–2026** | 397.8 KB | `85c0bf9dbb96212af4413c1fc67808bf` | ASAM ASAP2 ECU Description File |
| `F4C9G595B_5c64-010_100_005_v7.3.1.a2l` | **2020–2026** | 910.4 KB | `7f4a50549f36ebdb003415a08a6819be` | ASAM ASAP2 ECU Description File |
| `F4C9G595B_5c64-010_100_005_v7.3.3.a2l` | **2020–2026** | 910.1 KB | `cedc22d21646be2df27e98cf88be9a19` | ASAM ASAP2 ECU Description File |
| `F4C9G595B_5c64-010_100_005_v7.3.a2l` | **2020–2026** | 843.1 KB | `47509a36fd4496cf5f91534a4e73f1dd` | ASAM ASAP2 ECU Description File |
| `F4C9G5F5B_5c64-010_130_005.a2l` | **2020–2026** | 397.8 KB | `1b3e49d222d19543b6cb5f410d12e6fb` | ASAM ASAP2 ECU Description File |
| `F4C9G5F5B_5c64-010_130_005_v7.3.1.a2l` | **2020–2026** | 910.4 KB | `dc31295616158c69d22c9e22dc08ca5a` | ASAM ASAP2 ECU Description File |
| `F4C9G5F5B_5c64-010_130_005_v7.3.3.a2l` | **2020–2026** | 910.1 KB | `4e001651e5eb263959b8b9f544419ef7` | ASAM ASAP2 ECU Description File |
| `F4C9G5F5B_5c64-010_130_005_v7.3.a2l` | **2020–2026** | 843.1 KB | `471998f3c9edc48e20fadfa882322dd4` | ASAM ASAP2 ECU Description File |
| `F4C9G5H5B_5c64-010_140_005.a2l` | **2020–2026** | 397.8 KB | `b1ed85b908c22aa5a0fe113e816aaceb` | ASAM ASAP2 ECU Description File |
| `F4C9G5H5B_5c64-010_140_005_v7.3.1.a2l` | **2020–2026** | 910.4 KB | `70c208e743ac7d77dcc97bf09e09213d` | ASAM ASAP2 ECU Description File |
| `F4C9G5H5B_5c64-010_140_005_v7.3.3.a2l` | **2020–2026** | 910.1 KB | `4964752704900510c86c15ec7dd977bf` | ASAM ASAP2 ECU Description File |
| `F4C9G5H5B_5c64-010_140_005_v7.3.a2l` | **2020–2026** | 843.1 KB | `cd7d2a32ce636f164a126d281802f3a4` | ASAM ASAP2 ECU Description File |
| `F4C9L8A6B_5c64-020_050_006.a2l` | **2020–2026** | 404.3 KB | `24481f8ee270d825db40b030fa1fe7b4` | ASAM ASAP2 ECU Description File |
| `F4C9L8A6B_5c64-020_050_006_v7.3.1.a2l` | **2020–2026** | 921.9 KB | `70076dcc9ca63d28a39e228279136d97` | ASAM ASAP2 ECU Description File |
| `F4C9L8A6B_5c64-020_050_006_v7.3.3.a2l` | **2020–2026** | 921.7 KB | `eaaad4492994853996349706ac3e2fda` | ASAM ASAP2 ECU Description File |
| `F4C9L8A6B_5c64-020_050_006_v7.3.a2l` | **2020–2026** | 845.6 KB | `6fd605074940c3134bd5ca8b872d5914` | ASAM ASAP2 ECU Description File |
| `F4C9L8C5B_5c64-020_060_005.a2l` | **2020–2026** | 404.3 KB | `f7f75a7600b6fad3f8b646330c893f95` | ASAM ASAP2 ECU Description File |
| `F4C9L8C5B_5c64-020_060_005_v7.3.1.a2l` | **2020–2026** | 921.9 KB | `e9479c4375867e5253fb57af6da2cc90` | ASAM ASAP2 ECU Description File |
| `F4C9L8C5B_5c64-020_060_005_v7.3.3.a2l` | **2020–2026** | 921.7 KB | `9594aa75ba803c8e4e66cde0db8a9c01` | ASAM ASAP2 ECU Description File |
| `F4C9L8C5B_5c64-020_060_005_v7.3.a2l` | **2020–2026** | 845.6 KB | `5c5b85118a8ed06247d68ca83d4c0bc7` | ASAM ASAP2 ECU Description File |
| `F4C9L8E6B_5c64-020_070_006.a2l` | **2020–2026** | 404.3 KB | `b85e36b7570620915892ba8f5d47b146` | ASAM ASAP2 ECU Description File |
| `F4C9L8E6B_5c64-020_070_006_v7.3.1.a2l` | **2020–2026** | 921.9 KB | `c562c8bcbfebe62cc488297df0655189` | ASAM ASAP2 ECU Description File |
| `F4C9L8E6B_5c64-020_070_006_v7.3.3.a2l` | **2020–2026** | 921.7 KB | `9059b892a4d02c2dd8c3d04d3fb46a3a` | ASAM ASAP2 ECU Description File |
| `F4C9L8E6B_5c64-020_070_006_v7.3.a2l` | **2020–2026** | 845.7 KB | `a1e9b9e23797156186fdf6df603f58cd` | ASAM ASAP2 ECU Description File |
| `F4C9L8G7B_5c64-020_080_007.a2l` | **2020–2026** | 404.3 KB | `7b43ed226f6b8151b762a367b32f1678` | ASAM ASAP2 ECU Description File |
| `F4C9L8G7B_5c64-020_080_007_v7.3.1.a2l` | **2020–2026** | 921.9 KB | `3e50d7c2213359be3933e23fb970c6d5` | ASAM ASAP2 ECU Description File |
| `F4C9L8G7B_5c64-020_080_007_v7.3.3.a2l` | **2020–2026** | 921.7 KB | `ae82a39a746ea1c3f10adef8a604c26c` | ASAM ASAP2 ECU Description File |
| `F4C9L8G7B_5c64-020_080_007_v7.3.a2l` | **2020–2026** | 845.6 KB | `db6e6bfca36a7b7aded93329a353a1ce` | ASAM ASAP2 ECU Description File |
| `F4C9L8J5B_5c64-020_090_005.a2l` | **2020–2026** | 404.3 KB | `f6c1ec5390689f3533e1d34ec362f3cd` | ASAM ASAP2 ECU Description File |
| `F4C9L8J5B_5c64-020_090_005_v7.3.1.a2l` | **2020–2026** | 921.9 KB | `99d16c59e660aebdeb98f3c9eb3820f9` | ASAM ASAP2 ECU Description File |
| `F4C9L8J5B_5c64-020_090_005_v7.3.3.a2l` | **2020–2026** | 921.7 KB | `a8c62b67a4b7374b2ea9f44836ce82fa` | ASAM ASAP2 ECU Description File |
| `F4C9L8J5B_5c64-020_090_005_v7.3.a2l` | **2020–2026** | 845.6 KB | `630d83290b201cf08ad1d5ebc583e4c2` | ASAM ASAP2 ECU Description File |
| `F4C9L8N6B_5c64-020_110_006.a2l` | **2020–2026** | 404.3 KB | `1f96bb1fe263067e033e1f99c051fb57` | ASAM ASAP2 ECU Description File |
| `F4C9L8N6B_5c64-020_110_006_v7.3.1.a2l` | **2020–2026** | 921.9 KB | `fa7dfa82d7faab2b0c98e523a8093cb5` | ASAM ASAP2 ECU Description File |
| `F4C9L8N6B_5c64-020_110_006_v7.3.3.a2l` | **2020–2026** | 921.7 KB | `13bcf99353705567b448c7943d68c873` | ASAM ASAP2 ECU Description File |
| `F4C9L8N6B_5c64-020_110_006_v7.3.a2l` | **2020–2026** | 845.6 KB | `ef67b07bbc990c0b3434cc6d8b659101` | ASAM ASAP2 ECU Description File |
| `F4C9L8R5B_5c64-020_130_005.a2l` | **2020–2026** | 404.3 KB | `f4ffee2f04ff1f6671f7285508d8d778` | ASAM ASAP2 ECU Description File |
| `F4C9L8R5B_5c64-020_130_005_v7.3.1.a2l` | **2020–2026** | 921.9 KB | `acc0cd26efb258e5ebf2a62a5ba1826a` | ASAM ASAP2 ECU Description File |
| `F4C9L8R5B_5c64-020_130_005_v7.3.3.a2l` | **2020–2026** | 921.7 KB | `f71eb4607c61e0fbced57aa86fc77115` | ASAM ASAP2 ECU Description File |
| `F4C9L8R5B_5c64-020_130_005_v7.3.a2l` | **2020–2026** | 845.6 KB | `4f19caee3863d58c260cfc7489ae6cc7` | ASAM ASAP2 ECU Description File |
| `F4C9L8R6B_5c64-020_135_006.a2l` | **2020–2026** | 404.3 KB | `63349f4c92564cd6faf6c0fd13f1f47f` | ASAM ASAP2 ECU Description File |
| `F4C9L8Y8B_5c64-020_200_008.a2l` | **2020–2026** | 401.9 KB | `5ff71e840cb407c88481feda8d8db9ec` | ASAM ASAP2 ECU Description File |
| `F4C9L8Y8B_5c64-020_200_008_v7.3.3.a2l` | **2020–2026** | 935.4 KB | `0b9b3702b0aa57a4d3082f2d50774559` | ASAM ASAP2 ECU Description File |
| `F4C9LU16B_aed2-020_060_006.a2l` | **2020–2026** | 404.3 KB | `aa7a29e3ae7567ab941d1d720914bea3` | ASAM ASAP2 ECU Description File |

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
