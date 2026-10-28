# RAV4_1AZ_2AZ_2AR_2GR - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/RAV4_1AZ_2AZ_2AR_2GR`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `38 files` (38 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `RAV4_1AZ_2AZ_2AR_2GR` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2001–2018

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `89663-04252.bin` | **2001–2018** | 736.0 KB | `b667f7a22ff45b154ac99f23ed2af9b1` | Factory Binary Firmware Dump |
| `89663-04262.bin` | **2001–2018** | 736.0 KB | `9d2bb19e249a210754b44dd1a93ddebb` | Factory Binary Firmware Dump |
| `89663-42053.bin` | **2001–2018** | 320.0 KB | `4afb04f3561c91c450effd764dc30684` | Factory Binary Firmware Dump |
| `89663-42054.bin` | **2001–2018** | 320.0 KB | `5a40f1e52773a484e9383f97a7aa9ca7` | Factory Binary Firmware Dump |
| `89663-42063.bin` | **2001–2018** | 320.0 KB | `69d0122990a5aabaef71dec391ac2426` | Factory Binary Firmware Dump |
| `89663-42064.bin` | **2001–2018** | 320.0 KB | `e8f5bd35fd8d2eca6db869d6cd2f666c` | Factory Binary Firmware Dump |
| `89663-42073.bin` | **2001–2018** | 320.0 KB | `9268e6a6e780d6d298bbecfaf4f7def1` | Factory Binary Firmware Dump |
| `89663-42074.bin` | **2001–2018** | 320.0 KB | `dd43f512d10129b0413ab33d64751a04` | Factory Binary Firmware Dump |
| `89663-42083.bin` | **2001–2018** | 320.0 KB | `451205df7d80b778a29b7ab2e690fba3` | Factory Binary Firmware Dump |
| `89663-42084.bin` | **2001–2018** | 320.0 KB | `90d21b76b4e93bb77584a085daac9bc7` | Factory Binary Firmware Dump |
| `89663-42181.bin` | **2001–2018** | 320.0 KB | `30f10a92ff94492234cd47ede6739887` | Factory Binary Firmware Dump |
| `89663-42182.bin` | **2001–2018** | 320.0 KB | `f7fb7bab8803154069b628f1ebff507f` | Factory Binary Firmware Dump |
| `89663-42191.bin` | **2001–2018** | 320.0 KB | `b8274dc63fbb2aae68c8a80aeb211bc5` | Factory Binary Firmware Dump |
| `89663-42192.bin` | **2001–2018** | 320.0 KB | `3d2e775538eafe7d17c73403a0a1ccae` | Factory Binary Firmware Dump |
| `89663-42201.bin` | **2001–2018** | 384.0 KB | `22bf0a9195f78f0ae1978708adcbb7bc` | Factory Binary Firmware Dump |
| `89663-42202.bin` | **2001–2018** | 384.0 KB | `a77824cbcb020137e348958cd161daa3` | Factory Binary Firmware Dump |
| `89663-42211.bin` | **2001–2018** | 384.0 KB | `bf3f457616925d72d827f2320732b4e4` | Factory Binary Firmware Dump |
| `89663-42212.bin` | **2001–2018** | 384.0 KB | `63397731a618d65cb94a285a2548e60b` | Factory Binary Firmware Dump |
| `89663-42243.bin` | **2001–2018** | 736.0 KB | `70cb1b3137febd09357e56883bc6fe3e` | Factory Binary Firmware Dump |
| `89663-42341.bin` | **2001–2018** | 368.0 KB | `76fed51be6d7962d7295e7b42b48174e` | Factory Binary Firmware Dump |
| `89663-42351.bin` | **2001–2018** | 368.0 KB | `a8de7018b25b3f909446fd2736dbbb47` | Factory Binary Firmware Dump |
| `89663-42362.bin` | **2001–2018** | 496.0 KB | `0280d05345ff1c703bab0a574a1b2bc9` | Factory Binary Firmware Dump |
| `89663-42372.bin` | **2001–2018** | 496.0 KB | `c82aee5580a3e831248ae9d21c0c8620` | Factory Binary Firmware Dump |
| `89663-42631.bin` | **2001–2018** | 736.0 KB | `85473eac6325486301fcabf9d4988f53` | Factory Binary Firmware Dump |
| `89663-42711.bin` | **2001–2018** | 736.0 KB | `914d010d5501cde8f8bf0c420b739fe2` | Factory Binary Firmware Dump |
| `89663-42721.bin` | **2001–2018** | 736.0 KB | `a95858f7980d42ca2bd9051c2325cae0` | Factory Binary Firmware Dump |
| `89663-42731.bin` | **2001–2018** | 736.0 KB | `a1994660e260456da00523e57c0967a1` | Factory Binary Firmware Dump |
| `89663-42831.bin` | **2001–2018** | 736.0 KB | `96e6fc55e8aa0ca59e8fa48bbdf50a80` | Factory Binary Firmware Dump |
| `89663-42853.bin` | **2001–2018** | 736.0 KB | `5774e8383fb78f4b6beaf15da8d7b9c9` | Factory Binary Firmware Dump |
| `89663-42863.bin` | **2001–2018** | 736.0 KB | `49660e7130a2a09da55ebf6fdda5b129` | Factory Binary Firmware Dump |
| `89663-42A13.bin` | **2001–2018** | 992.0 KB | `b497fe43b70aec91ffd47e971bd9a850` | Factory Binary Firmware Dump |
| `89663-42A33.bin` | **2001–2018** | 992.0 KB | `3c2717496ce42ab6620511acdf2a4864` | Factory Binary Firmware Dump |
| `89663-42F03.bin` | **2001–2018** | 992.0 KB | `f752916fff1c140790e9d49f0dbe8940` | Factory Binary Firmware Dump |
| `89663-42F11.bin` | **2001–2018** | 992.0 KB | `775b35699a2e8272db161ae07111f50f` | Factory Binary Firmware Dump |
| `89663-42F13.bin` | **2001–2018** | 992.0 KB | `176ab3a02ae1a3edd3fa1317c4a34919` | Factory Binary Firmware Dump |
| `89663-42F40.bin` | **2001–2018** | 992.0 KB | `8973a3a3aa968c8e66b427d6d84a4704` | Factory Binary Firmware Dump |
| `89663-42N52.bin` | **2001–2018** | 992.0 KB | `c330a5301428004c431abb069e40c184` | Factory Binary Firmware Dump |
| `89663-42N62.bin` | **2001–2018** | 992.0 KB | `63d7d8c55b3d2dc80e643c59c4e3fdbe` | Factory Binary Firmware Dump |

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
