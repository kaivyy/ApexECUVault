# M_POWER_S63_F10_F90_M5_M6 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_S63_F10_F90_M5_M6`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `55 files` (14 binary dumps, 41 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `M_POWER_S63_F10_F90_M5_M6` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2011–2023

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `000010CA3B8C01.xdf` | **2011–2023** | 637.8 KB | `861268aff0abe27b2e1e1c0a106039aa` | TunerPro Binary Definition Map |
| `000010CA3B8C01_original.bin` | **2011–2023** | 4.00 MB | `0dd83e918f3df32d04c462b535ea0d9e` | Factory Binary Firmware Dump |
| `000010CA598C01.xdf` | **2011–2023** | 630.3 KB | `40b2fb3ad1d325d622f69ae1027eaa8a` | TunerPro Binary Definition Map |
| `000010CA598C01_original.bin` | **2011–2023** | 4.00 MB | `9cfe95ad86ad74f8151117a24d8f3c7f` | Factory Binary Firmware Dump |
| `00004ACF0A3204.xdf` | **2011–2023** | 652.5 KB | `e45669d4d52dc60cb6bcc2d4276c0bd1` | TunerPro Binary Definition Map |
| `00004ACF0A3204_original.bin` | **2011–2023** | 8.00 MB | `1559258c9e0f7fd228e6efa5a999e9c7` | Factory Binary Firmware Dump |
| `00004ACF147803.xdf` | **2011–2023** | 658.1 KB | `597d4bfdc8ad2fb5efc492f2482aa481` | TunerPro Binary Definition Map |
| `00004ACF147803_original.bin` | **2011–2023** | 8.00 MB | `4503527b93e6ce592a9b8595622830ab` | Factory Binary Firmware Dump |
| `00004ACF1E6E05.xdf` | **2011–2023** | 652.7 KB | `2af11ea732261b5db6d559bf829bf15f` | TunerPro Binary Definition Map |
| `00004ACF1E6E05_original.bin` | **2011–2023** | 8.00 MB | `d0427f59c1135ea4ad7d48258455c94b` | Factory Binary Firmware Dump |
| `00004ACF1E7805.xdf` | **2011–2023** | 652.7 KB | `d6dc97ead974b74fd3ccac0d6d8a7934` | TunerPro Binary Definition Map |
| `00004ACF1E7805_original.bin` | **2011–2023** | 8.00 MB | `7f18fe0e6354407fbdf2b5a7133bd19f` | Factory Binary Firmware Dump |
| `00004ACF1E9605.xdf` | **2011–2023** | 652.7 KB | `8169ad83c416affb11fc9e7850783ad2` | TunerPro Binary Definition Map |
| `00004ACF1E9605_original.bin` | **2011–2023** | 8.00 MB | `d768576241ff96359ae416d0d9d181f5` | Factory Binary Firmware Dump |
| `00004ACF1EA006.xdf` | **2011–2023** | 652.7 KB | `81e91047b1b1716abec60567ff716733` | TunerPro Binary Definition Map |
| `00004ACF1EA006_original.bin` | **2011–2023** | 8.00 MB | `11c6ca46da75524b22523e50ab677bb4` | Factory Binary Firmware Dump |
| `00004ACF1EAA05.xdf` | **2011–2023** | 652.7 KB | `4df2808f53aa64558113ba51af40cc51` | TunerPro Binary Definition Map |
| `00004ACF1EAA05_original.bin` | **2011–2023** | 8.00 MB | `975835652e81499e12b19290df85279a` | Factory Binary Firmware Dump |
| `00004ACF1EB405.xdf` | **2011–2023** | 652.7 KB | `722a52dae76eede311b47d0656f023a1` | TunerPro Binary Definition Map |
| `00004ACF1EB405_original.bin` | **2011–2023** | 8.00 MB | `9aebadd1dc558eb08cfe0998d774af8e` | Factory Binary Firmware Dump |
| `00004ACF286E05.xdf` | **2011–2023** | 674.0 KB | `2609741adfc5c4b7d4d2312736597cfa` | TunerPro Binary Definition Map |
| `00004ACF286E05_original.bin` | **2011–2023** | 8.00 MB | `53973a1ccd7cc1f76a2a62f4ea60c224` | Factory Binary Firmware Dump |
| `00004ACF287806.xdf` | **2011–2023** | 674.0 KB | `5ef31f1d7441b1f631707ffee1a08f4e` | TunerPro Binary Definition Map |
| `00004ACF287806_original.bin` | **2011–2023** | 8.00 MB | `4ba04ce3d33efc8b5778600ead64a118` | Factory Binary Firmware Dump |
| `00004ACF288205.xdf` | **2011–2023** | 674.0 KB | `8009651bb5cd1a1471b66ee685baba4b` | TunerPro Binary Definition Map |
| `00004ACF288205_original.bin` | **2011–2023** | 8.00 MB | `cc01cfde49cb1b81baf5b87bdbafd43e` | Factory Binary Firmware Dump |
| `00004ACF289605.xdf` | **2011–2023** | 674.0 KB | `91f1f262280ee2dc0736a85c484b837c` | TunerPro Binary Definition Map |
| `00004ACF289605_original.bin` | **2011–2023** | 8.00 MB | `4d3d4d8ac5a72be4042a9648e209b05e` | Factory Binary Firmware Dump |
| `H4C99274B_4acf-010_050_004.a2l` | **2011–2023** | 335.0 KB | `480ca66ac3e9a44f5bdf8337301f85b5` | ASAM ASAP2 ECU Description File |
| `H4C993A3B_4acf-020_120_003.a2l` | **2011–2023** | 365.5 KB | `ff34481eceb245d2d973ecb918195951` | ASAM ASAP2 ECU Description File |
| `H4C99695B_4acf-030_110_005.a2l` | **2011–2023** | 373.8 KB | `78863e843feb732114e01309e6df5c8a` | ASAM ASAP2 ECU Description File |
| `H4C996B5B_4acf-030_120_005.a2l` | **2011–2023** | 373.8 KB | `098d5401a35c7e034b40cde0484a804d` | ASAM ASAP2 ECU Description File |
| `H4C996H5B_4acf-030_150_005.a2l` | **2011–2023** | 373.8 KB | `fbcffc64c1d0cf50923129e05fd5540f` | ASAM ASAP2 ECU Description File |
| `H4C996K5B_4acf-030_160_005.a2l` | **2011–2023** | 373.6 KB | `166af3308051cb066f76313e391639de` | ASAM ASAP2 ECU Description File |
| `H4C996K6B_4acf-030_160_006.a2l` | **2011–2023** | 373.8 KB | `0993b0a9374ceeece8575bec85e3f74c` | ASAM ASAP2 ECU Description File |
| `H4C996P5B_4acf-030_170_005.a2l` | **2011–2023** | 373.8 KB | `093f24031c1f8a52fce3436e0a8288aa` | ASAM ASAP2 ECU Description File |
| `H4C996R5B_4acf-030_180_073.a2l` | **2011–2023** | 373.8 KB | `41b9d9598f1b38c42cfeb85c82e06a76` | ASAM ASAP2 ECU Description File |
| `H4C9L8A5B_4acf-040_110_005.a2l` | **2011–2023** | 380.3 KB | `b9830b683ec998e3506b03db0fae38b3` | ASAM ASAP2 ECU Description File |
| `H4C9L8E6B_4acf-040_120_006.a2l` | **2011–2023** | 380.3 KB | `50259f36bd38e7dcd5a993f2429ad56b` | ASAM ASAP2 ECU Description File |
| `H4C9L8J5B_4acf-040_130_005.a2l` | **2011–2023** | 380.1 KB | `b00da35cf45a72a40d9f22d55f89355f` | ASAM ASAP2 ECU Description File |
| `H4C9L8N5B_4acf-040_150_005.a2l` | **2011–2023** | 380.1 KB | `06bf8ceae90a6b2206f96c00113108e6` | ASAM ASAP2 ECU Description File |
| `V4C9F4K6B_4963-040_170_006.a2l` | **2011–2023** | 371.9 KB | `cdbd540d475da88597e20b833b2b938a` | ASAM ASAP2 ECU Description File |
| `V4C9F4N6B_4963-040_180_006.a2l` | **2011–2023** | 371.9 KB | `33c0130d3fb8a509119224e7bc504955` | ASAM ASAP2 ECU Description File |
| `V4C9H6H6B_4963-060_130_006.a2l` | **2011–2023** | 383.8 KB | `fa782c98a60259491959470908cf1f3b` | ASAM ASAP2 ECU Description File |
| `V4C9H6N7B_4963-060_150_007.a2l` | **2011–2023** | 383.8 KB | `08c3ea3d55dfeee97d45a8ba2108b2d7` | ASAM ASAP2 ECU Description File |
| `V4C9H6S8B_4963-060_170_008.a2l` | **2011–2023** | 383.8 KB | `b163ab9187ab7b5157e5164f8c976682` | ASAM ASAP2 ECU Description File |
| `V4C9J717B_4963-070_030_007.a2l` | **2011–2023** | 387.7 KB | `079285a21be10a88efa0b54dae3f4bca` | ASAM ASAP2 ECU Description File |
| `V4C9J796B_4963-070_060_006.a2l` | **2011–2023** | 387.4 KB | `9239c126b0890a83150cacac20addfd4` | ASAM ASAP2 ECU Description File |
| `V4C9J7A5B_4963-070_070_005.a2l` | **2011–2023** | 387.4 KB | `79157031f10f52a5a6634b360c226a90` | ASAM ASAP2 ECU Description File |
| `V4C9J7N6B_4963-070_080_006.a2l` | **2011–2023** | 387.5 KB | `7ad74945565e6766bae4484dcc78520e` | ASAM ASAP2 ECU Description File |
| `V4C9J7S8B_4963-070_100_008.a2l` | **2011–2023** | 387.5 KB | `2b03039841b60b6f15074545eaad433d` | ASAM ASAP2 ECU Description File |
| `V4C9J7V5B_4963-070_120_005.a2l` | **2011–2023** | 387.5 KB | `18581cfbe8cb7942e80ceef4a606705d` | ASAM ASAP2 ECU Description File |
| `V4C9J7W5B_4963-070_130_005.a2l` | **2011–2023** | 387.5 KB | `5e3d031fc447a45064429271005aaa68` | ASAM ASAP2 ECU Description File |
| `V4C9L8N6B_4963-080_060_006.a2l` | **2011–2023** | 382.5 KB | `ce7975ebdccd22daad5440616ca3b52a` | ASAM ASAP2 ECU Description File |
| `V4C9L8S9B_4963-080_080_009.a2l` | **2011–2023** | 382.5 KB | `151db47bf627c2d70d94e98b3efbc257` | ASAM ASAP2 ECU Description File |

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
