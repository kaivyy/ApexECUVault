# MATIC_VARIO_PCX_ADV - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/MATIC_VARIO_PCX_ADV`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `36 files` (3 binary dumps, 33 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MATIC_VARIO_PCX_ADV` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `GENERATIONAL_38770-K0W-NA1_Honda_All_New_ADV_160_eSP+_2022_2025.xdf` | **2022–2025** | 2.5 KB | `695e3df521cb59aa86f68a41dabaaeec` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K1ZG-N21_Honda_All_New_PCX_160_eSP+_Gen_4_2021_2025.xdf` | **2021–2025** | 2.5 KB | `235b96081bde106d33f43643b56674ab` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K2SA-N01_Honda_All_New_Vario_160___Click_160_2022_2025.xdf` | **2022–2025** | 2.5 KB | `b2f8b974c4a1792047aba9f2a2f5a9a0` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K59-A11_Honda_Vario_150_Gen_1_LED_eSP_(2015-2017).xdf` | **2015–2017** | 5.4 KB | `e46e4e4235bf5710fc4e0116facde4de` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K59-A71_Honda_All_New_Vario_150_Gen_2_Keyless_(2018-2022).xdf` | **2018–2022** | 5.4 KB | `fd4bf7fe772c09f77eeb736aeba7fa00` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K60-B01_Honda_Vario_125_Gen_2_LED_eSP_(2015-2017).xdf` | **2015–2017** | 5.4 KB | `3e72445aed5e1aac12163716c1727d79` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K60-B61_Honda_All_New_Vario_125_Gen_3_(2018-2022).xdf` | **2018–2022** | 5.4 KB | `a3061844078c7316dbf007a26a06ddc9` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-KZR-601_Honda_Vario_125_Gen_1_Bohlam___Helm-in_(2012-2014).xdf` | **2012–2014** | 5.4 KB | `1c7889cd0e7f6c414adda92e6118b0d6` | TunerPro Binary Definition Map |
| `HONDA_30400-K0WF-T01_ADV150_2017-2019_ADV_150___ADV_160_(2019-2024).xdf` | **2017–2019** | 9.9 KB | `9cc0d130868deffdd274a1911705205f` | TunerPro Binary Definition Map |
| `HONDA_30400-K0WF-T01_ADV150_ADV_150___ADV_160_(2019-2024).xdf` | **2019–2024** | 9.9 KB | `6a5d7db2eacb11464701d4da4d8fac95` | TunerPro Binary Definition Map |
| `HONDA_30400-K0WM-TA1_ADV160_ADV_150___ADV_160_(2019-2024).xdf` | **2019–2024** | 9.9 KB | `219a79144eed206fd5ff253e93530953` | TunerPro Binary Definition Map |
| `HONDA_30400-K1ZF-T01_PCX160_NOABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | **2021–2024** | 9.9 KB | `0d8ee34e83511933ba354ca14e51981c` | TunerPro Binary Definition Map |
| `HONDA_30400-K1ZF-T11_PCX160ABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | **2021–2024** | 9.9 KB | `8c81309b3be15d948cf63087c0cde9ef` | TunerPro Binary Definition Map |
| `HONDA_30400-K1ZP-T51_PCX160_NOABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | **2021–2024** | 9.9 KB | `ea45f74e337b506f9bc11285c8aac84a` | TunerPro Binary Definition Map |
| `HONDA_30400-K1ZP-T71_PCX160_ABS_PCX_160_e_HEV___ABS_(2021-2024).xdf` | **2021–2024** | 9.9 KB | `1557a118750f3bc05433070580dff26a` | TunerPro Binary Definition Map |
| `HONDA_30400-K2VH-T11_CLICK125_2023_Click_125i_(2023-2024).xdf` | **2023–2024** | 9.9 KB | `5723d145a146ec8b4f7da5a455cd7797` | TunerPro Binary Definition Map |
| `HONDA_30400-K36F-T01_PCX150_2014-2015_PCX_150_(2014-2017).xdf` | **2014–2015** | 9.9 KB | `414ace585b8bb862a2367bd3d8bbeb05` | TunerPro Binary Definition Map |
| `HONDA_30400-K36S-T31__PCX150_2016-2017_PCX_150_(2014-2017).xdf` | **2016–2017** | 9.9 KB | `d9bce3d6f2c1455379ed3b48f49c7379` | TunerPro Binary Definition Map |
| `HONDA_30400-K46-N21_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `63daa9ac031dd0f0f937cc81fdb9b9aa` | TunerPro Binary Definition Map |
| `HONDA_30400-K46-N31_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `4d53e68816e62c3ba11a176cf3079eb6` | TunerPro Binary Definition Map |
| `HONDA_30400-K46-NA1_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `e5d6e8c515e7e3cbcb40cce9a2fd1aea` | TunerPro Binary Definition Map |
| `HONDA_30400-K59K-T11_Click150_2018-2020_Click_150i_(2018-2022).xdf` | **2018–2020** | 9.9 KB | `5ec86ebb5a8d81cb07635cfb36b1ed46` | TunerPro Binary Definition Map |
| `HONDA_30400-K60F-T01_Click125_2014-2015_Click_125i_LED_(2018-2022).xdf` | **2014–2015** | 9.9 KB | `b7847bfdf39aa12267b2edb68736f2cb` | TunerPro Binary Definition Map |
| `HONDA_30400-K60S-T71_Click125_2016-2017_Click_125i_LED_(2018-2022).xdf` | **2016–2017** | 9.9 KB | `f5495f9b898683ee5004a0f5e0d3ae61` | TunerPro Binary Definition Map |
| `HONDA_30400-K97F-T_PCX150_2017-2019_PCX_150_Smart_Key_(2018-2020).xdf` | **2017–2019** | 9.9 KB | `c8386403d129a890b7b3f9562bed7083` | TunerPro Binary Definition Map |
| `HONDA_38770-K46-N01_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `ab7172e4cebbffaeaed8d54df89922c1` | TunerPro Binary Definition Map |
| `HONDA_38770-KVG-V42_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `bcd915ffd0739b9adefd7c5224e87ac9` | TunerPro Binary Definition Map |
| `HONDA_38770-MKH-C02_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | **2017–2024** | 16.3 KB | `77f00d644ae65eb99c5fbf65da3bd5b8` | TunerPro Binary Definition Map |
| `HONDA_38770-MKH-C03_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | **2017–2024** | 16.3 KB | `73fa4462836cf5c70300692e86f5d282` | TunerPro Binary Definition Map |
| `HONDA_38770-MKH-D01_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | **2017–2024** | 16.3 KB | `cba998f35bed9eb76a470fbd3297dff5` | TunerPro Binary Definition Map |
| `HONDA_38770-MKH-D22_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | **2017–2024** | 16.3 KB | `de601fc0d88d65276a41707b380799c2` | TunerPro Binary Definition Map |
| `HONDA_38770-MKH-D23_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | **2017–2024** | 16.3 KB | `a48bf22696ab71ff4fb65d1921b64244` | TunerPro Binary Definition Map |
| `HONDA_38770-MKH-D42_X-ADV_750___Forza_750___NC750X_(2017-2024).xdf` | **2017–2024** | 16.3 KB | `4f82f575b534ad930d52de37b9d2da43` | TunerPro Binary Definition Map |
| `HONDA_CLICK_VARIO_110_KVB_S53_48KB_ORI.bin` | **2000–2024** | 48.0 KB | `47995583b4f9ea7c6d5c8052a8839c9e` | Factory Binary Firmware Dump |
| `HONDA_XADV_750_38770_MKH_D22_512KB_ORI.bin` | **2000–2024** | 512.0 KB | `8601ef381db3cf63228c81556f68ee0b` | Factory Binary Firmware Dump |
| `HONDA_XADV_750_38770_MKH_D42_512KB_ORI.bin` | **2000–2024** | 512.0 KB | `8601ef381db3cf63228c81556f68ee0b` | Factory Binary Firmware Dump |

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
