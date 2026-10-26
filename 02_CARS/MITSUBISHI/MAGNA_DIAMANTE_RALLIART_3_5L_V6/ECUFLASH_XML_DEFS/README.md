# ECUFLASH XML DEFS - ECU Calibration Suite

**Repository Path**: `02_CARS/MITSUBISHI/MAGNA_DIAMANTE_RALLIART_3_5L_V6/ECUFLASH_XML_DEFS`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `31 files` (0 binary dumps, 31 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ECUFLASH_XML_DEFS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `22490005.xml` | `.XML` | `12,258` bytes | RomRaider / EcuFlash XML Definition |
| `22520004.xml` | `.XML` | `12,256` bytes | RomRaider / EcuFlash XML Definition |
| `22600000.xml` | `.XML` | `12,089` bytes | RomRaider / EcuFlash XML Definition |
| `22620000.xml` | `.XML` | `12,085` bytes | RomRaider / EcuFlash XML Definition |
| `23430000.xml` | `.XML` | `12,089` bytes | RomRaider / EcuFlash XML Definition |
| `80350003.xml` | `.XML` | `15,659` bytes | RomRaider / EcuFlash XML Definition |
| `81930003.xml` | `.XML` | `15,674` bytes | RomRaider / EcuFlash XML Definition |
| `82000001.xml` | `.XML` | `15,577` bytes | RomRaider / EcuFlash XML Definition |
| `82000002.xml` | `.XML` | `15,577` bytes | RomRaider / EcuFlash XML Definition |
| `82030001.xml` | `.XML` | `15,583` bytes | RomRaider / EcuFlash XML Definition |
| `82030002.xml` | `.XML` | `15,583` bytes | RomRaider / EcuFlash XML Definition |
| `82450006.xml` | `.XML` | `15,578` bytes | RomRaider / EcuFlash XML Definition |
| `83890006.xml` | `.XML` | `15,677` bytes | RomRaider / EcuFlash XML Definition |
| `85490000.xml` | `.XML` | `15,447` bytes | RomRaider / EcuFlash XML Definition |
| `85490001.xml` | `.XML` | `15,447` bytes | RomRaider / EcuFlash XML Definition |
| `87190003.xml` | `.XML` | `16,238` bytes | RomRaider / EcuFlash XML Definition |
| `87200002.xml` | `.XML` | `632` bytes | RomRaider / EcuFlash XML Definition |
| `87200004.xml` | `.XML` | `15,568` bytes | RomRaider / EcuFlash XML Definition |
| `87200005a.xml` | `.XML` | `15,591` bytes | RomRaider / EcuFlash XML Definition |
| `87200005b.xml` | `.XML` | `649` bytes | RomRaider / EcuFlash XML Definition |
| `87410004.xml` | `.XML` | `15,657` bytes | RomRaider / EcuFlash XML Definition |
| `91760000.xml` | `.XML` | `626` bytes | RomRaider / EcuFlash XML Definition |
| `91760002.xml` | `.XML` | `13,312` bytes | RomRaider / EcuFlash XML Definition |
| `91970002.xml` | `.XML` | `13,166` bytes | RomRaider / EcuFlash XML Definition |
| `97180003.xml` | `.XML` | `14,127` bytes | RomRaider / EcuFlash XML Definition |
| `97180004.xml` | `.XML` | `621` bytes | RomRaider / EcuFlash XML Definition |
| `97190002.xml` | `.XML` | `13,987` bytes | RomRaider / EcuFlash XML Definition |
| `98320000.xml` | `.XML` | `13,307` bytes | RomRaider / EcuFlash XML Definition |
| `98320001.xml` | `.XML` | `621` bytes | RomRaider / EcuFlash XML Definition |
| `magna_3g_at_base.xml` | `.XML` | `7,203` bytes | RomRaider / EcuFlash XML Definition |
| `magna_3g_base.xml` | `.XML` | `52,637` bytes | RomRaider / EcuFlash XML Definition |

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
