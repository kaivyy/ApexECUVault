# ECUFLASH_XML_DEFS - ECU Calibration Suite

**Repository Path**: `02_CARS/MITSUBISHI/MAGNA_DIAMANTE_RALLIART_3_5L_V6/ECUFLASH_XML_DEFS`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `31 files` (0 binary dumps, 31 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ECUFLASH_XML_DEFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `22490005.xml` | **1996–2005** | 12.0 KB | `6252daf1ccf8d6d0a7f77a88daaa687f` | ECU / XML Calibration Map Definition |
| `22520004.xml` | **1996–2005** | 12.0 KB | `387a3ee7ccf561e860a6c239347429f2` | ECU / XML Calibration Map Definition |
| `22600000.xml` | **1996–2005** | 11.8 KB | `a319d1b2eb7c84acbc10fdd71030255b` | ECU / XML Calibration Map Definition |
| `22620000.xml` | **1996–2005** | 11.8 KB | `e5eceafd5d96db4630386c74ba29a174` | ECU / XML Calibration Map Definition |
| `23430000.xml` | **1996–2005** | 11.8 KB | `1b0c29a7d6f9515b35ba235782b5b3bb` | ECU / XML Calibration Map Definition |
| `80350003.xml` | **1996–2005** | 15.3 KB | `6c22f38599fc340ef5fb444f69860768` | ECU / XML Calibration Map Definition |
| `81930003.xml` | **1996–2005** | 15.3 KB | `91f7ff0dedff9cd099906215e587d86c` | ECU / XML Calibration Map Definition |
| `82000001.xml` | **1996–2005** | 15.2 KB | `35fd2f594f3832efa1170b4cda9c0718` | ECU / XML Calibration Map Definition |
| `82000002.xml` | **1996–2005** | 15.2 KB | `fb36165904e0bbf14e77939b1f1b4f4e` | ECU / XML Calibration Map Definition |
| `82030001.xml` | **1996–2005** | 15.2 KB | `d179268b0929b223065f396fdbfadd6b` | ECU / XML Calibration Map Definition |
| `82030002.xml` | **1996–2005** | 15.2 KB | `9edc0c79a541f3bf708e54b1f82af517` | ECU / XML Calibration Map Definition |
| `82450006.xml` | **1996–2005** | 15.2 KB | `540c2a021c3b5bf9bba9c479629f26cd` | ECU / XML Calibration Map Definition |
| `83890006.xml` | **1996–2005** | 15.3 KB | `ff870d8847daed0a7cb495420ebf7576` | ECU / XML Calibration Map Definition |
| `85490000.xml` | **1996–2005** | 15.1 KB | `386dad764548811568c17fb1cd27fe60` | ECU / XML Calibration Map Definition |
| `85490001.xml` | **1996–2005** | 15.1 KB | `09f50f4ac7dadf4fa8f2ecba797f7d42` | ECU / XML Calibration Map Definition |
| `87190003.xml` | **1996–2005** | 15.9 KB | `dcca595231d64558b17a7100ecd4fe71` | ECU / XML Calibration Map Definition |
| `87200002.xml` | **1996–2005** | 632 B | `3aca20aaaaeb4660654e5b34402643f5` | ECU / XML Calibration Map Definition |
| `87200004.xml` | **1996–2005** | 15.2 KB | `a730928d7754fa90ff9de4db45854e51` | ECU / XML Calibration Map Definition |
| `87200005a.xml` | **1996–2005** | 15.2 KB | `e2b70e7b5fd18081145685bf96569a89` | ECU / XML Calibration Map Definition |
| `87200005b.xml` | **1996–2005** | 649 B | `83d383f9af666e4ff50bbd1bc2efaa73` | ECU / XML Calibration Map Definition |
| `87410004.xml` | **1996–2005** | 15.3 KB | `5e6b65f269a77d48c737be09dc341367` | ECU / XML Calibration Map Definition |
| `91760000.xml` | **1996–2005** | 626 B | `82dad44e7f069b6df8275fdbd965f019` | ECU / XML Calibration Map Definition |
| `91760002.xml` | **1996–2005** | 13.0 KB | `767bfee07016d61dc763d1a433bac5ab` | ECU / XML Calibration Map Definition |
| `91970002.xml` | **1996–2005** | 12.9 KB | `bcad5fce69c23110415eec673b711760` | ECU / XML Calibration Map Definition |
| `97180003.xml` | **1996–2005** | 13.8 KB | `46e290bbf3f5ebfbdf4d9a3ddc5ce815` | ECU / XML Calibration Map Definition |
| `97180004.xml` | **1996–2005** | 621 B | `0dc4a2fbd5573ca6c277482c9e762335` | ECU / XML Calibration Map Definition |
| `97190002.xml` | **1996–2005** | 13.7 KB | `14bfb72dcce2a898698e69a3a2d76ef1` | ECU / XML Calibration Map Definition |
| `98320000.xml` | **1996–2005** | 13.0 KB | `175d03e8517184b0079d8559e9aaccbc` | ECU / XML Calibration Map Definition |
| `98320001.xml` | **1996–2005** | 621 B | `33c6b603b4a9076da847eea32e8d36ff` | ECU / XML Calibration Map Definition |
| `magna_3g_at_base.xml` | **1996–2005** | 7.0 KB | `557f9bb2b6c2551fa1676e8e73d0d400` | ECU / XML Calibration Map Definition |
| `magna_3g_base.xml` | **1996–2005** | 51.4 KB | `50e333616771f081e3326cccd4fb3576` | ECU / XML Calibration Map Definition |

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
