# SUZUKI GSX-R1000 & GSX1300R HAYABUSA - Hyperbike ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/SUZUKI/BIG_BIKE_GSXR_HAYABUSA`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `19 files` (11 binary dumps, 8 definition maps)  

---

## 1. Technical Platform Overview

Pustaka kalibrasi resmi pabrikan Denso untuk Suzuki GSX-R1000 (M7 gen 2017+) dan Suzuki GSX1300R Hayabusa Gen 2 & Gen 3 (2021-2026). Mencakup firmware dump 2,097,152 bytes (2MB) untuk spesifikasi US, EU, dan Race, dipasangkan secara presisi dengan TunerPro XDF definitions untuk tuning throttle-by-wire (ETV), fuel injection primary/secondary, quickshifter/autoblipper, anti-lag (ALS), dan traction control strategies.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Denso / Mitsubishi 32-Bit Dual-Core Engine Control Module`
- **Arsitektur MCU & Memori**: `Renesas SH7058 / SH72543 / M32R 2MB Flash`
- **Protokol Diagnostik & Flashing**: `K-Line (SDS ISO 14230 KWP2000) / CAN-Bus (ISO 15765 UDS) / Bench Bootmode`

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
| `32990-10L1x - 5JCZSJ10.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `32990-48L00.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `32990-48L00.xdf` | `.XDF` | `3,817,943` bytes | ECU Parameter Definition Map (XDF) |
| `32990-48L10-US.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `32990-48L10-US.xdf` | `.XDF` | `3,830,183` bytes | ECU Parameter Definition Map (XDF) |
| `32990-48L20-EU.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `32990-48L20-EU.xdf` | `.XDF` | `3,830,586` bytes | ECU Parameter Definition Map (XDF) |
| `32990-48L30.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `32990-48L30.xdf` | `.XDF` | `3,818,152` bytes | ECU Parameter Definition Map (XDF) |
| `5JCUSJ40.ori` | `.ORI` | `2,031,679` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `5JCXSJ10.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `5JCZSJB0.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `5JCZSJB0.xdf` | `.XDF` | `3,727,292` bytes | ECU Parameter Definition Map (XDF) |
| `5JCZSNC0.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `5JCZSNC0.xdf` | `.XDF` | `3,723,868` bytes | ECU Parameter Definition Map (XDF) |
| `GENERATIONAL_32920-10L00_Suzuki_GSX1300R_Hayabusa_Gen_3_2021_2026.xdf` | `.XDF` | `2,543` bytes | ECU Parameter Definition Map (XDF) |
| `GENERATIONAL_32920-15H00_Suzuki_GSX1300R_Hayabusa_Gen_2_2008_2020.xdf` | `.XDF` | `2,543` bytes | ECU Parameter Definition Map (XDF) |
| `Hayabusa gen 3 stock.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `suzuki hayabusa 32990-10L4.ori` | `.ORI` | `2,031,679` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |

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
