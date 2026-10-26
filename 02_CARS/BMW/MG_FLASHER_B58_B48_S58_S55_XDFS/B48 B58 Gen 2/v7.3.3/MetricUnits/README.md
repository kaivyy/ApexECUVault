# MetricUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/v7.3.3/MetricUnits`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `57 files` (0 binary dumps, 57 definition maps)  

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
| `R4C9F493B_5d55-040_100_003_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.86 MB | `2d1339b9b825864be2caeb8bebaef722` | TunerPro Binary Definition Map |
| `R4C9F4C6B_5d55-040_140_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.86 MB | `192f3ecfb19f89d5adc9389fd1ef5bd3` | TunerPro Binary Definition Map |
| `R4C9F4E6B_5d55-040_150_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.86 MB | `746dca49220e6f26eb999aa7d694a564` | TunerPro Binary Definition Map |
| `R4C9F4K6B_5d55-040_170_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.86 MB | `cbe7cccc915b06622950e7baba54d674` | TunerPro Binary Definition Map |
| `R4C9F4N5B_5d55-040_180_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.86 MB | `83b7a15ca93a7410af2ffdc2a6a509e9` | TunerPro Binary Definition Map |
| `R4C9F4P7B_5d55-040_190_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.86 MB | `83b7a15ca93a7410af2ffdc2a6a509e9` | TunerPro Binary Definition Map |
| `R4C9F4P9B_5d55-040_190_009_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.86 MB | `83b7a15ca93a7410af2ffdc2a6a509e9` | TunerPro Binary Definition Map |
| `R4C9H56AB_5d55-050_115_010_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `6d3e7fac43b3c9652682846dc4df5c58` | TunerPro Binary Definition Map |
| `R4C9H596B_5d55-050_120_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `537d37613f27bc2906b072ce8dd26943` | TunerPro Binary Definition Map |
| `R4C9H5C5B_5d55-050_140_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `ffcbb302d08404ca05a739458355e4f6` | TunerPro Binary Definition Map |
| `R4C9H5E5B_5d55-050_150_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `f2d8816f552704cb1c69aa14e71bfc0f` | TunerPro Binary Definition Map |
| `R4C9H5E6B_5d55-050_150_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `755f8238830aa7704fdb51725625ba2f` | TunerPro Binary Definition Map |
| `R4C9H5I5B_5d55-050_160_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `402d0581fc9fd587918754ead1971a2e` | TunerPro Binary Definition Map |
| `R4C9H5K5B_5d55-050_170_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `8c9fe64653e2593bf758488977d36fee` | TunerPro Binary Definition Map |
| `R4C9H5N6B_5d55-050_180_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `0c4f1e6962c7c0feccb4e56fa357f06b` | TunerPro Binary Definition Map |
| `R4C9H5P7B_5d55-050_190_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `57d56be5f504693de165e35a5df5be7e` | TunerPro Binary Definition Map |
| `R4C9H5P9B_5d55-050_190_009_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `57d56be5f504693de165e35a5df5be7e` | TunerPro Binary Definition Map |
| `R4C9H5S8B_5d55-050_200_008_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `5b3301703b76e58b47c2d716b2cbe9fe` | TunerPro Binary Definition Map |
| `R4C9H5V5B_5d55-050_220_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `ad7cce684f5d5b5105e9ebc512fdbe4b` | TunerPro Binary Definition Map |
| `R4C9H695B_5d55-060_100_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `f0f0a16f6c80ac80ac8f07154a311fbf` | TunerPro Binary Definition Map |
| `R4C9H6B5B_5d55-060_110_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `f72e1f29d36e168715e70e29847aae1d` | TunerPro Binary Definition Map |
| `R4C9H6D5B_5d55-060_120_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `101fcb5518de13045baf701e6674f115` | TunerPro Binary Definition Map |
| `R4C9H6D6B_5d55-060_120_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `e6e2ad21efcfae47d8c8c496d2026624` | TunerPro Binary Definition Map |
| `R4C9H6D7B_5d55-060_120_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `e099c848b18845cbef6f655ae15e67c9` | TunerPro Binary Definition Map |
| `R4C9H6H7B_5d55-060_130_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `af9aa1ea0a16705e55a6fd0ef7fdcd6c` | TunerPro Binary Definition Map |
| `R4C9H6K5B_5d55-060_140_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `0f6bce91d0ee461ad48a4e7f687fd3dd` | TunerPro Binary Definition Map |
| `R4C9H6N7B_5d55-060_150_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `2351e22a73ad1e1788d4125e4c8ce399` | TunerPro Binary Definition Map |
| `R4C9H6P7B_5d55-060_160_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `f228c04c4dbae55eb1d22af00bdc89ef` | TunerPro Binary Definition Map |
| `R4C9H6P9B_5d55-060_160_009_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `f228c04c4dbae55eb1d22af00bdc89ef` | TunerPro Binary Definition Map |
| `R4C9H6S8B_5d55-060_170_008_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `2d5e93651ee7177a22da0d6daea74178` | TunerPro Binary Definition Map |
| `R4C9H6V5B_5d55-060_190_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `f680dbfadbfda0845b5ab45758c209ce` | TunerPro Binary Definition Map |
| `R4C9H6W5B_5d55-060_200_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.90 MB | `f680dbfadbfda0845b5ab45758c209ce` | TunerPro Binary Definition Map |
| `R4C9J718B_5d55-070_030_008_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `3b8b901cad67c53c4c05c532fac0e1be` | TunerPro Binary Definition Map |
| `R4C9J755B_5d55-070_040_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `9b8f0f62b343594b555ed8f0da01f0a7` | TunerPro Binary Definition Map |
| `R4C9J756B_5d55-070_040_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `a76be94fbc8b4c998ae94a8a7aeff855` | TunerPro Binary Definition Map |
| `R4C9J757B_5d55-070_050_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `a76be94fbc8b4c998ae94a8a7aeff855` | TunerPro Binary Definition Map |
| `R4C9J758B_5d55-070_050_008_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `d834a35f3fb40e70e4fd6683157af0f2` | TunerPro Binary Definition Map |
| `R4C9J795B_5d55-070_060_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `d1a8a7484350813d59b5a56e08285238` | TunerPro Binary Definition Map |
| `R4C9J797B_5d55-070_060_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `128cd50455c3e236cf3850d617f80c6e` | TunerPro Binary Definition Map |
| `R4C9J7A5B_5d55-070_070_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `128cd50455c3e236cf3850d617f80c6e` | TunerPro Binary Definition Map |
| `R4C9J7N5B_5d55-070_080_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `3af9871bea9f50207fea024ff2e0a9e4` | TunerPro Binary Definition Map |
| `R4C9J7P7B_5d55-070_090_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `92b1041d01d66606fea9cf0b0b6e88e8` | TunerPro Binary Definition Map |
| `R4C9J7P9B_5d55-070_090_009_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `92b1041d01d66606fea9cf0b0b6e88e8` | TunerPro Binary Definition Map |
| `R4C9J7S8B_5d55-070_100_008_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `59d48b2041c06252011a8769c2a22e01` | TunerPro Binary Definition Map |
| `R4C9J7V5B_5d55-070_120_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `5f633ecf69d838ee4cfea95c2c0e079b` | TunerPro Binary Definition Map |
| `R4C9J7W5B_5d55-070_130_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.92 MB | `5f633ecf69d838ee4cfea95c2c0e079b` | TunerPro Binary Definition Map |
| `R4C9L818B_5d55-080_030_008_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `448d683eeef5d2cef7475783e58d1b91` | TunerPro Binary Definition Map |
| `R4C9L856B_5d55-080_040_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `dd131bd3d5a85519b8da9c4aed2ebedc` | TunerPro Binary Definition Map |
| `R4C9L857B_5d55-080_040_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `c57e7b17328ba469cbbef12561e49707` | TunerPro Binary Definition Map |
| `R4C9L875B_5d55-080_055_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `16880346bb2bbf92d5270c09535dd571` | TunerPro Binary Definition Map |
| `R4C9L8N5B_5d55-080_060_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `67fd678b6234a1435f034742f2b577f9` | TunerPro Binary Definition Map |
| `R4C9L8P7B_5d55-080_072_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `1a89ab9da854de33bdd4ed45a50cccd5` | TunerPro Binary Definition Map |
| `R4C9L8P9B_5d55-080_072_009_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `1a89ab9da854de33bdd4ed45a50cccd5` | TunerPro Binary Definition Map |
| `R4C9L8PCB_5d55-080_072_012_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `b3d737038879e655dfab883e9b7db61d` | TunerPro Binary Definition Map |
| `R4C9L8S8B_5d55-080_080_008_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `4f02e5a5bbfa222eb104cf4743011dae` | TunerPro Binary Definition Map |
| `R4C9L8V6B_5d55-080_100_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `94a5fdbf338f11c9346a906befdcdea0` | TunerPro Binary Definition Map |
| `R4C9L8W9B_5d55-080_140_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.91 MB | `d886c2f2a9da863d4c36ee3ff3b110a4` | TunerPro Binary Definition Map |

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
