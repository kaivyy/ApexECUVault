# MetricUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/Generic/MetricUnits`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `70 files` (0 binary dumps, 70 definition maps)  

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
| `R0C9J8B2B_3081-080_017_002.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `37e56aac98a3abd6d0aecdc1e1781820` | TunerPro Binary Definition Map |
| `R0C9J8B2B_3081-080_017_002.a2l` | **2015–2026** | 386.1 KB | `cb43b8aa50cdf25975f5820bf66393ac` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `835bf73c6983eba75e758f705df1b55e` | TunerPro Binary Definition Map |
| `R0C9J8D2B_3081-080_021_002.a2l` | **2015–2026** | 386.1 KB | `9d178c10946072783c664e90cff74d63` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `3619007869fe99bfdb8b9f4e46cdda05` | TunerPro Binary Definition Map |
| `R0C9J8I2B_3081-080_029_002.a2l` | **2015–2026** | 386.1 KB | `4fe2768a0520ccb5baccb9cf47db5fa8` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `3619007869fe99bfdb8b9f4e46cdda05` | TunerPro Binary Definition Map |
| `R0C9J8I3B_3081-080_029_003.a2l` | **2015–2026** | 386.1 KB | `1702c88c998fb647fe3388a101c0dc1e` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `3619007869fe99bfdb8b9f4e46cdda05` | TunerPro Binary Definition Map |
| `R0C9J8I4B_3081-080_029_004.a2l` | **2015–2026** | 386.1 KB | `6dfe004866ed11e3500d8290b95fc25d` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `308e11d1d6c6404de110ffc6dbb53d8e` | TunerPro Binary Definition Map |
| `R0C9J962B_3081-090_010_002.a2l` | **2015–2026** | 386.1 KB | `497f08e0487cccf4b5bdb0abd388864b` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `cbed67e127562be6ed2c6bc85e9c93a1` | TunerPro Binary Definition Map |
| `R0C9J9E3B_3081-090_020_003.a2l` | **2015–2026** | 386.1 KB | `3a84d98af2854b8df9270ccbbc58f21a` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `700a07a99bb957f36159df6ab41deb1a` | TunerPro Binary Definition Map |
| `R0C9J9E4B_3081-090_020_004.a2l` | **2015–2026** | 386.1 KB | `da592a6e9e9f50a54925075f6d34e3e9` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `da308a32b00e08dd36171f9d49a359b6` | TunerPro Binary Definition Map |
| `R0C9JA05B_3081-090_025_005.a2l` | **2015–2026** | 386.1 KB | `aae93b1347aaf3717036db72e318a1dd` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `675dede1ee6e0530f0702966d34482d0` | TunerPro Binary Definition Map |
| `R0C9JA15B_3081-090_030_005.a2l` | **2015–2026** | 386.1 KB | `eeb278610e27e647d7a40bd9c3a55c3b` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `a686b8f0f0b5c2ad581c469845484bf9` | TunerPro Binary Definition Map |
| `R0C9JC05B_3081-090_050_005.a2l` | **2015–2026** | 386.1 KB | `57b4a5d6ea066f9052de58b02e55afd3` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `f603443022b91c782646adb0c741c90b` | TunerPro Binary Definition Map |
| `R0C9JD06B_3081-090_060_006.a2l` | **2015–2026** | 386.1 KB | `9f48f188711b3d0ddc17a94bde0b2e7a` | ASAM ASAP2 ECU Description File |
| `R0C9JE15B_3081-090_080_005.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `cd64187267ac4ce2eab2f50ee3550903` | TunerPro Binary Definition Map |
| `R0C9JE15B_3081-090_080_005.a2l` | **2015–2026** | 386.1 KB | `19ad03eba45185a7b9868b8b2b1c495e` | ASAM ASAP2 ECU Description File |
| `R0R96015B_7706-000_007_005.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `3daa2ac971cbe810b176aecb70bb8851` | TunerPro Binary Definition Map |
| `R0R96015B_7706-000_007_005.a2l` | **2015–2026** | 386.4 KB | `5f9d06828919697156f028ab47e9c039` | ASAM ASAP2 ECU Description File |
| `R0R96025B_7706-000_008_005.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `3daa2ac971cbe810b176aecb70bb8851` | TunerPro Binary Definition Map |
| `R0R96025B_7706-000_008_005.a2l` | **2015–2026** | 386.4 KB | `0f54d1d667bfc6ccd68b8a9bc391a1a9` | ASAM ASAP2 ECU Description File |
| `R0R9A005B_7706-000_011_005.MetricUnits.xdf` | **2015–2026** | 972.2 KB | `04581a5100b1a876715dbecd2d7f0158` | TunerPro Binary Definition Map |
| `R0R9A005B_7706-000_011_005.a2l` | **2015–2026** | 386.4 KB | `fa61d3dca9f21df202d33ed4b02c3f12` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002.MetricUnits.xdf` | **2015–2026** | 903.6 KB | `89e7ce9a9cfc621386fc90c5716e4f4b` | TunerPro Binary Definition Map |
| `R1C9I562B_3076-050_006_002.a2l` | **2015–2026** | 358.4 KB | `0e7c61e00f5fa1d9114911fa3dcb8b14` | ASAM ASAP2 ECU Description File |
| `R1C9J772B_3076-070_009_002.MetricUnits.xdf` | **2015–2026** | 960.2 KB | `667b05f6d7016fcce1a29afa2c1bf792` | TunerPro Binary Definition Map |
| `R1C9J772B_3076-070_009_002.a2l` | **2015–2026** | 379.5 KB | `92264d4684d71ee891b80285c2803473` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `e7103b805aa3d6f05e86fbe509e485e4` | TunerPro Binary Definition Map |
| `R1C9J8B2B_3076-080_017_002.a2l` | **2015–2026** | 386.1 KB | `c11f935c694377679990faf7c43f4456` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `e7103b805aa3d6f05e86fbe509e485e4` | TunerPro Binary Definition Map |
| `R1C9J8B3B_3076-080_017_003.a2l` | **2015–2026** | 386.1 KB | `642a0f1e7d18a5b3a04574494660b3b7` | ASAM ASAP2 ECU Description File |
| `R1C9J8D3B_3076-080_018_003.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `e7103b805aa3d6f05e86fbe509e485e4` | TunerPro Binary Definition Map |
| `R1C9J8D3B_3076-080_018_003.a2l` | **2015–2026** | 386.1 KB | `8dfcb33efc62ba8ce4f4950eb1f563ec` | ASAM ASAP2 ECU Description File |
| `R1C9J8G3B_3428-000_001_001.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `9a765e997fa4c2a5ef829cc2f1382c36` | TunerPro Binary Definition Map |
| `R1C9J8G3B_3428-000_001_001.a2l` | **2015–2026** | 386.1 KB | `ccb14dba32247135cce45d1f92959081` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `e8dd6d50e852f99bb6b3659c4315b324` | TunerPro Binary Definition Map |
| `R1C9J8I2B_3076-080_029_002.a2l` | **2015–2026** | 386.1 KB | `b53583bd92116cdde3b5cf604562a6f0` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `e8dd6d50e852f99bb6b3659c4315b324` | TunerPro Binary Definition Map |
| `R1C9J8I7B_3076-080_029_007.a2l` | **2015–2026** | 386.1 KB | `b179e7c592c71791d91de5da5bae510a` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `b559e04a0882821d343725ed9e1f3896` | TunerPro Binary Definition Map |
| `R1C9J962B_3076-090_010_002.a2l` | **2015–2026** | 386.1 KB | `1be809321791f90cf3e1c729b016ed0f` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `3973205f6adb959aec5c4660d35cb83c` | TunerPro Binary Definition Map |
| `R1C9J9E3B_3076-090_020_003.a2l` | **2015–2026** | 386.1 KB | `c1f3d2bf5268abe391ffac0638f5a922` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `5057f02a277bc43e160d48aa53729db1` | TunerPro Binary Definition Map |
| `R1C9J9E5B_3076-090_020_005.a2l` | **2015–2026** | 386.1 KB | `41871db55d2ef80e473ed8c9d2a14488` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `3973205f6adb959aec5c4660d35cb83c` | TunerPro Binary Definition Map |
| `R1C9J9E7B_3076-090_020_007.a2l` | **2015–2026** | 386.1 KB | `c8da21332073d9bfcbeca83ca13a52e8` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `e39cdaa2ef7cfe86e5cfa51f5c1c224d` | TunerPro Binary Definition Map |
| `R1C9JA05B_3076-090_025_005.a2l` | **2015–2026** | 386.1 KB | `d8758065ba6d002ffb2887ec5c09acd9` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `22468a1e78992cc6128f5f8ddfd2c73e` | TunerPro Binary Definition Map |
| `R1C9JC05B_3076-090_050_005.a2l` | **2015–2026** | 386.1 KB | `ba0c6a822d7d6251966132140799d5e0` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `e66123db25edf025e1b89e6087d52e55` | TunerPro Binary Definition Map |
| `R1C9JD06B_3076-090_060_006.a2l` | **2015–2026** | 386.1 KB | `547dd8687323247792fc7640e19a1179` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `c4a7ce8eda5510e91faa487df5d51c95` | TunerPro Binary Definition Map |
| `R1C9JE15B_3076-090_080_005.a2l` | **2015–2026** | 386.1 KB | `35e191c5f5f850e8c80de63215831ba6` | ASAM ASAP2 ECU Description File |
| `R1R95005B_7972-000_005_005.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `23c4ed92d6d692ec8afc82d82a3138d3` | TunerPro Binary Definition Map |
| `R1R95005B_7972-000_005_005.a2l` | **2015–2026** | 386.3 KB | `4d5e94e4432b4110e5d0d5500fcebf42` | ASAM ASAP2 ECU Description File |
| `R1R96015B_7972-000_007_005.MetricUnits.xdf` | **2015–2026** | 971.7 KB | `88040bf691d1f09554efbca78459f15a` | TunerPro Binary Definition Map |
| `R1R96015B_7972-000_007_005.a2l` | **2015–2026** | 386.3 KB | `447c5d991d489ead0d1aa61eb1e89ee5` | ASAM ASAP2 ECU Description File |
| `V0C9J6J2B_3125-065_027_002.MetricUnits.xdf` | **2015–2026** | 823.6 KB | `05e570d704111c989637a13a72b43340` | TunerPro Binary Definition Map |
| `V0C9J6J2B_3125-065_027_002.a2l` | **2015–2026** | 348.3 KB | `bceec2dbec6912329e0600d747cc8742` | ASAM ASAP2 ECU Description File |

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
