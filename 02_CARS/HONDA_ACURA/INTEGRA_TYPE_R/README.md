# INTEGRA_TYPE_R - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/INTEGRA_TYPE_R`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `25 files` (25 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `INTEGRA_TYPE_R` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1995–2006

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `Int338gr.bin` | **1995–2006** | 48.0 KB | `264e10128d8b21727ca37801b08c56cc` | Factory Binary Firmware Dump |
| `Int340ls.bin` | **1995–2006** | 48.0 KB | `575deaa0e55e51431bd31fe795ab1259` | Factory Binary Firmware Dump |
| `Int359tr.bin` | **1995–2006** | 48.0 KB | `0a79ba65e11c63beee11a8e0b46a5b33` | Factory Binary Firmware Dump |
| `Int422gr.bin` | **1995–2006** | 48.0 KB | `429dae21e8e7c68468ad8be82f94992b` | Factory Binary Firmware Dump |
| `Int474gr.bin` | **1995–2006** | 48.0 KB | `f7f01f2db5d9ee7ffba18edf3c13eca2` | Factory Binary Firmware Dump |
| `Int475ls.bin` | **1995–2006** | 48.0 KB | `68613a835f5e6ac68b92ad40dc837ec6` | Factory Binary Firmware Dump |
| `Int497tr.bin` | **1995–2006** | 48.0 KB | `4ca311f462f1d35847b9754ffc567b8b` | Factory Binary Firmware Dump |
| `Int712gr.bin` | **1995–2006** | 48.0 KB | `f4bb112e8924b2354f8409bb06a38930` | Factory Binary Firmware Dump |
| `P73_M66507-715.bin` | **1995–2006** | 48.0 KB | `7abb209ca071708c7f96fee40af640dd` | Factory Binary Firmware Dump |
| `P74-USDM-214.bin` | **1995–2006** | 32.0 KB | `1c7b48c6dd70e23771a9a8c73f7a5cb4` | Factory Binary Firmware Dump |
| `PR3-900-93.bin` | **1995–2006** | 32.0 KB | `37a1d2d4585cff0dde8e3a9e76e2bbbc` | Factory Binary Firmware Dump |
| `PR3GSR.bin` | **1995–2006** | 32.0 KB | `7da9829e2865e9bb9d38a662a46b0ddc` | Factory Binary Firmware Dump |
| `STOCK-PR3.bin` | **1995–2006** | 32.0 KB | `5490eff6ba0981a520ffe499ff0d19f5` | Factory Binary Firmware Dump |
| `int233stock.bin` | **1995–2006** | 32.0 KB | `d8162fe1dd0efd3b8c86187fc8d41517` | Factory Binary Firmware Dump |
| `p2p_p75-rom.bin` | **1995–2006** | 32.0 KB | `92eb7bead98f2a7b92f4c934a6f2d065` | Factory Binary Firmware Dump |
| `p75-q01-270.bin` | **1995–2006** | 32.0 KB | `1786d82785ae4835093db38aa3bff6b5` | Factory Binary Firmware Dump |
| `pr3-901-58.bin` | **1995–2006** | 32.0 KB | `42f24a6afb95f4568e63bc5b20e98b07` | Factory Binary Firmware Dump |
| `pr3-j01-205.bin` | **1995–2006** | 32.0 KB | `3e40bf6b2821e513bdde2e9ce64260df` | Factory Binary Firmware Dump |
| `pr3-j51-219.bin` | **1995–2006** | 32.0 KB | `b1a63fc1a7796f6414bbbfc72c828f60` | Factory Binary Firmware Dump |
| `pr4-USDM-232.bin` | **1995–2006** | 32.0 KB | `33469c6ffe8b506a0c1a8cfbca743a49` | Factory Binary Firmware Dump |
| `pr4-a02.bin.bin` | **1995–2006** | 32.0 KB | `146bdfb053ff2d90612ec9e33e9a74d4` | Factory Binary Firmware Dump |
| `pr4-q02-54.rom` | **1995–2006** | 32.0 KB | `50fc882709993c8b9684de395cf4b81e` | Factory Binary Firmware Dump |
| `pr4-q51-33.bin` | **1995–2006** | 32.0 KB | `c3f4edc311f96aff3d86c19f4694662f` | Factory Binary Firmware Dump |
| `pr4-q60-92.bin` | **1995–2006** | 32.0 KB | `f7cd387a42778e07a1de54b9fe08e105` | Factory Binary Firmware Dump |
| `pr4-q61-235.bin` | **1995–2006** | 32.0 KB | `b9b35ec946dbb080f7c06d95acdb3692` | Factory Binary Firmware Dump |

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
