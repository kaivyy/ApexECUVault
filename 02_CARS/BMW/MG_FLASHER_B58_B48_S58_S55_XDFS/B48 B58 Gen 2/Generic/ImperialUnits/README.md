# ImperialUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Generic/ImperialUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `86 files` (0 binary dumps, 86 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ImperialUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `R2C9C277B_3e7d-020_090_007.ImperialUnits.xdf` | **2015–2026** | 929.1 KB | `c31707a290fc9bfce01541fbbd138215` | TunerPro Binary Definition Map |
| `R2C9D392B_3e7d-030_110_002.ImperialUnits.xdf` | **2015–2026** | 952.6 KB | `67eba66c83a67e1b686e94b7555fe0fe` | TunerPro Binary Definition Map |
| `R2C9D3D6B_3e7d-030_120_006.ImperialUnits.xdf` | **2015–2026** | 952.6 KB | `64a09f9c231e5a1553307e0b098f284c` | TunerPro Binary Definition Map |
| `R2C9D3N5B_3e7d-030_130_005.ImperialUnits.xdf` | **2015–2026** | 952.6 KB | `0d59156ed6dc7a5548dbf31885bb1119` | TunerPro Binary Definition Map |
| `R2C9D3P7B_3e7d-030_140_007.ImperialUnits.xdf` | **2015–2026** | 952.6 KB | `0d59156ed6dc7a5548dbf31885bb1119` | TunerPro Binary Definition Map |
| `R2C9F493B_3e7d-040_100_003.ImperialUnits.xdf` | **2015–2026** | 982.2 KB | `691fd1807683ab1474566f17852f5b80` | TunerPro Binary Definition Map |
| `R2C9F4K6B_3e7d-040_170_006.ImperialUnits.xdf` | **2015–2026** | 982.2 KB | `16fc4159108153ad4f0aecea4907ab59` | TunerPro Binary Definition Map |
| `R2C9F4P7B_3e7d-040_190_007.ImperialUnits.xdf` | **2015–2026** | 982.2 KB | `d4d65e2bda22a0d8ef1bb1c5e632afdd` | TunerPro Binary Definition Map |
| `R2C9H56AB_3e7d-050_115_010.ImperialUnits.xdf` | **2015–2026** | 1003.9 KB | `9fe4c391d38c7a0d599c3b521b42e430` | TunerPro Binary Definition Map |
| `R2C9H5E6B_3e7d-050_150_006.ImperialUnits.xdf` | **2015–2026** | 1003.9 KB | `67ee11c7da8b5b5f6ea2a301607f74a3` | TunerPro Binary Definition Map |
| `R2C9H5I5B_3e7d-050_160_005.ImperialUnits.xdf` | **2015–2026** | 1003.9 KB | `3a0eff2cb42efc6aa3ab8b8b34380afd` | TunerPro Binary Definition Map |
| `R2C9H5P7B_3e7d-050_190_007.ImperialUnits.xdf` | **2015–2026** | 1003.9 KB | `57b7333f8536256b016ed5021e480076` | TunerPro Binary Definition Map |
| `R2C9H695B_3e7d-060_100_005.ImperialUnits.xdf` | **2015–2026** | 1016.5 KB | `5413bb466033eb5b1e522bab4f24ec80` | TunerPro Binary Definition Map |
| `R2C9H6D5B_3e7d-060_120_005.ImperialUnits.xdf` | **2015–2026** | 1016.5 KB | `12c0b52b69a9326be72c1df4539c0863` | TunerPro Binary Definition Map |
| `R2C9H6H5B_3e7d-060_130_005.ImperialUnits.xdf` | **2015–2026** | 1016.5 KB | `4849eae7c0ac3abf9b3e41e0e2ff256d` | TunerPro Binary Definition Map |
| `R2C9H6P7B_3e7d-060_160_007.ImperialUnits.xdf` | **2015–2026** | 1016.5 KB | `8c422f4086c6ba2f58e01caa8e70aaf4` | TunerPro Binary Definition Map |
| `R2C9J717B_3e7d-070_030_007.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `afc0b343036cae5b82770df2db72a9f4` | TunerPro Binary Definition Map |
| `R2C9J756B_3e7d-070_040_006.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `0f07aea5b12ab6697f181ba27e4af726` | TunerPro Binary Definition Map |
| `R2C9J757B_3e7d-070_040_007.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `5406b89f4cbfb29932bf5ef313c8b8e0` | TunerPro Binary Definition Map |
| `R2C9J795B_3e7d-070_060_005.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `42ce0a3fd017a8529801a3e06a2c50d0` | TunerPro Binary Definition Map |
| `R2C9J7N5B_3e7d-070_080_005.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `9c3e4a2c244334bfd44a4445e05e6b7b` | TunerPro Binary Definition Map |
| `R2C9J7P7B_3e7d-070_090_007.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `9b3c2e54ab936ed8362954a7c55d04a1` | TunerPro Binary Definition Map |
| `R2C9L856B_3e7d-080_040_006.ImperialUnits.xdf` | **2015–2026** | 1013.2 KB | `0db098a4965d3d215999f4c0970c4bca` | TunerPro Binary Definition Map |
| `R2C9L8N5B_3e7d-080_060_005.ImperialUnits.xdf` | **2015–2026** | 1013.2 KB | `07ab5762de2449e998e09ac6b8509c8d` | TunerPro Binary Definition Map |
| `R2C9L8P7B_3e7d-080_072_007.ImperialUnits.xdf` | **2015–2026** | 1013.2 KB | `047031ac04522d4f1e1d766d85391f72` | TunerPro Binary Definition Map |
| `R2C9L8PCB_3e7d-080_072_012.ImperialUnits.xdf` | **2015–2026** | 1013.2 KB | `06e659c92c2dc0786a0169149e8c7645` | TunerPro Binary Definition Map |
| `R4C9F493B_5d55-040_100_003.ImperialUnits.xdf` | **2015–2026** | 982.8 KB | `22c2f3540ffb93ebc7d044031611fc18` | TunerPro Binary Definition Map |
| `R4C9F4C6B_5d55-040_140_006.ImperialUnits.xdf` | **2015–2026** | 982.8 KB | `6f151d33ad403426f5dc1cd44e867d88` | TunerPro Binary Definition Map |
| `R4C9F4E6B_5d55-040_150_006.ImperialUnits.xdf` | **2015–2026** | 982.8 KB | `9c503e4c4bb4f1be74e63054e3ae8cfa` | TunerPro Binary Definition Map |
| `R4C9F4G5B_5d55-040_160_005.ImperialUnits.xdf` | **2015–2026** | 982.8 KB | `c93e1936edb7fcf418db6f98c1c159a9` | TunerPro Binary Definition Map |
| `R4C9F4K6B_5d55-040_170_006.ImperialUnits.xdf` | **2015–2026** | 982.8 KB | `98850513ff16073d0b7eaa7f6a2f1da1` | TunerPro Binary Definition Map |
| `R4C9F4N5B_5d55-040_180_005.ImperialUnits.xdf` | **2015–2026** | 982.8 KB | `07f9d7b9b84b7b78e482a3b8ca442687` | TunerPro Binary Definition Map |
| `R4C9F4P7B_5d55-040_190_007.ImperialUnits.xdf` | **2015–2026** | 982.8 KB | `07f9d7b9b84b7b78e482a3b8ca442687` | TunerPro Binary Definition Map |
| `R4C9F4P9B_5d55-040_190_009.ImperialUnits.xdf` | **2015–2026** | 982.8 KB | `07f9d7b9b84b7b78e482a3b8ca442687` | TunerPro Binary Definition Map |
| `R4C9H56AB_5d55-050_115_010.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `2530b5038fdd26b9f9e0db41323101e1` | TunerPro Binary Definition Map |
| `R4C9H596B_5d55-050_120_006.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `dabf6b1fa48e0f83a2de517c62e0f20f` | TunerPro Binary Definition Map |
| `R4C9H5C5B_5d55-050_140_005.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `5580a588dc582463e4852c4d72c79a57` | TunerPro Binary Definition Map |
| `R4C9H5E5B_5d55-050_150_005.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `bdd903cc8085a0ec4867ef1d8ba6315c` | TunerPro Binary Definition Map |
| `R4C9H5E6B_5d55-050_150_006.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `7f5278120c1fc55ef4b3744c18ad32f0` | TunerPro Binary Definition Map |
| `R4C9H5I5B_5d55-050_160_005.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `66ea2627b495d0e11cb78df37d3ff087` | TunerPro Binary Definition Map |
| `R4C9H5K5B_5d55-050_170_005.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `9ce084fbc9efe371d3215670c0e75089` | TunerPro Binary Definition Map |
| `R4C9H5N6B_5d55-050_180_006.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `910ef046c130e35be6706676bac28b7d` | TunerPro Binary Definition Map |
| `R4C9H5P7B_5d55-050_190_007.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `21295749865262c665626bf85500f8c6` | TunerPro Binary Definition Map |
| `R4C9H5P9B_5d55-050_190_009.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `21295749865262c665626bf85500f8c6` | TunerPro Binary Definition Map |
| `R4C9H5S8B_5d55-050_200_008.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `f77281ffd01aa69c066df64c270c84e2` | TunerPro Binary Definition Map |
| `R4C9H5V5B_5d55-050_220_005.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `55953b2c7df944128ebe18e01f8c4072` | TunerPro Binary Definition Map |
| `R4C9H5W5B_5d55-050_230_005.ImperialUnits.xdf` | **2015–2026** | 1004.4 KB | `55953b2c7df944128ebe18e01f8c4072` | TunerPro Binary Definition Map |
| `R4C9H695B_5d55-060_100_005.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `224aa528981e20175f4e1d4fa83b56fc` | TunerPro Binary Definition Map |
| `R4C9H6B5B_5d55-060_110_005.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `e5f880ae70f4fb058abc236b41909969` | TunerPro Binary Definition Map |
| `R4C9H6D5B_5d55-060_120_005.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `c28cc8bc2508836b850472479d4b1a45` | TunerPro Binary Definition Map |
| `R4C9H6D6B_5d55-060_120_006.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `7127b2a95d5b1c9c735ef2618cb24c57` | TunerPro Binary Definition Map |
| `R4C9H6D7B_5d55-060_120_007.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `48f92426d2eb61341576218d423bb384` | TunerPro Binary Definition Map |
| `R4C9H6H7B_5d55-060_130_007.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `c17c3465bca97a775bd1d2d7603f5af3` | TunerPro Binary Definition Map |
| `R4C9H6K5B_5d55-060_140_005.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `5a9644d5eaca6d075782ccef4d204a74` | TunerPro Binary Definition Map |
| `R4C9H6N7B_5d55-060_150_007.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `3a65621ed027a26629b965fecdcb449d` | TunerPro Binary Definition Map |
| `R4C9H6P7B_5d55-060_160_007.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `24c9ede2a98b2756f745a53ffc509f45` | TunerPro Binary Definition Map |
| `R4C9H6P9B_5d55-060_160_009.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `24c9ede2a98b2756f745a53ffc509f45` | TunerPro Binary Definition Map |
| `R4C9H6S8B_5d55-060_170_008.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `892783ea09254031edf28e92ed78047b` | TunerPro Binary Definition Map |
| `R4C9H6V5B_5d55-060_190_005.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `ef997f0c5483219042315d78245ee317` | TunerPro Binary Definition Map |
| `R4C9H6W5B_5d55-060_200_005.ImperialUnits.xdf` | **2015–2026** | 1017.0 KB | `ef997f0c5483219042315d78245ee317` | TunerPro Binary Definition Map |
| `R4C9J718B_5d55-070_030_008.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `85342886cb3371ac065ed1ef879a1447` | TunerPro Binary Definition Map |
| `R4C9J755B_5d55-070_040_005.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `88886c21ef68cad9213d518840c9605c` | TunerPro Binary Definition Map |
| `R4C9J756B_5d55-070_040_006.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `c85639fe2260c7c61d2407f5aca3d36a` | TunerPro Binary Definition Map |
| `R4C9J757B_5d55-070_050_007.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `c85639fe2260c7c61d2407f5aca3d36a` | TunerPro Binary Definition Map |
| `R4C9J758B_5d55-070_050_008.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `046aa716d95c78626e4a8857928971d2` | TunerPro Binary Definition Map |
| `R4C9J795B_5d55-070_060_005.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `02e98f5b734b4ff715c2a57086f86556` | TunerPro Binary Definition Map |
| `R4C9J797B_5d55-070_060_007.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `87f34c2d06c331bed56724f1e07dc229` | TunerPro Binary Definition Map |
| `R4C9J7A5B_5d55-070_070_005.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `87f34c2d06c331bed56724f1e07dc229` | TunerPro Binary Definition Map |
| `R4C9J7N5B_5d55-070_080_005.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `290625e7c81eced12cc912bbc48eea7a` | TunerPro Binary Definition Map |
| `R4C9J7P7B_5d55-070_090_007.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `18772528364f0c23089366ac12aa5f19` | TunerPro Binary Definition Map |
| `R4C9J7P9B_5d55-070_090_009.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `18772528364f0c23089366ac12aa5f19` | TunerPro Binary Definition Map |
| `R4C9J7S8B_5d55-070_100_008.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `fa03b071f46546e167017a08b2f72deb` | TunerPro Binary Definition Map |
| `R4C9J7V5B_5d55-070_120_005.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `8a058ac1ed79d2e57b39b2a414d2b3aa` | TunerPro Binary Definition Map |
| `R4C9J7W5B_5d55-070_130_005.ImperialUnits.xdf` | **2015–2026** | 1.00 MB | `8a058ac1ed79d2e57b39b2a414d2b3aa` | TunerPro Binary Definition Map |
| `R4C9L818B_5d55-080_030_008.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `9e9626680c4ae5500a3e05a13e3f0b2d` | TunerPro Binary Definition Map |
| `R4C9L856B_5d55-080_040_006.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `454fd2a5bd8aa32277809a7e7b177adf` | TunerPro Binary Definition Map |
| `R4C9L857B_5d55-080_040_007.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `96211b39e0f5b4ab6477701e848d0b93` | TunerPro Binary Definition Map |
| `R4C9L875B_5d55-080_055_005.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `fac942b42e0bd7a9b49bf6063313d004` | TunerPro Binary Definition Map |
| `R4C9L8N5B_5d55-080_060_005.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `8fc1ee2ee7b0b5ccf6cacf9ba3b3b336` | TunerPro Binary Definition Map |
| `R4C9L8P7B_5d55-080_072_007.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `0da74874ac6153b50dbddf17250a99c2` | TunerPro Binary Definition Map |
| `R4C9L8P9B_5d55-080_072_009.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `0da74874ac6153b50dbddf17250a99c2` | TunerPro Binary Definition Map |
| `R4C9L8PCB_5d55-080_072_012.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `af909b7677f05f9fb1e25bffa255c540` | TunerPro Binary Definition Map |
| `R4C9L8S8B_5d55-080_080_008.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `719bc9f6fa9c1cc899d6540410233368` | TunerPro Binary Definition Map |
| `R4C9L8V5B_5d55-080_100_005.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `b79805f0a8fa5e1568f771894c46d197` | TunerPro Binary Definition Map |
| `R4C9L8V6B_5d55-080_100_006.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `dc5e89bbbb4de6034551fae572e58e86` | TunerPro Binary Definition Map |
| `R4C9L8W9B_5d55-080_140_005.ImperialUnits.xdf` | **2015–2026** | 1013.7 KB | `c287140a2c002dbee050d14fe0568b45` | TunerPro Binary Definition Map |

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
