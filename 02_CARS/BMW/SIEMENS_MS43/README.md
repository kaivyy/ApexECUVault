# BMW SIEMENS MS43 - Factory DME Calibration Suite

**Repository Path**: `02_CARS/BMW/SIEMENS_MS43`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `35 files` (18 binary dumps, 17 definition maps)  

---

## 1. Technical Platform Overview

Koleksi 18 berkas biner factory firmware asli (512KB uncompressed) untuk DME Siemens MS43 versi perangkat lunak MS430069. Digunakan pada jajaran mesin BMW M54 (M54B22, M54B25, M54B30) dan M52TUB28 di platform BMW E46 3-Series (320i, 325i, 330i, Compact), E39 5-Series (525i, 530i), E53 X5 3.0i, dan E36/7 Z3 3.0i (spesifikasi EU2, EU4, LHD, RHD, dan US). Termasuk TunerPro XDF v1.16 standar dan ExtendedLoad.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Siemens MS43 (Digital Motor Electronics)`
- **Arsitektur MCU & Memori**: `Siemens / Infineon C167CR / AMD 29F400BB 512KB Flash`
- **Protokol Diagnostik & Flashing**: `BMW DS2 Diagnostic Protocol / K-Line (ISO 9141-2 / KWP2000) / OBD2`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`, `0110C6`, `MS430069`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`, `32920-xxxxx`): Nomor resmi Denso MCU firmware flash untuk mobil dan motor.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx-xxxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **VAG Hardware / Software IDs** (misal `038906012xx`, `03G906021xx`, `8D0907558xx`): Nomor bagian resmi Volkswagen Audi Group untuk identifikasi kalibrasi mesin EDC15, EDC16, dan ME7.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `MS43 ECU Definitions.xml` | `.XML` | `513,710` bytes | ECU Parameter Definition Map (XML) |
| `MS43 logger_METRIC_EN_v1.0.0 - ext load.xml` | `.XML` | `62,908` bytes | ECU Parameter Definition Map (XML) |
| `MS43 logger_METRIC_EN_v1.0.0.xml` | `.XML` | `64,814` bytes | ECU Parameter Definition Map (XML) |
| `Siemens_MS43_MS430037_ENG_512K_v1.16.xdf` | `.XDF` | `3,313,194` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430037_ENG_64K_v1.16.xdf` | `.XDF` | `3,313,188` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430055_ENG_512K_v1.16.xdf` | `.XDF` | `3,500,961` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430055_ENG_64K_v1.16.xdf` | `.XDF` | `3,500,955` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430056_ENG_512K_v1.16.xdf` | `.XDF` | `3,509,939` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430056_ENG_64K_v1.16.xdf` | `.XDF` | `3,509,933` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430064_ENG_512K_v1.16.xdf` | `.XDF` | `3,568,377` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430064_ENG_64K_v1.16.xdf` | `.XDF` | `3,568,371` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430066_ENG_512K_v1.16.xdf` | `.XDF` | `3,620,768` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430066_ENG_64K_v1.16.xdf` | `.XDF` | `3,620,762` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430069_E36Z3_M54B30_EU4_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E39_M54B25_EU4_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E39_M54B30_EU4_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E39_M54B30_US.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_Compact_M54B25_EU4_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M52TUB28_EU4_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B22_EU4_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B22_EU4_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B25_EU4_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B25_EU4_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B25_US.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B30_EU2_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B30_EU2_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B30_EU4_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B30_EU4_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E46_M54B30_US.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E53_M54B30_EU4.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_E53_M54B30_US.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS43_MS430069_ENG_512K_v1.16.xdf` | `.XDF` | `3,627,965` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430069_ENG_64K_v1.16.xdf` | `.XDF` | `3,627,959` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430069_ExtendedLoad_ENG_512K_v1.16.xdf` | `.XDF` | `3,627,837` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS43_MS430069_ExtendedLoad_ENG_64K_v1.16.xdf` | `.XDF` | `3,627,823` bytes | ECU Parameter Definition Map (XDF) |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro / RomRaider yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, Smoke Limiter, Torque-to-Fuel Limiter, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance, Low/High Octane Timing, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow & Boost Management**: Peta Target Boost Pressure, Wastegate Duty Cycle (WGDC / N75 Map), MAF/MAP Scaling, dan Throttle Response Curves (Driver Wish).
- **Safety Limits & Thresholds**: Rev Limiter (Hard/Soft Cut), Top Speed Limiter (Vmax), Overboost Fuel Cut, EGT (Exhaust Gas Temperature) Protection, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
