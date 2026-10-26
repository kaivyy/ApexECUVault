# ORIGINAL BINS - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/ORIGINAL_BINS`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `26 files` (26 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ORIGINAL_BINS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2014–2020

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `00000D07596401_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `22f4467bf1ea293466a2cf3c97595d66` | Factory Binary Firmware Dump |
| `00000D07596401_original.bin` | **2014–2020** | 4.00 MB | `e5ced22adfcc37ae04010bd1757afcc2` | Factory Binary Firmware Dump |
| `00000E2B3B0A01_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `c5830c4d9e58945730e26df2a8a51404` | Factory Binary Firmware Dump |
| `00000E2B3B0A01_original.bin` | **2014–2020** | 4.00 MB | `9ec1f0116c862471f366b45274b1b175` | Factory Binary Firmware Dump |
| `00000FEF81A001_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `ad12310982ab8aa554d816d48440c553` | Factory Binary Firmware Dump |
| `00000FEF81A001_original.bin` | **2014–2020** | 4.00 MB | `2141d6f1bdb333648c551f0627539991` | Factory Binary Firmware Dump |
| `00001A841D1401_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `00e722618d0099967cef01acf498edf8` | Factory Binary Firmware Dump |
| `00001A841D1401_original.bin` | **2014–2020** | 4.00 MB | `00fb6d68da0d1da072bdac473f9d24e2` | Factory Binary Firmware Dump |
| `00001A841D2801_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `2987e6721b32d15a86c419b9b964ffc4` | Factory Binary Firmware Dump |
| `00001A841D2801_original.bin` | **2014–2020** | 4.00 MB | `1dd5c21041f21977d3018fb19d574546` | Factory Binary Firmware Dump |
| `00001C41279601_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `6cea001165ae87fe938f22281285675d` | Factory Binary Firmware Dump |
| `00001C41279601_original.bin` | **2014–2020** | 4.00 MB | `f580fb866af36e4cf777a65c4f1a0ee0` | Factory Binary Firmware Dump |
| `000021571D8202_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `0e1e9492e73620de9ccf62b143aa736f` | Factory Binary Firmware Dump |
| `000021571D8202_original.bin` | **2014–2020** | 4.00 MB | `f366030dba59706a62ab3befa574750a` | Factory Binary Firmware Dump |
| `000021571DAA01_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `13e3c907a38db3bf1bf02502df7aee98` | Factory Binary Firmware Dump |
| `000021571DAA01_original.bin` | **2014–2020** | 4.00 MB | `f79e479bdcde078a4ad6c6ce37adbfdc` | Factory Binary Firmware Dump |
| `000021571DBE01_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `f33f8fd2aa2b1ed7ea02e700f384db05` | Factory Binary Firmware Dump |
| `000021571DBE01_original.bin` | **2014–2020** | 4.00 MB | `8852385a6d9953eceff1e570e7d3b0e0` | Factory Binary Firmware Dump |
| `00002DF2132801_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `09238e53da6a3fe2f1e0d73dac479b6d` | Factory Binary Firmware Dump |
| `00002DF2132801_original.bin` | **2014–2020** | 4.00 MB | `b5f8af6342fa39902c1f2126e4011086` | Factory Binary Firmware Dump |
| `00005BA8134601_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `df04508b920e9b79d08c44afd9b4deae` | Factory Binary Firmware Dump |
| `00005BA8134601_original.bin` | **2014–2020** | 4.00 MB | `849a1be62b6ca75aede391ad419d2a73` | Factory Binary Firmware Dump |
| `00005BA8135001_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `033bc84fddd71ecfee6d466bceaaf67f` | Factory Binary Firmware Dump |
| `00005BA8135001_original.bin` | **2014–2020** | 4.00 MB | `1a1d5d8d08827fd68e18ce91fc4fca9d` | Factory Binary Firmware Dump |
| `00005BA8135A01_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `3401426fa2c085eac040c4d80ae678dc` | Factory Binary Firmware Dump |
| `00005BA8135A01_original.bin` | **2014–2020** | 4.00 MB | `28c681bd80da47f4fe54508af611d83f` | Factory Binary Firmware Dump |

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
