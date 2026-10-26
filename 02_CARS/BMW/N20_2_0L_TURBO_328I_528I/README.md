# N20 2 0L TURBO 328I 528I - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/N20_2_0L_TURBO_328I_528I`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `12 files` (12 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `N20_2_0L_TURBO_328I_528I` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2011–2017

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `00000ABF3BA001_n20o1_original.bin` | **2011–2017** | 4.00 MB | `5687afc10dc179d450144940c3ff6b67` | Factory Binary Firmware Dump |
| `00000ABF3BA001_original.bin` | **2011–2017** | 4.00 MB | `2e98a51eae98cd164df41a459065c77a` | Factory Binary Firmware Dump |
| `0000113D3BA001_n20o1_original.bin` | **2011–2017** | 4.00 MB | `d41efa5e96d319f543e4095ec8698b9c` | Factory Binary Firmware Dump |
| `0000113D3BA001_original.bin` | **2011–2017** | 4.00 MB | `6a761f89406c1877f908d54c9c63643f` | Factory Binary Firmware Dump |
| `000013E713AA01_n20o1_original.bin` | **2011–2017** | 4.00 MB | `25e81bbc76f11d2588c6124e7128585a` | Factory Binary Firmware Dump |
| `000013E713AA01_original.bin` | **2011–2017** | 4.00 MB | `e32bf56d3e0fad8cf8c0f26b03bb24ca` | Factory Binary Firmware Dump |
| `000019A813AA01_n20o1_original.bin` | **2011–2017** | 4.00 MB | `ed829b922c1cf74634035f9251cfbcbe` | Factory Binary Firmware Dump |
| `000019A813AA01_original.bin` | **2011–2017** | 4.00 MB | `719221dce7d4e833fac8b0695a5adbd6` | Factory Binary Firmware Dump |
| `00001BC91D9601_n20o1_original.bin` | **2011–2017** | 4.00 MB | `492dd4e3da430c6a61b8ebed77245de3` | Factory Binary Firmware Dump |
| `00001BC91D9601_original.bin` | **2011–2017** | 4.00 MB | `016b16866faed4a13b83b9cc54b7adcd` | Factory Binary Firmware Dump |
| `00001C9F1D9601_n20o1_original.bin` | **2011–2017** | 4.00 MB | `ccda51f278928f4edbbd170ff9f33426` | Factory Binary Firmware Dump |
| `00001C9F1D9601_original.bin` | **2011–2017** | 4.00 MB | `57ffa57f20ff903a39677996d044129b` | Factory Binary Firmware Dump |

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
