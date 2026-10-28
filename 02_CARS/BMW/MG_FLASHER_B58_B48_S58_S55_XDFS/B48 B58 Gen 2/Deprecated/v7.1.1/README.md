# v7.1.1 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.1.1`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `38 files` (0 binary dumps, 38 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.1.1` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R4C9F4E6B_5d55-040_150_006_v7.1.1.a2l` | **2015–2026** | 179.5 KB | `db7c3d95c0d969a1c8d6aeb99dded5e5` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.1.1.a2l` | **2015–2026** | 179.5 KB | `66d6f9bdfca9aff6423a80a353c074bc` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.1.1.a2l` | **2015–2026** | 179.5 KB | `4010c76eec3d6c59fd0832332268e56b` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.1.1.a2l` | **2015–2026** | 179.5 KB | `ae9cdbe99b8d085b9549cb0d319d55bc` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.1.1.a2l` | **2015–2026** | 179.5 KB | `e85ec4e53d6dd464dded1d52e01bfd12` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `e7d66085621a9fe4cefa295d759ba632` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `8b70e92db971c8975e2964d87be0a460` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `4dc8ff87b03066e8717e9e5c7e2e018a` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `c2c6dd0b9ff1dd76689d089227ea0900` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `24c767450e6557b2dd343966c440c3e1` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `ddca4a8a2fba8370e1eae846366db14f` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `866dc2d89bf372861639bf5a0e3524b4` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `295ad13b60ef4c63937ed00710c5ca1e` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `0a1c39a0ec0af5f41fab80ed8606740e` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `bfba37326dea715ea5ec9044bceb171a` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `cc62cd1d7ca0081b80b3cbf8ea1f95eb` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `1f83ab60535c090b630d674e78d89576` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `4b12d4b48debf6712181b4790f9a1caa` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `c3c6dc4f65ef85459e9cdd2c577d2b08` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `b800aef7f07051ec5186ff00f19e8ea5` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `bfa1343dee56e358e3d989b3ae2025a0` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `d0df8552d667babba079ebac57f85c5b` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `a5bf96eea08e14d977e8a80cce290630` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `2629e5e96d1608fc7e5aef98bf8d8ce8` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `494b63eca208b2cc28bbd0a12dbed2e4` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `2cbc5e4ddffd891a755dfd82c89ea717` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `98ade953d07faebf18079e2dd37ff0c2` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `0a17e72810a716eb4604303a01a3875b` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `9c53c5ffee48ec8bc33194fe4dc37058` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `4af48d72e30aa236f89d514ccc002eb7` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `6e67fa41c7ce1d441478971539a7f1d2` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `631eac266abafe4067e311bad1f25181` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `5df2b82eebb0dc3b8fbea70de196a46c` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `3c0ef0dd0ee4f420090866e349ea25ec` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `b575f5dd5cc4d1d84b556be072dbcfbf` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `4a6549e7d3c36b5f9dee71de42575731` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `db09c773f9fad4b1d552a40636f4d095` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.1.1.a2l` | **2015–2026** | 181.3 KB | `5e128020a8069f3533bf6e135ebac168` | ASAM ASAP2 ECU Description File |

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
