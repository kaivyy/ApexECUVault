# SUZUKI GSX-R600 & GSX-R750 - Supersport ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/SUZUKI/SUPERSPORT_GSXR600_GSXR750`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `5 files` (2 binary dumps, 3 definition maps)  

---

## 1. Technical Platform Overview

Koleksi komprehensif kalibrasi ECU OEM Denso untuk jajaran supersport Suzuki GSX-R600 dan GSX-R750 generasi K6 hingga L9 (2006-2020). Meliputi pembacaan firmware flash biner asli pabrikan Denso 1,048,576 bytes (1MB) seperti G750K9 (part number 32920-38H00) dan varian restriksi G750K9G, serta definisi TunerPro XDF untuk pemetaan IAP/TPS fuel injection, secondary throttle plates (STP), per-gear ignition timing, rev limiter (15,000 RPM GSX-R750 / 16,000 RPM GSX-R600), dan penyesuaian sensor O2/Pair valve.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Denso 32-Bit Engine Control Module`
- **Arsitektur MCU & Memori**: `Renesas SuperH SH7054 / SH7058 (512KB / 1024KB Flash)`
- **Protokol Diagnostik & Flashing**: `K-Line (SDS ISO 14230 KWP2000) / Bench Bootmode (AUD / JTAG)`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Suzuki Part Numbers** (`32920-xxxxx`, `32990-xxxxx`): Nomor komponen resmi Suzuki Genuine Parts (SGP) untuk unit ECM/ECU Denso.
- **Denso Software IDs** (misal `DJ0HSE01`, `DJ55SE00`, `DJE4SE01`, `DJF4SE00`, `5JCZSJA0`): Kode revisi software pabrik yang tertanam di blok ROM Denso.
- **TunerPro XDF Maps** (`.xdf`): File deskriptor matematis yang memetakan offset memori hex ke unit engineering nyata (RPM, ms, derajat pengapian, kPa).

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **BusaECUeditor**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2008–2010

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `G750K9.bin` | **2008–2010** | 1.00 MB | `16240ffff6d744307f3087c33d472172` | Factory Binary Firmware Dump |
| `G750K9G.bin` | **2008–2010** | 1.00 MB | `5bf7e3c900851a94288489bbd8eee696` | Factory Binary Firmware Dump |
| `GENERATIONAL_32920-01H00_Suzuki_GSX_R600_K6_K7_2006_2007_125PS.xdf` | **2006–2007** | 1.8 KB | `2d1e8330b5a02497dd6fd634ab1cc21d` | TunerPro Binary Definition Map |
| `GENERATIONAL_32920-14J00_Suzuki_GSX_R600_L1_L9_Showa_BPF_2011_2020_126PS.xdf` | **2011–2020** | 1.8 KB | `4eddf667010876f481b966a79fa9321d` | TunerPro Binary Definition Map |
| `GENERATIONAL_32920-14J50_Suzuki_GSX_R750_L1_L9_2011_2020_150PS.xdf` | **2011–2020** | 1.8 KB | `833eb20d7488a7cf87528d5baea75111` | TunerPro Binary Definition Map |

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
