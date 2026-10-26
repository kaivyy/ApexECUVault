# MSS54HP - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/M_POWER_MSS54_M3_CSL/03_BIN_PARTIAL_CALIBRATIONS/MSS54HP`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `42 files` (42 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MSS54HP` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `211323001601J424 (EU3 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601J429 (US 6MT non-heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601J444 (NoEOBD 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601J449 (Japan 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601J464 (Low Compression 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601J469 (US 6MT heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601JD34 (EU3 SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601JD39 (US SMG non-heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601JD54 (NoEOBD SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601JD59 (Japan SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601JD74 (EU3 Low Compression SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001601JD79 (US SMG heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801J424 (EU3 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801J444 (NoEOBD 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801J449 (Japan 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801J464 (Low Compression 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801J469 (US 6MT heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801J489.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801JD34 (EU3 SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801JD54 (NoEOBD SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801JD59 (Japan SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801JD74 (EU3 Low Compression SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801JD79 (US SMG heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323001801JD99 (US SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001J424 (EU3 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001J444 (NoEOBD 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001J449 (Japan 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001J464 (Low Compression 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001J469 (US 6MT heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001J484 (EU4 6MT).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001JD34 (EU3 SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001JD54 (NoEOBD SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001JD59 (Japan SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001JD74 (EU3 Low Compression SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002001JD94 (EU4 SMG).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002501J469 (US 6MT heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002501JD39 (US SMG non-heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002501JD79 (US SMG heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002701J429 (US 6MT non-heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002701J469 (US 6MT heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002701JD39 (US SMG non-heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `211323002701JD79 (US SMG heated DMTL).bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |

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
