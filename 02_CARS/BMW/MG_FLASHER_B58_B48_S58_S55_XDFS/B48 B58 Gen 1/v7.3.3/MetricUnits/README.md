# MetricUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/v7.3.3/MetricUnits`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `54 files` (0 binary dumps, 54 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MetricUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R0C9J8B2B_3081-080_017_002_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `4ac2216e0aa578aa2fd17f09f79cc0fe` | TunerPro Binary Definition Map |
| `R0C9J8B2B_3081-080_017_002_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `7f49b46f45ee23f5c62816e037a05f82` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `f656e22b0a33966d9c7384d9e1c487bd` | TunerPro Binary Definition Map |
| `R0C9J8D2B_3081-080_021_002_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `fd3592c4bae717cebd36c13ad8bd9613` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `d1fa375892d741f6e71559ebdf6a650f` | TunerPro Binary Definition Map |
| `R0C9J8I2B_3081-080_029_002_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `82dcbc174bc95291d684aa28b7aa1aa3` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `d1fa375892d741f6e71559ebdf6a650f` | TunerPro Binary Definition Map |
| `R0C9J8I3B_3081-080_029_003_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `e598acab19ed437468bb8a190672ba7d` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `d1fa375892d741f6e71559ebdf6a650f` | TunerPro Binary Definition Map |
| `R0C9J8I4B_3081-080_029_004_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `e8484d103902c6e0d2989c5abc9b56dd` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `b6761e3ba9243e1d8a1cc85eb9cf9099` | TunerPro Binary Definition Map |
| `R0C9J962B_3081-090_010_002_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `9f8b12fab0f3f2d32078fc88c52d75d0` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `ee291db344ffb07b02655292e0334c98` | TunerPro Binary Definition Map |
| `R0C9J9E3B_3081-090_020_003_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `3c05377c33fe7d0f216386428d2792ea` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `676c3d8abf21465416546a3fc0b95263` | TunerPro Binary Definition Map |
| `R0C9J9E4B_3081-090_020_004_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `47f927379495778ea9b1eea1446bef0e` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `ed90498c9efc6337011c3e7e5a341718` | TunerPro Binary Definition Map |
| `R0C9JA05B_3081-090_025_005_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `d2a1488c15499d9bba6b2c0a566e72df` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `45988f361b0f2d640de8c26d4301d7ba` | TunerPro Binary Definition Map |
| `R0C9JA15B_3081-090_030_005_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `c363e0f6a126971877f8aea05ef4d5dd` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `873db837b5bbcc3c7bb0118adb017f2e` | TunerPro Binary Definition Map |
| `R0C9JC05B_3081-090_050_005_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `d5d7f33413fba2c1d206b1b2e8b01976` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `648f820df55d8728f01fdf211d11f2af` | TunerPro Binary Definition Map |
| `R0C9JD06B_3081-090_060_006_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `06f1e3ec6755d8b341acabf8b839adc9` | ASAM ASAP2 ECU Description File |
| `R0C9JE15B_3081-090_080_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `fe028b9253f12430786ce7e81d0f80ea` | TunerPro Binary Definition Map |
| `R0C9JE15B_3081-090_080_005_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `2cb619abdd3ed9b9473aaf86807864ba` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.74 MB | `2e9f2aec87af503d058f6e6dab001d10` | TunerPro Binary Definition Map |
| `R1C9I562B_3076-050_006_002_v7.3.3.a2l` | **2015–2026** | 860.1 KB | `d2e0e4274ebc386f5742220676039c4a` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `8805fa0b86e001926c2ae407dafb6b23` | TunerPro Binary Definition Map |
| `R1C9J8B2B_3076-080_017_002_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `90d75e37bfabe3f41329446d57957f3e` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `8805fa0b86e001926c2ae407dafb6b23` | TunerPro Binary Definition Map |
| `R1C9J8B3B_3076-080_017_003_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `96e732ad786c4a8bd148e351b1421b1d` | ASAM ASAP2 ECU Description File |
| `R1C9J8D3B_3076-080_018_003_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `8805fa0b86e001926c2ae407dafb6b23` | TunerPro Binary Definition Map |
| `R1C9J8D3B_3076-080_018_003_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `0d151b52972aad59a89245db9378a5e1` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `c64293024f429d8a0663673867bc62d4` | TunerPro Binary Definition Map |
| `R1C9J8I2B_3076-080_029_002_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `f5b1048fb692f2cf87ecbc613ebd4ddb` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `c64293024f429d8a0663673867bc62d4` | TunerPro Binary Definition Map |
| `R1C9J8I7B_3076-080_029_007_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `63b0ae89d57923be0ded3fa91b456dc6` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `dbd91b3ade92f77fa391923d3ab1f25f` | TunerPro Binary Definition Map |
| `R1C9J962B_3076-090_010_002_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `63eddb93aa8d4b2b6e70e448d5b3058e` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `3677256f153da2a14dc829d9c92d1b8f` | TunerPro Binary Definition Map |
| `R1C9J9E3B_3076-090_020_003_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `5245fe362f86c466c9c1cefb65855bec` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `d8990d8a05953c12cd1edaa1bb070147` | TunerPro Binary Definition Map |
| `R1C9J9E5B_3076-090_020_005_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `4104fcc835d0322dc074e05f9232f707` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `3677256f153da2a14dc829d9c92d1b8f` | TunerPro Binary Definition Map |
| `R1C9J9E7B_3076-090_020_007_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `d2505fc7c054b9ac4ff2e012fbacd3c6` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `83e3613349675a105a0805e84a1a734c` | TunerPro Binary Definition Map |
| `R1C9JA05B_3076-090_025_005_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `14b4425047f41dcca341acbe6fed3a94` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `9f13a1bf5a76976c3d16f8d24fd8c81f` | TunerPro Binary Definition Map |
| `R1C9JC05B_3076-090_050_005_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `798f44adae732a63bac72df1a31b7bdb` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `25139845f06ba0913147cbbcedaac04f` | TunerPro Binary Definition Map |
| `R1C9JD06B_3076-090_060_006_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `5e1f81e061391dc6fc80ebec9f28c031` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.3.3.MetricUnits.xdf` | **2015–2026** | 2.83 MB | `7c78d3b2216e9052e480d68d52271dc5` | TunerPro Binary Definition Map |
| `R1C9JE15B_3076-090_080_005_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `0e8689342ce6148cd6c72c8529e91897` | ASAM ASAP2 ECU Description File |

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
