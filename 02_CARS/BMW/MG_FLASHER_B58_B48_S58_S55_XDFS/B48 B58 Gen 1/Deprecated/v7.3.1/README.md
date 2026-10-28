# v7.3.1 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.3.1`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `27 files` (0 binary dumps, 27 definition maps)  

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
| `R0C9J8B2B_3081-080_017_002_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `2644caa747cc56d73c3efef8958bc6c8` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `cf456c1bd8a6a8672a51ff97918ffc79` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `482031dae4ed3cae284f4cf5ea2e8429` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `aec1634fece1a5a831e9def373fe56eb` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `e6daf2689385295f15c4c847b73afb3a` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `46fa7c1e317c81ee0d3e9e3756f3ecf9` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `516a0fa881000de2ef1ec8bca5f0bdbe` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `9911f5746e354185aa8e5276101e76ed` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `ee88e75a1ec22613424602eb2ce7a1a3` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `b11add0b43631045216e3cadbf368fb1` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `0e034ca74480a079d3252f9204d26bbd` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `783b7d9756fc9873085eb94fa071a858` | ASAM ASAP2 ECU Description File |
| `R0C9JE15B_3081-090_080_005_v7.3.1.a2l` | **2015–2026** | 894.3 KB | `412dcedd305e7824cb31682e01210346` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.3.1.a2l` | **2015–2026** | 859.4 KB | `0fc78eb97608719b61e6e2f413a2ee5f` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `a437966001dc94f702509e649754c570` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `9c93bd554266285ffac2b32c4e958741` | ASAM ASAP2 ECU Description File |
| `R1C9J8D3B_3076-080_018_003_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `472fc2fbe16567da29b99b816511f134` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `8414a59458aca01d17614576c8b37dac` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `2e7705df4470c483d97427bb517add1f` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `1bff9f031b11e787666e8529a1251df6` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `e20688bd8cf4f110e3ca3693d8e864b0` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `b4a4bca7ff1e44ece658d865c915d42b` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `6ecce163a8639bd790808df14db86d86` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `1cfa57df1600e94b9b10fcf8da5fda78` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `3da82a274901ce9967d6bbd271dc75c3` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `4f30b4ae77c9ce18c1ea3b5dfa06aa62` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.3.1.a2l` | **2015–2026** | 894.8 KB | `d7b405b426aa56a0350e08e97e231e76` | ASAM ASAP2 ECU Description File |

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
