# v7.1.3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Deprecated/v7.1.3`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `25 files` (0 binary dumps, 25 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.1.3` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R0C9J8B2B_3081-080_017_002_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `d611bdf50d24a562209e2726a6b1047f` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `4972fb77045c836c188a96ba9a7ff4bc` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `8220b637fca66db301a524dd12352147` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `3705805d6e4fc3c26a1112a71832bc6d` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `be1cde7b019ca74d55d4e66522c6526e` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `273ac180abd3dddd84d80f0f51af676e` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `ebfd56e3daaeb2929ab755336e27108c` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `774ebb08dda1dde884e0f17a9bc76ba0` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `2a529363ee4b03de8241e7052a33dcce` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `a92439b538f9f3310c0d8c9e406f2be1` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `4617fa579f11914f2710a919a799a219` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.1.3.a2l` | **2015–2026** | 177.1 KB | `612ddd328e0a002c5f84ebc5db64425d` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.1.3.a2l` | **2015–2026** | 176.3 KB | `9514a05d616a0095dfc7faaf3854c295` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `f648f3efb60c3d74de329b9e0083bdcd` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `1a795a0b960b92e54fa0207852c9dafc` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `830b055b70ff27e5a480e725368a481e` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `6392feb65e3d6522df7f1e1a5c9f85ab` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `fd47c07d0cf2de9ef94a60d5db83a3f6` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `e2e23745e1c688f4e4cf462b500f4f2a` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `6e7329ba45b66e52577d0214029073da` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `cbbff1f2660c332f338b2f5414f66888` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `59e561d3a27dd694b29628363fce80b1` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `1b25c78313416834737579a1d6a81462` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `046f18b1eb8031dab41415ad55e92075` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.1.3.a2l` | **2015–2026** | 177.3 KB | `91189e319da3155c7e9f020661f41f8f` | ASAM ASAP2 ECU Description File |

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
