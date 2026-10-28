# v7.3.1 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.3.1`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `46 files` (0 binary dumps, 46 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.3.1` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R4C9F493B_5d55-040_100_003_v7.3.1.a2l` | **2015–2026** | 902.6 KB | `d239cdbdc2e60fd4a3f8cceb4c5b4919` | ASAM ASAP2 ECU Description File |
| `R4C9F4E6B_5d55-040_150_006_v7.3.1.a2l` | **2015–2026** | 902.6 KB | `9ac0fed1afa32ff192f6a4dfb27d1018` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.3.1.a2l` | **2015–2026** | 902.6 KB | `d52c4690cdff9e54bd7968b519313068` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.3.1.a2l` | **2015–2026** | 902.6 KB | `ecf0ce84105b0847b2d96023c893eaa7` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.3.1.a2l` | **2015–2026** | 902.6 KB | `b7e29fad2d65b80da711791986687cfd` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.3.1.a2l` | **2015–2026** | 902.6 KB | `5f630ee069e1dbb2e80980b3f6aae79b` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `14db27181eb1df2dfff6ede12fa92aa2` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `9eef7b99d5c2c7c3696f3e3b7fcf55fc` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `9569156d135fb35a4680ddaae1a260bb` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `accf61bc85f74d08c8e62c62ca009ba1` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `7403d0408dcfe1d07dfd107f1c9f4eb6` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `5e8fc2d258d960ded39704771012d32e` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `5dc60a3603a863dee089156c6149ac65` | ASAM ASAP2 ECU Description File |
| `R4C9H5V5B_5d55-050_220_005_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `9f7818ce71adf6a3fc20467da9665b5b` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `47427dc54ea85ff2d69ed03447e03f40` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `fa8dfffdd3e3ccedc6345bc8cc17af69` | ASAM ASAP2 ECU Description File |
| `R4C9H6D6B_5d55-060_120_006_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `a656246bcf5341b6344bf661cd7b6e7b` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `9980a08c2ab20b7bb1b9c565c38115ce` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `32176734ea21a1b1173fd9e67e127df0` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `24918aafe17661afaf8c98fb9ba8aaf6` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `dcc1ff928936939b92eaafdbc3f8fc61` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `48d07544a831c3febe4da0f4d1180983` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `cab4d66832449811c794ad413287198b` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `2ea90520b1af2b5c8e1c59aaa9db39c8` | ASAM ASAP2 ECU Description File |
| `R4C9H6V5B_5d55-060_190_005_v7.3.1.a2l` | **2015–2026** | 917.4 KB | `b63534a1a2f2d4ce3814d8a0ad905b75` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `4b57f906e77689b7f0274aefaefdb281` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `b00cf03aa01ff8249d1488fb511fc984` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `16242b66565f6b271fd0f09de4f09307` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `6521d5fd8b84ae2cefe5ac93e1c0ad34` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `5dd2d14889f6597b45b0a02b80729584` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `9e5789133ea7caa023cd08b1a78cb7fa` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `8b8e62f7eebfb6c6379b7374c25d0020` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `78277abaaf59dd8ddc61680e59bed7fa` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `7748a89890b760eca2b1d7be9814c4c4` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `409eb01fa5aeb6bc4d310eefc3e23052` | ASAM ASAP2 ECU Description File |
| `R4C9J7V5B_5d55-070_120_005_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `e9bd59e693d6b762442faa113f0942ae` | ASAM ASAP2 ECU Description File |
| `R4C9J7W5B_5d55-070_130_005_v7.3.1.a2l` | **2015–2026** | 925.3 KB | `444109ee4996bb4db9627bb9d5c9cf13` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `3bf945b7629c41585e0f85e81a95cf01` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `9c99e8fbea9dafe9d75f5384097a5e41` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `e154fdf9be5db8f616b3a5cfcd47ae2c` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `96e4f666498518205b0074871dd10541` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `e4c9a7cea115a925a743b353dc0c88c2` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `0778e511d3b1e976c5afa664eccdd4ef` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `29661552301dd9e7598a1ba13ae65368` | ASAM ASAP2 ECU Description File |
| `R4C9L8V6B_5d55-080_100_006_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `0a647125acec92561489418111b736ae` | ASAM ASAP2 ECU Description File |
| `R4C9L8W9B_5d55-080_140_005_v7.3.1.a2l` | **2015–2026** | 920.6 KB | `90017b35a5e811d1bcb1ef45a1fa83e3` | ASAM ASAP2 ECU Description File |

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
