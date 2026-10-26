# DELPHI DYNO TUNES - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HARLEY_DAVIDSON_INDIAN/DELPHI_DYNO_TUNES`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `33 files` (33 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `DELPHI_DYNO_TUNES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233new.ori` | `.ORI` | `196,863` bytes | Original Hardware Read Dump |
| `1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233rk.ori` | `.ORI` | `191,646` bytes | Original Hardware Read Dump |
| `1HD1HBZ115K802247_32498-05_127_0000000201_1328.ori` | `.ORI` | `67,952` bytes | Original Hardware Read Dump |
| `1HD1KTC37JB676262_RadioInfo.bin` | `.BIN` | `20` bytes | Binary Firmware / Calibration Dump |
| `1HD1KTM12FB697962_41000057_617_0004080F01_2233.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `1HD1KTP27LB649034_RadioInfo.bin` | `.BIN` | `20` bytes | Binary Firmware / Calibration Dump |
| `1HD1KTP3XKB630226_RadioInfo.bin` | `.BIN` | `20` bytes | Binary Firmware / Calibration Dump |
| `AmericanSpeed_-_Delfi_Centurion_blue flhx.ori` | `.ORI` | `65,904` bytes | Original Hardware Read Dump |
| `BigBaggerBonzai_-_Delfi_Centurion_ed h.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `BigBaggerBonzai_-_Delfi_Centurion_ed.ori` | `.ORI` | `110,892` bytes | Original Hardware Read Dump |
| `BigBerthaWorthit-_-_Delfi_Centurion_CenturionIntRegistration.bin` | `.BIN` | `700` bytes | Binary Firmware / Calibration Dump |
| `BigBerthaWorthit-_-_Delfi_Centurion_beeneychinswap.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `BigBerthaWorthit-_-_Delfi_Centurion_beeneyswap2.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `BigBerthaWorthit-_-_Delfi_Centurion_chin.ori` | `.ORI` | `90,318` bytes | Original Hardware Read Dump |
| `CenturionIntRegistration.bin` | `.BIN` | `700` bytes | Binary Firmware / Calibration Dump |
| `DontFugganDieDarleeng_-_Delfi_Centurion_1HD1KTM12FB697962_41000057_617_0004080F01_2233.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `FatTireFelisha_-_Delfi_Centurion_1HD1HBZ115K802247_32498-05_127_0000000201_1328.ori` | `.ORI` | `67,952` bytes | Original Hardware Read Dump |
| `GaggBaggerGertruude_-_Delfi_Centurion_1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `GaggBaggerGertruude_-_Delfi_Centurion_1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233new.ori` | `.ORI` | `196,863` bytes | Original Hardware Read Dump |
| `GaggBaggerGertruude_-_Delfi_Centurion_1HD1FBM33GB634368_41000057_41000184F   _617_00060C0F01_2233rk.ori` | `.ORI` | `191,646` bytes | Original Hardware Read Dump |
| `GaggBaggerGertruude_-_Delfi_Centurion_jayder.ori` | `.ORI` | `187,495` bytes | Original Hardware Read Dump |
| `HorsePowerbySurina_-_Delfi_Centurion_rodney rg.ori` | `.ORI` | `67,952` bytes | Original Hardware Read Dump |
| `Lil-Susie_-_Delfi_Centurion_streetglide.ori` | `.ORI` | `67,952` bytes | Original Hardware Read Dump |
| `beeneychinswap.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `beeneyswap2.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `blue flhx.ori` | `.ORI` | `65,904` bytes | Original Hardware Read Dump |
| `chin.ori` | `.ORI` | `90,318` bytes | Original Hardware Read Dump |
| `ed h.ori` | `.ORI` | `168,189` bytes | Original Hardware Read Dump |
| `ed.ori` | `.ORI` | `110,892` bytes | Original Hardware Read Dump |
| `jayder.ori` | `.ORI` | `187,495` bytes | Original Hardware Read Dump |
| `rodney rg.ori` | `.ORI` | `67,952` bytes | Original Hardware Read Dump |
| `streetglide.ori` | `.ORI` | `67,952` bytes | Original Hardware Read Dump |

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
