# TRAIL_CRF150L_CRF250L - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/TRAIL_CRF150L_CRF250L`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `23 files` (6 binary dumps, 17 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `TRAIL_CRF150L_CRF250L` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `38770-EKCJ-J000.bin` | **2000–2024** | 256.0 KB | `90d0757c5dbbf71f18c332778f7435df` | Factory Binary Firmware Dump |
| `38770-KYK-D12.bin` | **2000–2024** | 64.0 KB | `f9e963fd1886a39d46f9a8a708b7d320` | Factory Binary Firmware Dump |
| `38770-KYK-D12.xdf` | **2000–2024** | 18.2 KB | `22f4b2a539194b14bc79c4376bf8482b` | TunerPro Binary Definition Map |
| `38770-MEN-E21.bin` | **2000–2024** | 256.0 KB | `796970fd1cdc559a93f9863b2d4e6a5e` | Factory Binary Firmware Dump |
| `38770-MKE-DataSettings.xdf` | **2000–2024** | 23.0 KB | `dc932d513d0e1b3e0bd4c7e5bf3d8ec3` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K84-901_Honda_CRF150L_Trail_Dual_Purpose_2017_2025.xdf` | **2017–2025** | 2.5 KB | `281906d4fe2145ce8d4bb1a8e98a99f7` | TunerPro Binary Definition Map |
| `HONDA_38770-K1T-A11_CRF300L___CRF300_Rally_(2021-2024).xdf` | **2021–2024** | 16.3 KB | `5555f7e3491381f5b2da174c0cc328fa` | TunerPro Binary Definition Map |
| `HONDA_38770-K1T-T01_CRF300L___CRF300_Rally_(2021-2024).xdf` | **2021–2024** | 16.3 KB | `1bf812d0211d69f5d7266acd5d5fa8af` | TunerPro Binary Definition Map |
| `HONDA_38770-K84-901_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `fafe71a3b36e3b40449ef7de30b5f4b3` | TunerPro Binary Definition Map |
| `HONDA_38770-KYK-D12_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `470af66dd467f5e9135c1d10b0081ab3` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-902_CRF250L___CRF250M___CRF250_Rally.xdf` | **2000–2024** | 16.3 KB | `7c0b752becaaea655c79c35ea353e6ca` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-914_CRF250L___CRF250M___CRF250_Rally.xdf` | **2000–2024** | 16.3 KB | `fd41ef963a87f312870849bd47ba0929` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-A22_CRF250L___CRF250M___CRF250_Rally.xdf` | **2000–2024** | 16.3 KB | `6bbd654e4f10bfa9ed7c178049fe1f20` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-J01_CRF250L___CRF250M___CRF250_Rally.xdf` | **2000–2024** | 16.3 KB | `29d5b844401cc8f7468f1fd0b7351ad0` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-J81_CRF250L___CRF250M___CRF250_Rally.xdf` | **2000–2024** | 16.3 KB | `039593a7dfddead0fc5b5e1d37ea5902` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-L41_CRF250L___CRF250M___CRF250_Rally.xdf` | **2000–2024** | 16.3 KB | `dc06414e9651aae93153fa7ca4eab159` | TunerPro Binary Definition Map |
| `HONDA_38770-MKE-A71_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `5f958feddae1be6e2e47b492de506851` | TunerPro Binary Definition Map |
| `HONDA_38770-MKE-A81_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `6479e76f00cea594902c916304c67a97` | TunerPro Binary Definition Map |
| `HONDA_38770-MKE-AF3_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `edfa56a9536ba1a751127bae40f861cb` | TunerPro Binary Definition Map |
| `HONDA_38770-MKK-D02_Africa_Twin_CRF1000L___CRF1100L.xdf` | **2000–2024** | 16.3 KB | `1648af151049c525c7824cd80cfc0a34` | TunerPro Binary Definition Map |
| `HONDA_CRF110F_38770_KYK_D12_64KB_ORI.bin` | **2000–2024** | 64.0 KB | `f9e963fd1886a39d46f9a8a708b7d320` | Factory Binary Firmware Dump |
| `HONDA_CRF450R_38770_MEN_E21_256KB_ORI.bin` | **2000–2024** | 256.0 KB | `796970fd1cdc559a93f9863b2d4e6a5e` | Factory Binary Firmware Dump |
| `HONDA_CRF450R_HRC_38770_EKCJ_J000_256KB_ORI.bin` | **2000–2024** | 256.0 KB | `90d0757c5dbbf71f18c332778f7435df` | Factory Binary Firmware Dump |

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
