# MetricUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Generic/MetricUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `86 files` (0 binary dumps, 86 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MetricUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `R2C9C277B_3e7d-020_090_007.MetricUnits.xdf` | **2015–2026** | 928.2 KB | `a5aabafc576d85e109e5f532f7e2cb88` | TunerPro Binary Definition Map |
| `R2C9D392B_3e7d-030_110_002.MetricUnits.xdf` | **2015–2026** | 951.6 KB | `fead5455ec968ee9b44806d5d35e08b2` | TunerPro Binary Definition Map |
| `R2C9D3D6B_3e7d-030_120_006.MetricUnits.xdf` | **2015–2026** | 951.6 KB | `0572c5511bb1ce451085fb4d79a9d741` | TunerPro Binary Definition Map |
| `R2C9D3N5B_3e7d-030_130_005.MetricUnits.xdf` | **2015–2026** | 951.6 KB | `cfef8273a952fe23134808178801cdc4` | TunerPro Binary Definition Map |
| `R2C9D3P7B_3e7d-030_140_007.MetricUnits.xdf` | **2015–2026** | 951.6 KB | `cfef8273a952fe23134808178801cdc4` | TunerPro Binary Definition Map |
| `R2C9F493B_3e7d-040_100_003.MetricUnits.xdf` | **2015–2026** | 981.2 KB | `2a30d75f87f4ebcbdd7da9d65efd73f2` | TunerPro Binary Definition Map |
| `R2C9F4K6B_3e7d-040_170_006.MetricUnits.xdf` | **2015–2026** | 981.2 KB | `882afa957842480156e871742f779170` | TunerPro Binary Definition Map |
| `R2C9F4P7B_3e7d-040_190_007.MetricUnits.xdf` | **2015–2026** | 981.2 KB | `26789fd31636a89709227f2a32d00cc0` | TunerPro Binary Definition Map |
| `R2C9H56AB_3e7d-050_115_010.MetricUnits.xdf` | **2015–2026** | 1002.8 KB | `36d7a15b19f53699c378e3c9989369f3` | TunerPro Binary Definition Map |
| `R2C9H5E6B_3e7d-050_150_006.MetricUnits.xdf` | **2015–2026** | 1002.8 KB | `aed8b78cfa354310d2bd942ddcb8db0a` | TunerPro Binary Definition Map |
| `R2C9H5I5B_3e7d-050_160_005.MetricUnits.xdf` | **2015–2026** | 1002.8 KB | `365e905e1cfee6ae62aff722c979b9b6` | TunerPro Binary Definition Map |
| `R2C9H5P7B_3e7d-050_190_007.MetricUnits.xdf` | **2015–2026** | 1002.8 KB | `823874d1aa08b0f7e7d34ba5d034faa4` | TunerPro Binary Definition Map |
| `R2C9H695B_3e7d-060_100_005.MetricUnits.xdf` | **2015–2026** | 1015.4 KB | `66415339f88166e35b4b1c1d4bd5cef9` | TunerPro Binary Definition Map |
| `R2C9H6D5B_3e7d-060_120_005.MetricUnits.xdf` | **2015–2026** | 1015.4 KB | `dc6fef353b89f0cae95ded3cd0178463` | TunerPro Binary Definition Map |
| `R2C9H6H5B_3e7d-060_130_005.MetricUnits.xdf` | **2015–2026** | 1015.4 KB | `8c446d4e88c545f357ea32804e030591` | TunerPro Binary Definition Map |
| `R2C9H6P7B_3e7d-060_160_007.MetricUnits.xdf` | **2015–2026** | 1015.4 KB | `f57969af358f21970738649b2f32afaf` | TunerPro Binary Definition Map |
| `R2C9J717B_3e7d-070_030_007.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `2d5b15ba36f6d102be013813a1f2a474` | TunerPro Binary Definition Map |
| `R2C9J756B_3e7d-070_040_006.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `d79a7fe6462404d79c7865fcc14c1b24` | TunerPro Binary Definition Map |
| `R2C9J757B_3e7d-070_040_007.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `a99dc81e6bba4a6aea019b87e627f927` | TunerPro Binary Definition Map |
| `R2C9J795B_3e7d-070_060_005.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `d703c33950c35fb7a80395b8af91251b` | TunerPro Binary Definition Map |
| `R2C9J7N5B_3e7d-070_080_005.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `445bd816e11b1585df1eebf8944251a1` | TunerPro Binary Definition Map |
| `R2C9J7P7B_3e7d-070_090_007.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `10c687651a46f14ac47221a34f4504cb` | TunerPro Binary Definition Map |
| `R2C9L856B_3e7d-080_040_006.MetricUnits.xdf` | **2015–2026** | 1012.1 KB | `b38bd11cfab80e9c9159b46700f5816d` | TunerPro Binary Definition Map |
| `R2C9L8N5B_3e7d-080_060_005.MetricUnits.xdf` | **2015–2026** | 1012.1 KB | `3ac2108f525765787d02d89d3f7188e0` | TunerPro Binary Definition Map |
| `R2C9L8P7B_3e7d-080_072_007.MetricUnits.xdf` | **2015–2026** | 1012.1 KB | `73c3e19acfc4d3c6c9c8b90002e248f7` | TunerPro Binary Definition Map |
| `R2C9L8PCB_3e7d-080_072_012.MetricUnits.xdf` | **2015–2026** | 1012.1 KB | `6ed55c8b6f749a744c99b49ae743392d` | TunerPro Binary Definition Map |
| `R4C9F493B_5d55-040_100_003.MetricUnits.xdf` | **2015–2026** | 981.8 KB | `3ee0dfb3a9ad2e181df69d4ce8e2d85a` | TunerPro Binary Definition Map |
| `R4C9F4C6B_5d55-040_140_006.MetricUnits.xdf` | **2015–2026** | 981.8 KB | `d31949d01078bb7c3e2e3e5f8610f99e` | TunerPro Binary Definition Map |
| `R4C9F4E6B_5d55-040_150_006.MetricUnits.xdf` | **2015–2026** | 981.8 KB | `797b1905303ed024ef06749ca0758092` | TunerPro Binary Definition Map |
| `R4C9F4G5B_5d55-040_160_005.MetricUnits.xdf` | **2015–2026** | 981.8 KB | `fe54228d95341d16fca8b992c365a039` | TunerPro Binary Definition Map |
| `R4C9F4K6B_5d55-040_170_006.MetricUnits.xdf` | **2015–2026** | 981.8 KB | `bca0c7afddcfffa7085537cc1b141b08` | TunerPro Binary Definition Map |
| `R4C9F4N5B_5d55-040_180_005.MetricUnits.xdf` | **2015–2026** | 981.8 KB | `e535bd03ed2163f0b79396c7fe6fbdcf` | TunerPro Binary Definition Map |
| `R4C9F4P7B_5d55-040_190_007.MetricUnits.xdf` | **2015–2026** | 981.8 KB | `e535bd03ed2163f0b79396c7fe6fbdcf` | TunerPro Binary Definition Map |
| `R4C9F4P9B_5d55-040_190_009.MetricUnits.xdf` | **2015–2026** | 981.8 KB | `e535bd03ed2163f0b79396c7fe6fbdcf` | TunerPro Binary Definition Map |
| `R4C9H56AB_5d55-050_115_010.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `23b61927ff0084162f6215d28604b238` | TunerPro Binary Definition Map |
| `R4C9H596B_5d55-050_120_006.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `3735e7c410ce36aed157706817c19a37` | TunerPro Binary Definition Map |
| `R4C9H5C5B_5d55-050_140_005.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `db57ca376a022e72f8b5620a846a61b6` | TunerPro Binary Definition Map |
| `R4C9H5E5B_5d55-050_150_005.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `00605261442ff48a14c502f5848a6418` | TunerPro Binary Definition Map |
| `R4C9H5E6B_5d55-050_150_006.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `6bd6438a05a80e2e6a919af7df4905e4` | TunerPro Binary Definition Map |
| `R4C9H5I5B_5d55-050_160_005.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `1decfcf2e91961b8ad0914d5842387bb` | TunerPro Binary Definition Map |
| `R4C9H5K5B_5d55-050_170_005.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `f71570dee1e7a90f0915472d068c90fe` | TunerPro Binary Definition Map |
| `R4C9H5N6B_5d55-050_180_006.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `c19150bc08c0714228259bee66e8fc35` | TunerPro Binary Definition Map |
| `R4C9H5P7B_5d55-050_190_007.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `e680dbb6c71af0acc3ce36e18ddf0a2c` | TunerPro Binary Definition Map |
| `R4C9H5P9B_5d55-050_190_009.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `e680dbb6c71af0acc3ce36e18ddf0a2c` | TunerPro Binary Definition Map |
| `R4C9H5S8B_5d55-050_200_008.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `b344727816ef27845f23a0e4b0e2c236` | TunerPro Binary Definition Map |
| `R4C9H5V5B_5d55-050_220_005.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `85a779232a35cf95583c4dc8a3ea4fe8` | TunerPro Binary Definition Map |
| `R4C9H5W5B_5d55-050_230_005.MetricUnits.xdf` | **2015–2026** | 1003.4 KB | `85a779232a35cf95583c4dc8a3ea4fe8` | TunerPro Binary Definition Map |
| `R4C9H695B_5d55-060_100_005.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `03a1d3f74e84a83ae3013897f7aec96f` | TunerPro Binary Definition Map |
| `R4C9H6B5B_5d55-060_110_005.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `597669bb7a1bdce50f6c60423698b861` | TunerPro Binary Definition Map |
| `R4C9H6D5B_5d55-060_120_005.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `57f2c845cb076abe19bba0dfc9bbc9dc` | TunerPro Binary Definition Map |
| `R4C9H6D6B_5d55-060_120_006.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `6cce226be3d95ce7cd31d77788ca1d0d` | TunerPro Binary Definition Map |
| `R4C9H6D7B_5d55-060_120_007.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `d31050e0176caea12e07cd63a04605ab` | TunerPro Binary Definition Map |
| `R4C9H6H7B_5d55-060_130_007.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `1dcb87e5048efd340da231173fa52f8c` | TunerPro Binary Definition Map |
| `R4C9H6K5B_5d55-060_140_005.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `90582d4cd08d73ad83d97cb965a0442e` | TunerPro Binary Definition Map |
| `R4C9H6N7B_5d55-060_150_007.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `22594a36ac4b8d16bfba5fefc54e193a` | TunerPro Binary Definition Map |
| `R4C9H6P7B_5d55-060_160_007.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `e5a11ec406c0096a22681c41f380dbcd` | TunerPro Binary Definition Map |
| `R4C9H6P9B_5d55-060_160_009.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `e5a11ec406c0096a22681c41f380dbcd` | TunerPro Binary Definition Map |
| `R4C9H6S8B_5d55-060_170_008.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `9d8a12c88aaf6163d55c18d16a0d932f` | TunerPro Binary Definition Map |
| `R4C9H6V5B_5d55-060_190_005.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `913aecb466b3add6efa8142f46af0dd1` | TunerPro Binary Definition Map |
| `R4C9H6W5B_5d55-060_200_005.MetricUnits.xdf` | **2015–2026** | 1015.9 KB | `913aecb466b3add6efa8142f46af0dd1` | TunerPro Binary Definition Map |
| `R4C9J718B_5d55-070_030_008.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `3d321f5c6f2c32a3ec8310b4a2e8e540` | TunerPro Binary Definition Map |
| `R4C9J755B_5d55-070_040_005.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `fab2cf9c364b884fae8c63b1cbba5389` | TunerPro Binary Definition Map |
| `R4C9J756B_5d55-070_040_006.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `145859aef766179b69b491eb4a8e22e4` | TunerPro Binary Definition Map |
| `R4C9J757B_5d55-070_050_007.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `145859aef766179b69b491eb4a8e22e4` | TunerPro Binary Definition Map |
| `R4C9J758B_5d55-070_050_008.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `a500711c3084c11c8f5605c4fa09b9a5` | TunerPro Binary Definition Map |
| `R4C9J795B_5d55-070_060_005.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `13d0c94da310803871abca98d273c4cb` | TunerPro Binary Definition Map |
| `R4C9J797B_5d55-070_060_007.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `9a8b96ccfebcbdb65e22018eefbfa1d8` | TunerPro Binary Definition Map |
| `R4C9J7A5B_5d55-070_070_005.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `9a8b96ccfebcbdb65e22018eefbfa1d8` | TunerPro Binary Definition Map |
| `R4C9J7N5B_5d55-070_080_005.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `58c0c27ce8f524a830d753f96ad1e322` | TunerPro Binary Definition Map |
| `R4C9J7P7B_5d55-070_090_007.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `182ae8b264ff2416b11f063d55d044a2` | TunerPro Binary Definition Map |
| `R4C9J7P9B_5d55-070_090_009.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `182ae8b264ff2416b11f063d55d044a2` | TunerPro Binary Definition Map |
| `R4C9J7S8B_5d55-070_100_008.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `5eca225e425c36e86ab1672a1c534961` | TunerPro Binary Definition Map |
| `R4C9J7V5B_5d55-070_120_005.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `f01e00d47a1b021cf55bc7f35b6a67e2` | TunerPro Binary Definition Map |
| `R4C9J7W5B_5d55-070_130_005.MetricUnits.xdf` | **2015–2026** | 1.00 MB | `f01e00d47a1b021cf55bc7f35b6a67e2` | TunerPro Binary Definition Map |
| `R4C9L818B_5d55-080_030_008.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `be3d7e9dc1ede0f256b747aa33210f88` | TunerPro Binary Definition Map |
| `R4C9L856B_5d55-080_040_006.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `5b048f0d23a9c5108b1ea0e606598e2f` | TunerPro Binary Definition Map |
| `R4C9L857B_5d55-080_040_007.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `0c29d04f6ff9e244262619cf0746c87d` | TunerPro Binary Definition Map |
| `R4C9L875B_5d55-080_055_005.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `ed0b3879038096b1778bcb03b25cbe93` | TunerPro Binary Definition Map |
| `R4C9L8N5B_5d55-080_060_005.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `508e9d3e4342d1394e94f150a41abeae` | TunerPro Binary Definition Map |
| `R4C9L8P7B_5d55-080_072_007.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `ef199c810a1aa0143e964836b422e66c` | TunerPro Binary Definition Map |
| `R4C9L8P9B_5d55-080_072_009.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `ef199c810a1aa0143e964836b422e66c` | TunerPro Binary Definition Map |
| `R4C9L8PCB_5d55-080_072_012.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `d126a426f90424391ff2e3de2b0052d0` | TunerPro Binary Definition Map |
| `R4C9L8S8B_5d55-080_080_008.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `caa957b1a99bbce33bc0f3c0b3761082` | TunerPro Binary Definition Map |
| `R4C9L8V5B_5d55-080_100_005.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `4566024fecc5de7a66de42c369289f5c` | TunerPro Binary Definition Map |
| `R4C9L8V6B_5d55-080_100_006.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `12f1da649574f906e88dccfcb84d9de2` | TunerPro Binary Definition Map |
| `R4C9L8W9B_5d55-080_140_005.MetricUnits.xdf` | **2015–2026** | 1012.7 KB | `4546eb2f34a4ea735136be631f63a019` | TunerPro Binary Definition Map |

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
