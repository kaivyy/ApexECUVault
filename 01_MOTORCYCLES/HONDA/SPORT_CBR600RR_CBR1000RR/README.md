# HONDA CBR600RR & CBR1000RR FIREBLADE - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/SPORT_CBR600RR_CBR1000RR`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `98 files` (49 binary dumps, 49 definition maps)  

---

## 1. Technical Platform Overview

Koleksi komprehensif kalibrasi ECU OEM untuk lini supersport dan superbike Honda CBR600RR (PC37, PC40) dan CBR1000RR Fireblade (SC57, SC59, SC77, SC82). Meliputi pembacaan firmware flash biner asli pabrikan Keihin 256KB/1MB dan definisi TunerPro XDF untuk pemetaan bahan bakar PGM-FI, timing pengapian independen per silinder, kontrol katup knalpot (EXCV), dan kalibrasi pembatas putaran mesin (rev limiter).

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Keihin / Denso Multi-Cylinder Supersport ECM`
- **Arsitektur MCU & Memori**: `Renesas SH7058 / Motorola MC68HC16 / MPC500 series`
- **Protokol Diagnostik & Flashing**: `K-Line (ISO 14230 KWP2000) / HDS Proprietary / Bench Bootmode`

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
| `38770-MEE-612.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEE-622.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEE-F02.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-613.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-643.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-672.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-772.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-A21.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-A22.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-D01.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-D21.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-F21.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL-L22.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MEL.xdf` | `.XDF` | `105,258` bytes | ECU Parameter Definition Map (XDF) |
| `38770-MFJ-A02.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFJ-D04.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFJ-F03.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-622.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-631.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-644.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-671.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-691.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-702.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-741.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-761.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-773.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-861.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-871.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-A21.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-D21.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-F21.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-J21.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-J41.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MFL-L21.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MGM-D11.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MGP-A01.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MGP-A92.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MGP-D01.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MGP-D62.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MGP-F01.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MGP-F63.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MGP-L01.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MJC-A01.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MJC-D01.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MKF-D43.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MKF-D72.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MKF-L13.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-MKF-TK2.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-N1A-D11.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `38770-NL3-750.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `CBR1000RR_2012_US.xdf` | `.XDF` | `63,564` bytes | ECU Parameter Definition Map (XDF) |
| `GENERATIONAL_38770-MKR-D12_Honda_CBR1000RR_R_Fireblade_SP_SC82_2020_2026_217.5PS.xdf` | `.XDF` | `1,830` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MEE-612_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MEE-613_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MEE-622_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MEE-A02_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MEE-D01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MEE-F02_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MFJ-D04_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MFJ-D42_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MFJ-F03_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MGZ-A03_CBR500R___CB500F___CB500X_(2013-2015).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MGZ-C02_CBR500R___CB500F___CB500X_(2013-2015).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MGZ-C03_CBR500R___CB500F___CB500X_(2013-2015).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MGZ-D02_CBR500R___CB500F___CB500X_(2013-2015).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MGZ-U02_CBR500R___CB500F___CB500X_(2013-2015).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJC-A01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJC-D01_Honda_Generic_ECM.xdf` | `.XDF` | `16,692` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-A02_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-BB1_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-D41_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-G12_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-G52_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-HB3_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-S11_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-T15_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-T52_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-TB1_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJE-VB1_CBR650F___CB650F_(2014-2018).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-961_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-AQ1_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-B41_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-D51_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-D91_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-DR1_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-N11_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-N41_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-NM1_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-T11_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MJW-_CBR500R___CB500F___CB500X_(2016-2018).xdf` | `.XDF` | `16,712` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MKN-D11_CBR650R___CB650R_(2019-2024).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MKN-D51_CBR650R___CB650R_(2019-2024).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MKN-DB1_CBR650R___CB650R_(2019-2024).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MKN-HB2_CBR650R___CB650R_(2019-2024).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MKN-HF2_CBR650R___CB650R_(2019-2024).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MKN-L32_CBR650R___CB650R_(2019-2024).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MKN-T11_CBR650R___CB650R_(2019-2024).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |
| `HONDA_38770-MKN-U11_CBR650R___CB650R_(2019-2024).xdf` | `.XDF` | `16,703` bytes | ECU Parameter Definition Map (XDF) |

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
