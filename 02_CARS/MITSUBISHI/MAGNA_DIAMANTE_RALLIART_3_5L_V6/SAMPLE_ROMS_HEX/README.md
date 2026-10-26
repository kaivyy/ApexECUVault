# SAMPLE ROMS HEX - ECU Calibration Suite

**Repository Path**: `02_CARS/MITSUBISHI/MAGNA_DIAMANTE_RALLIART_3_5L_V6/SAMPLE_ROMS_HEX`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `15 files` (15 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `SAMPLE_ROMS_HEX` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1996–2005

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `00 TH Executive 3-0 Auto.hex` | **2000** | 128.0 KB | `29e28b3c2edba41b971fc61aeff2e0c2` | Intel HEX Calibration Firmware |
| `00 TJ Solara 3-5 Auto.hex` | **2000** | 512.0 KB | `030e0fb3800f1c527e1da4c99aaa4e36` | Intel HEX Calibration Firmware |
| `00 TJ VR-X 3-5 Auto.hex` | **2000** | 512.0 KB | `78d44b0db984b08be55a78505d6110e8` | Intel HEX Calibration Firmware |
| `00 TJ VR-X 3-5 Manual.hex` | **2000** | 256.0 KB | `51cee78ffc93d09593e40654828728c0` | Intel HEX Calibration Firmware |
| `01 TJ LE (Comm Games) 3-5 Auto.hex` | **2001** | 512.0 KB | `36fe7a138dce32e7c2e81549d24e0780` | Intel HEX Calibration Firmware |
| `01 TJ VR-X MY02 3-5 Manual.hex` | **2001** | 256.0 KB | `33193ac19d6001b27dace25d6a349247` | Intel HEX Calibration Firmware |
| `01 USDM Diamante 3-5 Auto.hex` | **2001** | 512.0 KB | `dbcea2788bad4391445eb71db86d0517` | Intel HEX Calibration Firmware |
| `02 USDM Diamante 3-5 Auto.hex` | **2002** | 512.0 KB | `c57b71c99c0e655a6e7b7b7074044b88` | Intel HEX Calibration Firmware |
| `03 TJ AWD 3-5 Auto.hex` | **2003** | 512.0 KB | `075703b1b67d002ae574b7ec232e9842` | Intel HEX Calibration Firmware |
| `03 TJ Executive 3-5 Auto.hex` | **2003** | 256.0 KB | `426a7cadcfff10b04a0ae71b852d0698` | Intel HEX Calibration Firmware |
| `03 TJ Ralliart 3-5 Auto.hex` | **2003** | 512.0 KB | `552b1571e3608e846c3607e8893c915b` | Intel HEX Calibration Firmware |
| `03 TJ Ralliart 3-5 Manual.hex` | **2003** | 256.0 KB | `e8f313c8768f7a53e3c542a606d3e71c` | Intel HEX Calibration Firmware |
| `04 TL AWD 3-5 Auto.hex` | **2004** | 512.0 KB | `76f9cb2c9dd5a45c79553a37a5256708` | Intel HEX Calibration Firmware |
| `04 TL VR-X 3-5 Manual.hex` | **2004** | 256.0 KB | `133d81f75afc32b5f52453546581d313` | Intel HEX Calibration Firmware |
| `99 TH Sports 3-5 Manual.hex` | **1999** | 128.0 KB | `b313dff3624180f75e596a95b688b5ed` | Intel HEX Calibration Firmware |

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
