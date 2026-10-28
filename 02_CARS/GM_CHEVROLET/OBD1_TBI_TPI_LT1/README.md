# OBD1_TBI_TPI_LT1 - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/OBD1_TBI_TPI_LT1`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `26 files` (26 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `OBD1_TBI_TPI_LT1` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `2240AYFP.BIN` | **2000–2024** | 64.0 KB | `0b4b86ec7594e0183ebfc9e1b529a857` | Factory Binary Firmware Dump |
| `ANZA.bin` | **2000–2024** | 16.0 KB | `bac00c6ed052846369efa5c632a1b0c4` | Factory Binary Firmware Dump |
| `APYP.bin` | **2000–2024** | 16.0 KB | `dc9f6c758832e709320553b96b3f6fb8` | Factory Binary Firmware Dump |
| `ARAP.bin` | **2000–2024** | 16.0 KB | `85c39ceefcee8f26ce8f41168ed6992c` | Factory Binary Firmware Dump |
| `AYCF6730 88.BIN` | **2000–2024** | 32.0 KB | `a49fcfe4b2c67b24256328cf5fd3cf76` | Factory Binary Firmware Dump |
| `Abyr4326 88.bin` | **2000–2024** | 32.0 KB | `156f5391abed9852f2a7999a301135bf` | Factory Binary Firmware Dump |
| `Arpl 88.bin` | **2000–2024** | 32.0 KB | `b6293a0cc5a7c513ffd8fe82d0fa6485` | Factory Binary Firmware Dump |
| `Atj9188 88.bin` | **2000–2024** | 32.0 KB | `65fe2a269b4b7cbac400bd0118ffdf64` | Factory Binary Firmware Dump |
| `Atmf5241 88.bin` | **2000–2024** | 32.0 KB | `65e7e153b933d7b9af566dfa6770422b` | Factory Binary Firmware Dump |
| `Atta6656 88.bin` | **2000–2024** | 32.0 KB | `8e646d563a32dfd713155e9b3959a0ee` | Factory Binary Firmware Dump |
| `BCKC 11.BIN` | **2000–2024** | 64.0 KB | `52d88f2ffcf9630c4560d92f47604474` | Factory Binary Firmware Dump |
| `BDJZ.bin` | **2000–2024** | 64.0 KB | `31cbe8ad8ccbab03a24787928f762ecc` | Factory Binary Firmware Dump |
| `BFFK1287.BIN` | **2000–2024** | 64.0 KB | `a8c2ab8e49fd0402164819f4807c7734` | Factory Binary Firmware Dump |
| `BFPL2416.BIN` | **2000–2024** | 64.0 KB | `c9a80d556704e96fa2b06663eb78d85b` | Factory Binary Firmware Dump |
| `BFPM 12.BIN` | **2000–2024** | 32.0 KB | `28e6ab94694bad544b53d6d68e9f2dd9` | Factory Binary Firmware Dump |
| `BFUZ.BIN` | **2000–2024** | 32.0 KB | `5a7cdbc25d430724d61906c7f2834b2f` | Factory Binary Firmware Dump |
| `BJKT8015.BIN` | **2000–2024** | 64.0 KB | `1c9d1937ba86908b182d468216860cf8` | Factory Binary Firmware Dump |
| `BJLK.bin` | **2000–2024** | 64.0 KB | `f14dc08de58013df597011e4f0f4b46d` | Factory Binary Firmware Dump |
| `BJWN.Bin` | **2000–2024** | 64.0 KB | `fb048a75993bb5b969b078de9dd3ca26` | Factory Binary Firmware Dump |
| `BJYM 0D.bin` | **2000–2024** | 64.0 KB | `425f3fe075126c6b7b69356995a7c58e` | Factory Binary Firmware Dump |
| `BLCH5094.BIN` | **2000–2024** | 64.0 KB | `bf1c366592be7e6b161b258c6d293cf8` | Factory Binary Firmware Dump |
| `BLYN8253.BIN` | **2000–2024** | 64.0 KB | `bfbfc78db8684b70c6e02dcfbee29a5b` | Factory Binary Firmware Dump |
| `Bawx 88.bin` | **2000–2024** | 32.0 KB | `3d57b6b1ff7239945502b15e6044e03f` | Factory Binary Firmware Dump |
| `Cld4324 88.bin` | **2000–2024** | 32.0 KB | `c58fa5f508ebb77a6383f984cfc448ff` | Factory Binary Firmware Dump |
| `atds 88.bin` | **2000–2024** | 32.0 KB | `93b872e21e2a286e8145314d1c2086ef` | Factory Binary Firmware Dump |
| `azty1407 88.bin` | **2000–2024** | 32.0 KB | `d665d66733b1379580f17fbeebee6788` | Factory Binary Firmware Dump |

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
