# SUBARU_5EAT_TCU_DENSO_HITACHI - ECU Calibration Suite

**Repository Path**: `02_CARS/SUBARU/SUBARU_5EAT_TCU_DENSO_HITACHI`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `29 files` (26 binary dumps, 3 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SUBARU_5EAT_TCU_DENSO_HITACHI` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `5AT_3.272_LEGAS_EJDM2008.bin` | **2008** | 1.00 MB | `51e1b9ed0e72938573fe6c4c2fedb74e` | Factory Binary Firmware Dump |
| `5AT_3.583_LEGASE_JDM2008.bin` | **2008** | 1.00 MB | `05fe405c9fe39c7c1484adcd11155be6` | Factory Binary Firmware Dump |
| `5EAT_ADE0236000.bin` | **2000–2024** | 512.0 KB | `afdf6cbc3f44987a43f5a2dc6b5bc313` | Factory Binary Firmware Dump |
| `5eat_tcu_denso_romraider_defs.xml` | **2000–2024** | 2.24 MB | `113bebbd405e3c8f28ee18e609c44378` | ECU / XML Calibration Map Definition |
| `5eat_tcu_logger.xml` | **2000–2024** | 45.4 KB | `5037f152a7321fbbe8f81952d1cb6145` | ECU / XML Calibration Map Definition |
| `5eat_tcu_romraider_defs.xml` | **2000–2024** | 5.66 MB | `16ef133d34b9ed9642c2057a57da18c9` | ECU / XML Calibration Map Definition |
| `8AF0237300_MB500NJ0VF32C_2006_TRIBECA_USDM.bin` | **2006** | 512.0 KB | `825cc624a601a89d95e2d95c4e477e70` | Factory Binary Firmware Dump |
| `8EFB206000_08FB2WA0_14_tribeca_usdm.bin` | **2000–2024** | 1.00 MB | `f67520400d791d3dd91bfa79568f14f5` | Factory Binary Firmware Dump |
| `91A0217300_MB4365.bin` | **2000–2024** | 384.0 KB | `dfb7bcc281f984f06c24e280d5974c1b` | Factory Binary Firmware Dump |
| `91A0217400_MB4372_A61022.bin` | **2000–2024** | 512.0 KB | `2c5a2360d6474a3428d90cb8b5aa1751` | Factory Binary Firmware Dump |
| `91A1207300_MB4364.bin` | **2000–2024** | 384.0 KB | `7834b35a6c25ecf96cde7321f3b14df2` | Factory Binary Firmware Dump |
| `91D0207500_MB436T_AH572_5EAT_JDM.bin` | **2000–2024** | 384.0 KB | `0f3e2c9db853b656918440c425e8c80c` | Factory Binary Firmware Dump |
| `91D1206000_5EAT.bin` | **2000–2024** | 384.0 KB | `b0f1f9c7c65657570bc70bfdbb42cbd8` | Factory Binary Firmware Dump |
| `91F0217100_MB436P_AG810_OBK03USDM.bin` | **2000–2024** | 384.0 KB | `8bd88dfde570bb07032ed429ecacb475` | Factory Binary Firmware Dump |
| `91FE207100_MB436L_AG802_5EAT_LGT05USDM.bin` | **2000–2024** | 384.0 KB | `cf82058608e4718e175b416f68985f7d` | Factory Binary Firmware Dump |
| `91FE216300.bin` | **2000–2024** | 512.0 KB | `104888b35ae076e2ad215dad688fac8f` | Factory Binary Firmware Dump |
| `AAD1A06000.bin` | **2000–2024** | 512.0 KB | `49afb305231252504b713d3ed9aa344c` | Factory Binary Firmware Dump |
| `ABD1A03100_A61022_LGT_JDM_2005_5EAT.bin` | **2005** | 384.0 KB | `e4637da77d0e2fe1a434554866264696` | Factory Binary Firmware Dump |
| `ACD1207000_MB558D01_LGT06_JDM.bin` | **2000–2024** | 512.0 KB | `74fbae3aca373c955c7f6e348ec68904` | Factory Binary Firmware Dump |
| `ACD1A06000_JDM_5EAT_2007_M32176F4V.bin` | **2007** | 512.0 KB | `439c4c3d3e5e9a0dd0841ec7c6ed8dae` | Factory Binary Firmware Dump |
| `B1AE207100_EZAE2WB1_2010_LGT_EDM.bin` | **2010** | 1.00 MB | `52c1f1fd2fea4a230035e9ed4051f887` | Factory Binary Firmware Dump |
| `Forester_SH9_STI_3.283_JDM2010.bin` | **2010** | 1.00 MB | `453872ab890176fd6198bc1163620f20` | Factory Binary Firmware Dump |
| `Impreza_STI_3.583_JDM2011.bin` | **2011** | 1.00 MB | `c7eb900692734f0174e964d7eb305ca0` | Factory Binary Firmware Dump |
| `SH7058S-3171121010_STI.bin` | **2000–2024** | 1.00 MB | `fc492e13db2ee78b54f0a7601724167d` | Factory Binary Firmware Dump |
| `SH7058S_TG5_3.083.bin` | **2000–2024** | 1.00 MB | `9abc6f3a7c8a428e5a9ba79f3f7fafc2` | Factory Binary Firmware Dump |
| `Tribeca_3.583_EDM_2009.bin` | **2009** | 1.00 MB | `bc566b8311fb7cf26e40e28dec3e58f7` | Factory Binary Firmware Dump |
| `[91D1207900-A61022]_31711AG589.bin` | **2000–2024** | 384.0 KB | `09764d513b8e9d39c662ba586a137d71` | Factory Binary Firmware Dump |
| `[AAD1A07100-A61022]_31711AJ782.bin` | **2000–2024** | 384.0 KB | `72760d6006e21fb9b87e651b27168393` | Factory Binary Firmware Dump |
| `[ABD1207000-A61022].bin` | **2000–2024** | 384.0 KB | `1e37115dee4255c99b2b3918159f884a` | Factory Binary Firmware Dump |

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
