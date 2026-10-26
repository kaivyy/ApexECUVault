# P01 512Kb - ECU Calibration Suite

**Repository Path**: `02_CARS/GM_CHEVROLET/LS_V8_GEN3_GEN4/.XDF Files/P01_512Kb`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `34 files` (30 binary dumps, 4 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `P01_512Kb` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: OEM Production

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `'01 C1500 LM7 os12208322.bin` | **2001** | 512.0 KB | `dc8741067b31fce1a74a88456164a14c` | Factory Binary Firmware Dump |
| `'01 GMC c1500 LM7 os 12208322.bin` | **2001** | 512.0 KB | `ba98023374ab41ed3aa9652a3cd96129` | Factory Binary Firmware Dump |
| `'01 K1500 4.8 LR4 os12208322.bin` | **2001** | 512.0 KB | `fca2b93c60909bd1f233f86927607d05` | Factory Binary Firmware Dump |
| `'01 K2500 8.1L18 0s12208322.bin` | **2001** | 512.0 KB | `309656e529aec44ce9d949873d0538a1` | Factory Binary Firmware Dump |
| `'01 LM7 os12208322.bin` | **2001** | 512.0 KB | `dc8741067b31fce1a74a88456164a14c` | Factory Binary Firmware Dump |
| `'01C1500 LM7 os12208322.bin` | **1999–2002 (P01)** | 512.0 KB | `b442ef77351cfcdfac594125f3c36141` | Factory Binary Firmware Dump |
| `'01K2500 6.0L os12208322.bin` | **1999–2002 (P01)** | 512.0 KB | `e02c04385d5323db5c8a0d913f204886` | Factory Binary Firmware Dump |
| `01 LM7 12202088 (1).bin` | **2001** | 512.0 KB | `18ad0009d5aecbd08507ada55a71507e` | Factory Binary Firmware Dump |
| `01 LM7 12202088.bin` | **2001** | 512.0 KB | `18ad0009d5aecbd08507ada55a71507e` | Factory Binary Firmware Dump |
| `01 chevy MPV 4x4 Half T LM7 os12208322.bin` | **2001** | 512.0 KB | `4dab85f1aa344500eca42a4260abb648` | Factory Binary Firmware Dump |
| `12202088 - 2001 512k.xdf` | **2001** | 617.5 KB | `f100e3a728d6b40bd1da32c831cfb3be` | TunerPro Binary Definition Map |
| `12208322 - 2001 512k.xdf` | **2001** | 617.5 KB | `0742ffff2c2ca927c638c6f546073edd` | TunerPro Binary Definition Map |
| `12209203 - 2002 512k V1.xdf` | **2002** | 588.1 KB | `b706e5a686283cbf25f9cd2dda54f58f` | TunerPro Binary Definition Map |
| `12212156 - 2002 512k V1.xdf` | **2002** | 588.1 KB | `56f1f73f8e4306b4d97913a794f5ef3f` | TunerPro Binary Definition Map |
| `2001 5.3 Auto OS12208322.bin` | **2001** | 512.0 KB | `1bbe1d698bb2e4d7476113493dadb26f` | Factory Binary Firmware Dump |
| `2001 8.1 12208322.bin` | **2001** | 512.0 KB | `54244ec3cff1831ac914e488e827befc` | Factory Binary Firmware Dump |
| `2001 Chevrolet Silverado Truck Automatic LQ4 6.0 Litre (12208322).bin` | **2001** | 512.0 KB | `dcb1714dd8a0ccc82f40f07a5108dc8f` | Factory Binary Firmware Dump |
| `2001 Chevy 1500 4x2 4.8 LR4 12208322.bin` | **2001** | 512.0 KB | `1f321826a57415ab8e6d97a8fc6b29e6` | Factory Binary Firmware Dump |
| `2001 Chevy S-10 L35 4.3L 4L60E (12202088).bin` | **2001** | 512.0 KB | `b15c78939740180888c087ebdfe21163` | Factory Binary Firmware Dump |
| `2001 Chevy Tahoe LM7 5.3L Auto (12202088).bin` | **2001** | 512.0 KB | `4ceb219cacd6b2a5f5f361510fac86f1` | Factory Binary Firmware Dump |
| `20014.84x4 12208322.bin` | **1999–2002 (P01)** | 512.0 KB | `fca2b93c60909bd1f233f86927607d05` | Factory Binary Firmware Dump |
| `2001_6.0_2500_2wd _Cal_OS12202088.bin` | **2001** | 512.0 KB | `27bcf28b45720ba064694ebc7cc6b577` | Factory Binary Firmware Dump |
| `2001_6.0_OS12208322.bin` | **2001** | 512.0 KB | `dcb1714dd8a0ccc82f40f07a5108dc8f` | Factory Binary Firmware Dump |
| `2002 4.8L LR4 4x2 1-2T MANUAL TRANS os12212156.bin` | **2002** | 512.0 KB | `177a2bfd1a26006e2378618dc6a9374a` | Factory Binary Firmware Dump |
| `2002 5.3L 2wd Stock DBC No EGR 12212156.bin` | **2002** | 512.0 KB | `6694c5961f93de2f8f0130647603e7ec` | Factory Binary Firmware Dump |
| `2002 Chevrolet Express Van Automatic L31 5.7L 4L60e 2wd (12212156) Lean Cruise (1).bin` | **2002** | 512.0 KB | `7d07f3cdc53881af805336b9e1d2ccd0` | Factory Binary Firmware Dump |
| `2002 Chevrolet Express Van Automatic L31 5.7L 4L60e 2wd (12212156) Lean Cruise.bin` | **2002** | 512.0 KB | `7d07f3cdc53881af805336b9e1d2ccd0` | Factory Binary Firmware Dump |
| `2002 Chevrolet Express Van L31 5.7 Litre 4L80E(12212156).bin` | **2002** | 512.0 KB | `cfefc4bf9306f47a51cdb10533b77907` | Factory Binary Firmware Dump |
| `2002 Chevrolet Silverado Truck Auto LM7 5.3L (12212156) (1).bin` | **2002** | 512.0 KB | `05377159d32794dac3dda81f9e30cbb8` | Factory Binary Firmware Dump |
| `2002 Chevrolet Silverado Truck Auto LM7 5.3L (12212156).bin` | **2002** | 512.0 KB | `05377159d32794dac3dda81f9e30cbb8` | Factory Binary Firmware Dump |
| `2002 Chevrolet Silverado Truck Manual LM7 5.3 Litre (12212156) (1).bin` | **2002** | 512.0 KB | `bc4516bb3aaa4c2ea4975b46d3696126` | Factory Binary Firmware Dump |
| `2002 Chevrolet Silverado Truck Manual LM7 5.3 Litre (12212156).bin` | **2002** | 512.0 KB | `bc4516bb3aaa4c2ea4975b46d3696126` | Factory Binary Firmware Dump |
| `2002 Chevy S-10 L35 4.3L 4L60E (12212156).bin` | **2002** | 512.0 KB | `0c64d7ceddad860c30b88d2922c24ec6` | Factory Binary Firmware Dump |
| `2002 Chevy S-10 L35 4.3L 4L60E (12212156)Lean Cruise.bin` | **2002** | 512.0 KB | `8d787123561de59bf70cd29a456c41bc` | Factory Binary Firmware Dump |

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
