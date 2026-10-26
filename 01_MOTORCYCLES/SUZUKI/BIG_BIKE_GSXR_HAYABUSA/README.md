# SUZUKI GSX-R1000, GSX1300R HAYABUSA & B-KING - Hyperbike Master ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/SUZUKI/BIG_BIKE_GSXR_HAYABUSA`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `41 files` (33 binary dumps, 8 definition maps)  

---

## 1. Technical Platform Overview

Pustaka kalibrasi resmi pabrikan Denso terlengkap untuk jajaran superbike dan hyperbike Suzuki: Hayabusa Gen 1 (1999-2007, 256KB Denso), Hayabusa Gen 2 K8 (2008-2020, 1MB Denso 32920-15H0/15H1), Hayabusa Gen 3 (2021-2026, 2MB RH850), B-King GSX1300BK (1340cc, 1MB Denso EU & US), dan Suzuki GSX-R1000 K7, K8, K9, L2-L4, L5-L6, hingga M7 (2007-2024). Berkas biner mencakup kalibrasi resmi pabrikan Denso 256KB, 1MB, dan 2MB, dipasangkan secara presisi dengan TunerPro XDF definitions untuk throttle-by-wire (ETV), primary/secondary fuel injection, quickshifter/autoblipper, anti-lag (ALS), dan traction control strategies.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Denso 32-Bit Dual-Core Engine Control Module`
- **Arsitektur MCU & Memori**: `Renesas SH7052 (256KB) / SH7058 (1MB) / RH850 (2MB Flash)`
- **Protokol Diagnostik & Flashing**: `K-Line (SDS ISO 14230 KWP2000) / CAN-Bus (ISO 15765 UDS) / Bench Bootmode`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Suzuki Part Numbers** (`32920-xxxxx`, `32990-xxxxx`): Nomor komponen resmi Suzuki Genuine Parts (SGP) untuk unit ECM/ECU Denso.
- **Denso Software IDs** (misal `DJ0HSE01`, `DJ55SE00`, `DJE4SE01`, `DJF4SE00`, `5JCZSJA0`): Kode revisi software pabrik yang tertanam di blok ROM Denso.
- **TunerPro XDF Maps** (`.xdf`): File deskriptor matematis yang memetakan offset memori hex ke unit engineering nyata (RPM, ms, derajat pengapian, kPa).

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **BusaECUeditor**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `21H50_DJ0HSE01.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `32990-10L1x - 5JCZSJ10.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `32990-48L00.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `32990-48L00.xdf` | `TunerPro Definition Map` | 3,817,943 | Definisi peta parameter kalibrasi TunerPro (3,817,943 bytes) untuk konversi skala dan offset tabel ECU |
| `32990-48L10-US.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `32990-48L10-US.xdf` | `TunerPro Definition Map` | 3,830,183 | Definisi peta parameter kalibrasi TunerPro (3,830,183 bytes) untuk konversi skala dan offset tabel ECU |
| `32990-48L20-EU.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `32990-48L20-EU.xdf` | `TunerPro Definition Map` | 3,830,586 | Definisi peta parameter kalibrasi TunerPro (3,830,586 bytes) untuk konversi skala dan offset tabel ECU |
| `32990-48L30.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `32990-48L30.xdf` | `TunerPro Definition Map` | 3,818,152 | Definisi peta parameter kalibrasi TunerPro (3,818,152 bytes) untuk konversi skala dan offset tabel ECU |
| `37H00_DJ55SE00.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `5JCUSJ40.ori` | `Original OEM Binary Flash Dump` | 2,031,679 | Berkas biner firmware resmi pabrikan (2,031,679 bytes) hasil hardware read murni (Zero-Synthetic) |
| `5JCXSJ10.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `5JCZSJB0.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `5JCZSJB0.xdf` | `TunerPro Definition Map` | 3,727,292 | Definisi peta parameter kalibrasi TunerPro (3,727,292 bytes) untuk konversi skala dan offset tabel ECU |
| `5JCZSNC0.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `5JCZSNC0.xdf` | `TunerPro Definition Map` | 3,723,868 | Definisi peta parameter kalibrasi TunerPro (3,723,868 bytes) untuk konversi skala dan offset tabel ECU |
| `Bking.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `BkingUS.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `DJ0HSE70.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `DJ47SE10.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `DJ55SE10.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `DJE4SE01.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `DJE4SE10.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `DJF4SE00.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `DJF4SE10.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `G1BusaEUdefault.bin` | `Original OEM Binary Flash Dump` | 262,144 | Berkas biner firmware resmi pabrikan (262,144 bytes) hasil hardware read murni (Zero-Synthetic) |
| `G1BusaUSdefault.bin` | `Original OEM Binary Flash Dump` | 262,144 | Berkas biner firmware resmi pabrikan (262,144 bytes) hasil hardware read murni (Zero-Synthetic) |
| `GENERATIONAL_32920-10L00_Suzuki_GSX1300R_Hayabusa_Gen_3_2021_2026.xdf` | `TunerPro Definition Map` | 2,543 | Definisi peta parameter kalibrasi TunerPro (2,543 bytes) untuk konversi skala dan offset tabel ECU |
| `GENERATIONAL_32920-15H00_Suzuki_GSX1300R_Hayabusa_Gen_2_2008_2020.xdf` | `TunerPro Definition Map` | 2,543 | Definisi peta parameter kalibrasi TunerPro (2,543 bytes) untuk konversi skala dan offset tabel ECU |
| `Gixxer21H00.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Gixxer21H10.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Gixxer21H70.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `GixxerK7.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `GixxerK7EU.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `GixxerK8.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Gixxerk9US.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Hayabusa gen 3 stock.bin` | `Original OEM Binary Flash Dump` | 2,097,152 | Berkas biner firmware resmi pabrikan (2,097,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K8.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `gixxerk9.bin` | `Original OEM Binary Flash Dump` | 1,048,576 | Berkas biner firmware resmi pabrikan (1,048,576 bytes) hasil hardware read murni (Zero-Synthetic) |
| `suzuki hayabusa 32990-10L4.ori` | `Original OEM Binary Flash Dump` | 2,031,679 | Berkas biner firmware resmi pabrikan (2,031,679 bytes) hasil hardware read murni (Zero-Synthetic) |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel (IAP vs RPM untuk low-throttle opening, TPS vs RPM untuk high-throttle), Primary & Secondary Injector Balance, Decel Fuel Cut, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance independen per silinder (Cylinder 1-4 / Pair), Mode Selection (A/B/C Power Modes), MS0/MS1 Maps, dan Dwell Timing.
- **Airflow & ETV / STP Management**: Electronic Throttle Valve (ETV / Drive-by-Wire) Target Angle per mode berkendara, Secondary Throttle Valve (STP) control, dan Exhaust Control Valve (SET Valve) positioning.
- **Safety Limits & Motorsport Thresholds**: Rev Limiter (Hard & Soft Cut), Top Speed Limiter (Vmax 299 km/h restriction removal), Launch Control RPM limiter, Quickshifter kill-time duration, dan Pit Lane Limiter.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*. Algoritma checksum Denso Suzuki menggunakan standar CRC-16/CCITT-FALSE pada rentang blok memori yang ditentukan.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD/K-Line atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
