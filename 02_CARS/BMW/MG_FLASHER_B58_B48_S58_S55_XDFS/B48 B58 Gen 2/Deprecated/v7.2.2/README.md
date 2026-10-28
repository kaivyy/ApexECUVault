# v7.2.2 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.2.2`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `84 files` (0 binary dumps, 84 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.2.2` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2015–2026

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `R4C9F4E6B_5d55-040_150_006_v7.2.2.a2l` | **2015–2026** | 484.4 KB | `ea281ae4c1c6073578842db7ca6a8f43` | ASAM ASAP2 ECU Description File |
| `R4C9F4E6B_5d55-040_150_006_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `1ba5ceb069c9ca415b1078d661713ef5` | TunerPro Binary Definition Map |
| `R4C9F4K6B_5d55-040_170_006_v7.2.2.a2l` | **2015–2026** | 484.4 KB | `6bd73107b222fadaea1ecb7721deef61` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `e3007490fc28790b59e51c0802ad5d17` | TunerPro Binary Definition Map |
| `R4C9F4N5B_5d55-040_180_005_v7.2.2.a2l` | **2015–2026** | 484.4 KB | `1efe957e53dbc160ff6569df3ac9ce85` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `171cae551f8aa8607fb78e2ab30f901c` | TunerPro Binary Definition Map |
| `R4C9F4P7B_5d55-040_190_007_v7.2.2.a2l` | **2015–2026** | 484.4 KB | `deabddc5b83c94e18a5e67fe70c02b0d` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `171cae551f8aa8607fb78e2ab30f901c` | TunerPro Binary Definition Map |
| `R4C9F4P9B_5d55-040_190_009_v7.2.2.a2l` | **2015–2026** | 484.4 KB | `ff00757883a2f1936b73ae2ca5052226` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `171cae551f8aa8607fb78e2ab30f901c` | TunerPro Binary Definition Map |
| `R4C9H5C5B_5d55-050_140_005_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `31df7a3fb6b4f2887d5a76a5eed4c9c4` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `ed7e2c0fa644b1d086c0d32aa96534b0` | TunerPro Binary Definition Map |
| `R4C9H5I5B_5d55-050_160_005_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `f952eac16ad8b2df53c64e307953ab91` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `b0fa6e50bc13b4330bea199cbbc11f8f` | TunerPro Binary Definition Map |
| `R4C9H5K5B_5d55-050_170_005_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `c1f60accc24b156ba58c2efe1e5e7ad3` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `51a9fbebd2c4b12b202667e4a2572901` | TunerPro Binary Definition Map |
| `R4C9H5N6B_5d55-050_180_006_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `a602a36826dcaec3f5448c3254997e1a` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `84fd9f0f9ef3a8f5ff882cece977e808` | TunerPro Binary Definition Map |
| `R4C9H5P7B_5d55-050_190_007_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `8c847170a61a147fa894871db62051f4` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `6fc50b54c19ad6d728c313c1cacb20ba` | TunerPro Binary Definition Map |
| `R4C9H5P9B_5d55-050_190_009_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `e3c6c5fc4d712697e0bc77370fc594d8` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `6fc50b54c19ad6d728c313c1cacb20ba` | TunerPro Binary Definition Map |
| `R4C9H5S8B_5d55-050_200_008_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `bcb7776ab4c7710cca8bc7f851ccf4bd` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `d949ef291cd36d2baa4c1e6fbd1826b4` | TunerPro Binary Definition Map |
| `R4C9H5V5B_5d55-050_220_005_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `830dc98a92bddd5ab5d555a3783f2ff6` | ASAM ASAP2 ECU Description File |
| `R4C9H5V5B_5d55-050_220_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `febb80b9deb9029caa4985398f8c634f` | TunerPro Binary Definition Map |
| `R4C9H695B_5d55-060_100_005_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `7f784b95b4cb296568b41e694112ae89` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `5f0e33dc41cbc50a17b0df7ad817111e` | TunerPro Binary Definition Map |
| `R4C9H6B5B_5d55-060_110_005_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `5e2a6a1ab5233b517de1ab7018fbef51` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `014ba3747c4d7fdaf9240b60edac6000` | TunerPro Binary Definition Map |
| `R4C9H6D7B_5d55-060_120_007_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `1369d620f824ef5f259fc634bb571f48` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `28a195f787a62a4ce9a393696152cdce` | TunerPro Binary Definition Map |
| `R4C9H6H7B_5d55-060_130_007_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `d4a131df3a28a14381d25a08fa395467` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `b431b348b2c0bcef87a9ad6d522f865a` | TunerPro Binary Definition Map |
| `R4C9H6K5B_5d55-060_140_005_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `c3b3fc242a4b115adb5fd595ae06fc10` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `92ef0472d9b01d12440a3cf857fc85e4` | TunerPro Binary Definition Map |
| `R4C9H6N7B_5d55-060_150_007_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `ddc48f48d55cb2549a671edff2f2b054` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `d70536740f9cd2dbe01b5b8d9a28e402` | TunerPro Binary Definition Map |
| `R4C9H6P7B_5d55-060_160_007_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `7a9513ada64c86d434efa2e251af3fbf` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `981ee57abcb6089aa235a8483c32284e` | TunerPro Binary Definition Map |
| `R4C9H6P9B_5d55-060_160_009_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `eb2bd9017ca483c91b0ebe9df46cd245` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `981ee57abcb6089aa235a8483c32284e` | TunerPro Binary Definition Map |
| `R4C9H6S8B_5d55-060_170_008_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `9f7bb00fb1b92ff4d990d51a9b7688bd` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `5d0f6ca9e2cc43360743537e1ac817be` | TunerPro Binary Definition Map |
| `R4C9H6V5B_5d55-060_190_005_v7.2.2.a2l` | **2015–2026** | 487.0 KB | `950ec72a6289993f0224e4190a9b0368` | ASAM ASAP2 ECU Description File |
| `R4C9H6V5B_5d55-060_190_005_v7.2.2.xdf` | **2015–2026** | 1.32 MB | `2d93c39981fa62d5989a7f9f7d2d39c4` | TunerPro Binary Definition Map |
| `R4C9J718B_5d55-070_030_008_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `d96714e0b2e8580c4225d96a4ad269b4` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `871381e0ec2460cd83296ba2f68159e8` | TunerPro Binary Definition Map |
| `R4C9J755B_5d55-070_040_005_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `26f999e806573d2d263274f505aeb712` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `c5be19c6672c55cf0f635a6b4b23c1e0` | TunerPro Binary Definition Map |
| `R4C9J756B_5d55-070_040_006_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `0acefd22b3e45f67842da1b302db1625` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `7ca63c1b90c142e6734d79bc3c3b3018` | TunerPro Binary Definition Map |
| `R4C9J758B_5d55-070_050_008_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `f6474f98113fc3e63f600ec2ffbe37ef` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `a5a5f47b47c468d403a538ff3c6764f6` | TunerPro Binary Definition Map |
| `R4C9J797B_5d55-070_060_007_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `90bc9c35e0c705a92f0dece7001239fe` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `b140748db4055ffbd5132d67025a1525` | TunerPro Binary Definition Map |
| `R4C9J7A5B_5d55-070_070_005_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `a8f5db5b4c0ab46805fa7adbb37f8b4f` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `b140748db4055ffbd5132d67025a1525` | TunerPro Binary Definition Map |
| `R4C9J7N5B_5d55-070_080_005_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `0eee4a0f4f065ad72acb9746f32579a7` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `637d74eaadf5b37e298a3ad9650637e7` | TunerPro Binary Definition Map |
| `R4C9J7P7B_5d55-070_090_007_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `c0e8cfab54961638d1f5c2862c8c3e29` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `f55fcff93d03427f43c1d2da8170d357` | TunerPro Binary Definition Map |
| `R4C9J7P9B_5d55-070_090_009_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `af40981db0f0cbdd42c8e09959a82dce` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `f55fcff93d03427f43c1d2da8170d357` | TunerPro Binary Definition Map |
| `R4C9J7S8B_5d55-070_100_008_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `668edfd02ab94d3ec1152d93cb531c52` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `44efa7322f766d80a1345feed48c6ee6` | TunerPro Binary Definition Map |
| `R4C9J7V5B_5d55-070_120_005_v7.2.2.a2l` | **2015–2026** | 487.7 KB | `0443061cecb875e4958d5e6c88b44a63` | ASAM ASAP2 ECU Description File |
| `R4C9J7V5B_5d55-070_120_005_v7.2.2.xdf` | **2015–2026** | 1.33 MB | `6e0ec12a7134bcf9af4db953fc352b22` | TunerPro Binary Definition Map |
| `R4C9L857B_5d55-080_040_007_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `0b2fe1ea5035857ce1e1d1bd8cf7d345` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.2.2.xdf` | **2015–2026** | 1.31 MB | `366e2da5e10ee409efaab60ed954d602` | TunerPro Binary Definition Map |
| `R4C9L875B_5d55-080_055_005_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `50f352067981039b04472c11d4e0883e` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.2.2.xdf` | **2015–2026** | 1.31 MB | `c8cd33c95fa5cbd288b4890401e10592` | TunerPro Binary Definition Map |
| `R4C9L8N5B_5d55-080_060_005_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `87e116252bf6965c445612efdc8ea451` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.2.2.xdf` | **2015–2026** | 1.31 MB | `ed13bc1893dead6c78cdeac199b09d34` | TunerPro Binary Definition Map |
| `R4C9L8P7B_5d55-080_072_007_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `7b9f1819ad8fd1f70a0b1a6461fb0d3a` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.2.2.xdf` | **2015–2026** | 1.31 MB | `d279ffa50705b16aebcdd3cd0a2874af` | TunerPro Binary Definition Map |
| `R4C9L8P9B_5d55-080_072_009_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `80d422e53e9b134f11bc2f0675a93bdf` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.2.2.xdf` | **2015–2026** | 1.31 MB | `d279ffa50705b16aebcdd3cd0a2874af` | TunerPro Binary Definition Map |
| `R4C9L8PCB_5d55-080_072_012_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `14812cc3e08cb86a8b0fc4d06ac68e9b` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.2.2.xdf` | **2015–2026** | 1.31 MB | `e70740f558e2d3a7b6b22566700a8a5c` | TunerPro Binary Definition Map |
| `R4C9L8S8B_5d55-080_080_008_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `d2cfc7dd2082af5227c3081296405a28` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.2.2.xdf` | **2015–2026** | 1.31 MB | `d79d30ef2f1f18e9793f982a6eb059a7` | TunerPro Binary Definition Map |
| `R4C9L8V6B_5d55-080_100_006_v7.2.2.a2l` | **2015–2026** | 483.1 KB | `359c59ef307141ee45ac5d2646508043` | ASAM ASAP2 ECU Description File |
| `R4C9L8V6B_5d55-080_100_006_v7.2.2.xdf` | **2015–2026** | 1.31 MB | `cc53615a8790da7ce6a12f9ec03113ab` | TunerPro Binary Definition Map |

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
