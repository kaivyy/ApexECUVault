# v7.3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.3`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `46 files` (0 binary dumps, 46 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.3` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `R4C9F493B_5d55-040_100_003_v7.3.xdf` | **2015–2026** | 2.73 MB | `30ed693fc2d28c699f9cdf9f6a61c2dd` | TunerPro Binary Definition Map |
| `R4C9F4E6B_5d55-040_150_006_v7.3.xdf` | **2015–2026** | 2.73 MB | `a46b6f66fb903f7dc74a04b1ea9181fd` | TunerPro Binary Definition Map |
| `R4C9F4K6B_5d55-040_170_006_v7.3.xdf` | **2015–2026** | 2.73 MB | `12daf2322150a283caf7a2f4e8d203d7` | TunerPro Binary Definition Map |
| `R4C9F4N5B_5d55-040_180_005_v7.3.xdf` | **2015–2026** | 2.73 MB | `21a9f8d47a54f4e81dfec408150ae4e6` | TunerPro Binary Definition Map |
| `R4C9F4P7B_5d55-040_190_007_v7.3.xdf` | **2015–2026** | 2.73 MB | `21a9f8d47a54f4e81dfec408150ae4e6` | TunerPro Binary Definition Map |
| `R4C9F4P9B_5d55-040_190_009_v7.3.xdf` | **2015–2026** | 2.73 MB | `21a9f8d47a54f4e81dfec408150ae4e6` | TunerPro Binary Definition Map |
| `R4C9H5C5B_5d55-050_140_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `069c3b6fef84b718a54ba6b8580992a0` | TunerPro Binary Definition Map |
| `R4C9H5I5B_5d55-050_160_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `7df8f1332ab862c2fe35d0f4af7cc9b3` | TunerPro Binary Definition Map |
| `R4C9H5K5B_5d55-050_170_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `5a9112c36ef7a498544ecab7ab183bbc` | TunerPro Binary Definition Map |
| `R4C9H5N6B_5d55-050_180_006_v7.3.xdf` | **2015–2026** | 2.75 MB | `254f3d3965d80521ded8481b800b073d` | TunerPro Binary Definition Map |
| `R4C9H5P7B_5d55-050_190_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `621351823f77d1ac33ee0d71cef53ab3` | TunerPro Binary Definition Map |
| `R4C9H5P9B_5d55-050_190_009_v7.3.xdf` | **2015–2026** | 2.75 MB | `621351823f77d1ac33ee0d71cef53ab3` | TunerPro Binary Definition Map |
| `R4C9H5S8B_5d55-050_200_008_v7.3.xdf` | **2015–2026** | 2.75 MB | `2c777a9466942072210d205985c4d73f` | TunerPro Binary Definition Map |
| `R4C9H5V5B_5d55-050_220_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `3528783d615339dc5b701009c2c451ba` | TunerPro Binary Definition Map |
| `R4C9H695B_5d55-060_100_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `9b60e3494a8effd7c0ee101c888b2913` | TunerPro Binary Definition Map |
| `R4C9H6B5B_5d55-060_110_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `e0c32d7abc9550d79f9017a9d916d5e4` | TunerPro Binary Definition Map |
| `R4C9H6D6B_5d55-060_120_006_v7.3.xdf` | **2015–2026** | 2.75 MB | `2644d1d45be66f06abf3929fc9249938` | TunerPro Binary Definition Map |
| `R4C9H6D7B_5d55-060_120_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `ef33330129971a02475de0334be7f7c6` | TunerPro Binary Definition Map |
| `R4C9H6H7B_5d55-060_130_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `f294f4e2537c61fd795901e5f81d6b11` | TunerPro Binary Definition Map |
| `R4C9H6K5B_5d55-060_140_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `a3968c1c08b936eed0384830b4ce4ffe` | TunerPro Binary Definition Map |
| `R4C9H6N7B_5d55-060_150_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `7e14af622324980e9bc1082accf34cf9` | TunerPro Binary Definition Map |
| `R4C9H6P7B_5d55-060_160_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `b5b042fe7a3ae947672714b834c8c6d2` | TunerPro Binary Definition Map |
| `R4C9H6P9B_5d55-060_160_009_v7.3.xdf` | **2015–2026** | 2.75 MB | `b5b042fe7a3ae947672714b834c8c6d2` | TunerPro Binary Definition Map |
| `R4C9H6S8B_5d55-060_170_008_v7.3.xdf` | **2015–2026** | 2.75 MB | `292c411c486af37b5a49d0197b83b69f` | TunerPro Binary Definition Map |
| `R4C9H6V5B_5d55-060_190_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `0ec901c95df19a7b107d1061249acb75` | TunerPro Binary Definition Map |
| `R4C9J718B_5d55-070_030_008_v7.3.xdf` | **2015–2026** | 2.76 MB | `6ddaae807302b50dd133fd0bedd559f3` | TunerPro Binary Definition Map |
| `R4C9J755B_5d55-070_040_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `fdb8ade083c959f290fe68065596b407` | TunerPro Binary Definition Map |
| `R4C9J756B_5d55-070_040_006_v7.3.xdf` | **2015–2026** | 2.76 MB | `3f24f40a4cd69ee304449b6e91324c8e` | TunerPro Binary Definition Map |
| `R4C9J758B_5d55-070_050_008_v7.3.xdf` | **2015–2026** | 2.76 MB | `d922171c6849b66e830447b649d7bad8` | TunerPro Binary Definition Map |
| `R4C9J797B_5d55-070_060_007_v7.3.xdf` | **2015–2026** | 2.76 MB | `7e6d86c42863bcdae899c7d80bbba3c8` | TunerPro Binary Definition Map |
| `R4C9J7A5B_5d55-070_070_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `7e6d86c42863bcdae899c7d80bbba3c8` | TunerPro Binary Definition Map |
| `R4C9J7N5B_5d55-070_080_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `368faf5b44adf85680306bb85bbb3f35` | TunerPro Binary Definition Map |
| `R4C9J7P7B_5d55-070_090_007_v7.3.xdf` | **2015–2026** | 2.76 MB | `a6be730a013139a2eb24829a4e208ecc` | TunerPro Binary Definition Map |
| `R4C9J7P9B_5d55-070_090_009_v7.3.xdf` | **2015–2026** | 2.76 MB | `a6be730a013139a2eb24829a4e208ecc` | TunerPro Binary Definition Map |
| `R4C9J7S8B_5d55-070_100_008_v7.3.xdf` | **2015–2026** | 2.76 MB | `8773c6a60a4c8615bcd932d99020d00b` | TunerPro Binary Definition Map |
| `R4C9J7V5B_5d55-070_120_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `3f8346157e512c77bbe3b92518db4021` | TunerPro Binary Definition Map |
| `R4C9J7W5B_5d55-070_130_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `3f8346157e512c77bbe3b92518db4021` | TunerPro Binary Definition Map |
| `R4C9L857B_5d55-080_040_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `c984171bc7c2fa09736c9343ee0256bf` | TunerPro Binary Definition Map |
| `R4C9L875B_5d55-080_055_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `0c2f813c1da671fbbb58ca100b8b3157` | TunerPro Binary Definition Map |
| `R4C9L8N5B_5d55-080_060_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `6cb9d84a74ada8a70ecc9ebde883fce3` | TunerPro Binary Definition Map |
| `R4C9L8P7B_5d55-080_072_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `7916ce9d67ac3dd6cbb4677c278b593e` | TunerPro Binary Definition Map |
| `R4C9L8P9B_5d55-080_072_009_v7.3.xdf` | **2015–2026** | 2.75 MB | `7916ce9d67ac3dd6cbb4677c278b593e` | TunerPro Binary Definition Map |
| `R4C9L8PCB_5d55-080_072_012_v7.3.xdf` | **2015–2026** | 2.75 MB | `6c6a34030f07b9a0e4b115925b1129ef` | TunerPro Binary Definition Map |
| `R4C9L8S8B_5d55-080_080_008_v7.3.xdf` | **2015–2026** | 2.75 MB | `51110599a05e1f72f5dc9cb2c80ab087` | TunerPro Binary Definition Map |
| `R4C9L8V6B_5d55-080_100_006_v7.3.xdf` | **2015–2026** | 2.75 MB | `c030c3c11adfa3eb7d2da186517bd735` | TunerPro Binary Definition Map |
| `R4C9L8W9B_5d55-080_140_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `d952c72a6bda18dd2a394b9398f6d229` | TunerPro Binary Definition Map |

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
