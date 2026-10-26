# CBR1000RR FIREBLADE - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/CBR_SPORT/CBR1000RR_FIREBLADE`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `40 files` (38 binary dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CBR1000RR_FIREBLADE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2004–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `38770-MEL-613.bin` | **2004–2024** | 256.0 KB | `a3547c584cc4e065b70ce8c98256510a` | Factory Binary Firmware Dump |
| `38770-MEL-643.bin` | **2004–2024** | 256.0 KB | `31bfcee982044e15831cfcdb5ce2a5fc` | Factory Binary Firmware Dump |
| `38770-MEL-672.bin` | **2004–2024** | 256.0 KB | `216ca37427461715240efac4ae495c6e` | Factory Binary Firmware Dump |
| `38770-MEL-772.bin` | **2004–2024** | 256.0 KB | `afe0a882abb63e22a6c1f66ecc3a00e3` | Factory Binary Firmware Dump |
| `38770-MEL-A21.bin` | **2004–2024** | 256.0 KB | `bff4a3e9c107241bb8bd649d88327993` | Factory Binary Firmware Dump |
| `38770-MEL-A22.bin` | **2004–2024** | 256.0 KB | `9a4aefc92652927b5de9de4a73dc6d71` | Factory Binary Firmware Dump |
| `38770-MEL-D01.bin` | **2004–2024** | 256.0 KB | `5317f766f02332817a51adac55950d7e` | Factory Binary Firmware Dump |
| `38770-MEL-D21.bin` | **2004–2024** | 256.0 KB | `3b5a0171e7a88090ec4465ec28426bad` | Factory Binary Firmware Dump |
| `38770-MEL-F21.bin` | **2004–2024** | 256.0 KB | `105661b8aebe610ea9789a1880c41daa` | Factory Binary Firmware Dump |
| `38770-MEL-L22.bin` | **2004–2024** | 256.0 KB | `822879077bf8bf50c3abef2a8674b2f8` | Factory Binary Firmware Dump |
| `38770-MEL.xdf` | **2004–2024** | 102.8 KB | `18eec9c7684c31c044c71c3ed5727f26` | TunerPro Binary Definition Map |
| `38770-MFL-622.bin` | **2004–2024** | 256.0 KB | `a469edb62eb524a0748be7aceaddacb7` | Factory Binary Firmware Dump |
| `38770-MFL-631.bin` | **2004–2024** | 256.0 KB | `77e25c0a36e4a69c919b33372860acd6` | Factory Binary Firmware Dump |
| `38770-MFL-644.bin` | **2004–2024** | 256.0 KB | `6dcb21f697b1a7da5b0884571536b4f6` | Factory Binary Firmware Dump |
| `38770-MFL-671.bin` | **2004–2024** | 256.0 KB | `f74c4d596481a581dcd23ac3d63f846f` | Factory Binary Firmware Dump |
| `38770-MFL-691.bin` | **2004–2024** | 256.0 KB | `d917325508447d48aa38cef35c409bc5` | Factory Binary Firmware Dump |
| `38770-MFL-702.bin` | **2004–2024** | 256.0 KB | `a9649caa83ed794ebe36a020fdc8178f` | Factory Binary Firmware Dump |
| `38770-MFL-741.bin` | **2004–2024** | 256.0 KB | `0f44e20d7dea5c95157cf41c5ebc6be0` | Factory Binary Firmware Dump |
| `38770-MFL-761.bin` | **2004–2024** | 256.0 KB | `9d08caf02fdead1e4647c3d0e73f9065` | Factory Binary Firmware Dump |
| `38770-MFL-773.bin` | **2004–2024** | 256.0 KB | `9f540444500d7f3da0c0384d10c461a6` | Factory Binary Firmware Dump |
| `38770-MFL-861.bin` | **2004–2024** | 256.0 KB | `8eb7c11f6cce6e4844896ecd56630ed6` | Factory Binary Firmware Dump |
| `38770-MFL-871.bin` | **2004–2024** | 256.0 KB | `b35a7c1edcf9c7d31c43a4545a4ad4f5` | Factory Binary Firmware Dump |
| `38770-MFL-A21.bin` | **2004–2024** | 256.0 KB | `566e5379f862e29064a7b6a61059ee73` | Factory Binary Firmware Dump |
| `38770-MFL-D21.bin` | **2004–2024** | 256.0 KB | `52dd1534dfe38eb2fddfe319b716c02c` | Factory Binary Firmware Dump |
| `38770-MFL-F21.bin` | **2004–2024** | 256.0 KB | `6ff2f8e2122134d6fdc0706730e821c9` | Factory Binary Firmware Dump |
| `38770-MFL-J21.bin` | **2004–2024** | 256.0 KB | `fc496239d752f563f05fe6756a02baf6` | Factory Binary Firmware Dump |
| `38770-MFL-J41.bin` | **2004–2024** | 256.0 KB | `06e127927748cdd87b21c6f78d6e4357` | Factory Binary Firmware Dump |
| `38770-MFL-L21.bin` | **2004–2024** | 256.0 KB | `cd5381d89fc000b0dd9c6d640a1eb754` | Factory Binary Firmware Dump |
| `38770-MGP-A01.bin` | **2004–2024** | 256.0 KB | `f413f5bbb98943759172be4515d58a82` | Factory Binary Firmware Dump |
| `38770-MGP-A92.bin` | **2004–2024** | 256.0 KB | `328482096806497eecc516783ee3dbe8` | Factory Binary Firmware Dump |
| `38770-MGP-D01.bin` | **2004–2024** | 256.0 KB | `1f8694a9815a91e797da6a4013228cdb` | Factory Binary Firmware Dump |
| `38770-MGP-D62.bin` | **2004–2024** | 256.0 KB | `dea0de53cd2a0e7f5acb9b0c20b51ee3` | Factory Binary Firmware Dump |
| `38770-MGP-F01.bin` | **2004–2024** | 256.0 KB | `6ba0940cda716cccedcf902a6a0b2f8a` | Factory Binary Firmware Dump |
| `38770-MGP-F63.bin` | **2004–2024** | 256.0 KB | `f79fb005310ce70f0f8dd77cc02f5568` | Factory Binary Firmware Dump |
| `38770-MGP-L01.bin` | **2004–2024** | 256.0 KB | `77e7b178138477fca47d8ecbf02be622` | Factory Binary Firmware Dump |
| `38770-MKF-D43.bin` | **2004–2024** | 1.00 MB | `89535f291af29628a042399cf16fc71b` | Factory Binary Firmware Dump |
| `38770-MKF-D72.bin` | **2004–2024** | 1.00 MB | `536b4699bc61adc10a0210da4bf0b9c6` | Factory Binary Firmware Dump |
| `38770-MKF-L13.bin` | **2004–2024** | 1.00 MB | `7804b6309b93a05c294b8639a826f2d2` | Factory Binary Firmware Dump |
| `38770-MKF-TK2.bin` | **2004–2024** | 1.00 MB | `675d888b2463aac8d7b30ff045adab4f` | Factory Binary Firmware Dump |
| `CBR1000RR_2012_US.xdf` | **2012** | 62.1 KB | `fdd4c76d8680c68f5128286802c1b25d` | TunerPro Binary Definition Map |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro yang tersedia, struktur kalibrasi mencakup parameter esensial:
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
