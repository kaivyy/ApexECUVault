# SUBARU 5EAT TRANSMISSION - Denso & Hitachi TCU Calibration Suite

**Repository Path**: `02_CARS/SUBARU/SUBARU_5EAT_TCU_DENSO_HITACHI`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `29 files` (26 binary dumps, 3 definition maps)  

---

## 1. Technical Platform Overview

Koleksi komprehensif 26 berkas biner ROM asli pabrikan dan 3 file definisi RomRaider XML untuk unit kendali transmisi otomatis 5EAT Subaru. Meliputi platform Subaru Legacy GT (BL/BP, BM/BR), Outback 3.0R / 2.5GT, Forester SH9 STI JDM, Impreza WRX STI A-Line (GRF/GVF), dan Subaru B9 Tribeca (WX). Mendukung tuning shift point timing, torque converter lockup (TCC) slip tables, line pressure profiling, dan manual paddle-shift response.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Denso & Hitachi 5EAT (5-Speed Electronic Automatic Transmission) Controller`
- **Arsitektur MCU & Memori**: `Hitachi M32R (M32176F4V) 384KB/512KB & Renesas SH7058S 1024KB (1MB)`
- **Protokol Diagnostik & Flashing**: `Subaru Select Monitor (SSM II / SSM III) / K-Line / CAN-Bus`

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
| `5AT_3.272_LEGAS_EJDM2008.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `5AT_3.583_LEGASE_JDM2008.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `5EAT_ADE0236000.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `5eat_tcu_denso_romraider_defs.xml` | `.XML` | `2,349,329` bytes | ECU Parameter Definition Map (XML) |
| `5eat_tcu_logger.xml` | `.XML` | `46,473` bytes | ECU Parameter Definition Map (XML) |
| `5eat_tcu_romraider_defs.xml` | `.XML` | `5,931,931` bytes | ECU Parameter Definition Map (XML) |
| `8AF0237300_MB500NJ0VF32C_2006_TRIBECA_USDM.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `8EFB206000_08FB2WA0_14_tribeca_usdm.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `91A0217300_MB4365.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `91A0217400_MB4372_A61022.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `91A1207300_MB4364.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `91D0207500_MB436T_AH572_5EAT_JDM.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `91D1206000_5EAT.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `91F0217100_MB436P_AG810_OBK03USDM.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `91FE207100_MB436L_AG802_5EAT_LGT05USDM.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `91FE216300.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `AAD1A06000.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `ABD1A03100_A61022_LGT_JDM_2005_5EAT.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `ACD1207000_MB558D01_LGT06_JDM.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `ACD1A06000_JDM_5EAT_2007_M32176F4V.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `B1AE207100_EZAE2WB1_2010_LGT_EDM.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Forester_SH9_STI_3.283_JDM2010.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Impreza_STI_3.583_JDM2011.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `SH7058S-3171121010_STI.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `SH7058S_TG5_3.083.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Tribeca_3.583_EDM_2009.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `[91D1207900-A61022]_31711AG589.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `[AAD1A07100-A61022]_31711AJ782.bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `[ABD1207000-A61022].bin` | `.BIN` | `393,216` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |

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
