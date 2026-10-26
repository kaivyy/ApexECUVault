# BMW SIEMENS MS42 - Factory DME Calibration Suite

**Repository Path**: `02_CARS/BMW/SIEMENS_MS42`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `18 files` (16 binary dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Koleksi lengkap 16 berkas biner factory firmware asli (512KB uncompressed) untuk DME Siemens MS42 software version 0110C6. Digunakan luas pada lini mesin BMW M52TUB20, M52TUB24, M52TUB25, dan M52TUB28 Dual-VANOS lintas platform E46 3-Series (320i, 323i, 328i), E39 5-Series (520i, 523i, 528i), E38 7-Series (728i), dan E36/7 Z3 Roadster. Dilengkapi dengan TunerPro XDF 32KB partial & 512KB full flash definitions.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Siemens MS42 (Digital Motor Electronics)`
- **Arsitektur MCU & Memori**: `Siemens / Infineon C167CR / 29F400 512KB External Flash`
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
| `Siemens_MS42_0110C6_E36Z3_M52TUB20_EU3.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E36Z3_M52TUB28_EU3_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E36Z3_M52TUB28_EU3_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E38_M52TUB28_EU3.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E39_M52TUB20_EU3.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E39_M52TUB25_EU3_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E39_M52TUB25_EU3_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E39_M52TUB28_EU3_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E39_M52TUB28_EU3_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E46_M52TUB20_EU2_CATV.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E46_M52TUB20_EU3.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E46_M52TUB24_THAI_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E46_M52TUB25_EU3_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E46_M52TUB25_EU3_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E46_M52TUB28_EU3_LHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_E46_M52TUB28_EU3_RHD.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Siemens_MS42_0110C6_ENG_32K_v1.3.xdf` | `.XDF` | `2,321,565` bytes | ECU Parameter Definition Map (XDF) |
| `Siemens_MS42_0110C6_ENG_512K_v1.3.xdf` | `.XDF` | `2,321,571` bytes | ECU Parameter Definition Map (XDF) |

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
