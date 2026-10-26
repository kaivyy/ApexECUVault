# HYUNDAI N PERFORMANCE - Continental SIM2K-250 ECU Calibration Suite

**Repository Path**: `02_CARS/HYUNDAI_KIA/SIM2K_250_HYUNDAI_N_SERIES`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `18 files` (9 binary dumps, 9 definition maps)  

---

## 1. Technical Platform Overview

Koleksi 18 berkas kalibrasi asli (9 firmware binaries 2.62MB / 2.75MB + 9 TunerPro XDF definitions) untuk lini divisi Hyundai N Performance global: Hyundai i30N (PD/PDe), Hyundai Veloster N (JSN), Hyundai Elantra N / Avante N (CN7N), dan Hyundai Kona N (OSN) bermesin Theta II / Smartstream 2.0 T-GDI Turbo. Menampilkan pemetaan lengkap untuk boost target, wastegate duty cycle, direct injection rail pressure (HPP), multi-stage exhaust overrun pop & bang, variable intake cam phasing, dan rev matching.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Continental / Siemens SIM2K-250 (Kefico Powertrain Controller)`
- **Arsitektur MCU & Memori**: `Infineon Tricore SAK-TC1791 / TC1793 4MB Internal Flash`
- **Protokol Diagnostik & Flashing**: `UDS over CAN (ISO 14229 / ISO 15765 500kbps) / Bench BSL Bootmode`

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
| `CNNKKM___TAA.xdf` | `.XDF` | `2,435,181` bytes | ECU Parameter Definition Map (XDF) |
| `CNPNKM__FT5A.xdf` | `.XDF` | `9,522,614` bytes | ECU Parameter Definition Map (XDF) |
| `CNPNKM___T3A.xdf` | `.XDF` | `4,949,693` bytes | ECU Parameter Definition Map (XDF) |
| `CPQDDGMCXXXSDU50.xdf` | `.XDF` | `4,927,870` bytes | ECU Parameter Definition Map (XDF) |
| `CPQWDEMCXXXSDU50.xdf` | `.XDF` | `5,074,347` bytes | ECU Parameter Definition Map (XDF) |
| `CPQWDGMCXXXSDU50D.xdf` | `.XDF` | `5,048,473` bytes | ECU Parameter Definition Map (XDF) |
| `JSNNJMK__S2A.xdf` | `.XDF` | `2,812,840` bytes | ECU Parameter Definition Map (XDF) |
| `JSNNKMK__S2A.xdf` | `.XDF` | `2,812,840` bytes | ECU Parameter Definition Map (XDF) |
| `OSPNKM___T3A.xdf` | `.XDF` | `5,307,860` bytes | ECU Parameter Definition Map (XDF) |
| `Original [CNNKKM___TAA].bin` | `.BIN` | `2,621,440` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Original [CNPNKM__FT5A].bin` | `.BIN` | `2,621,440` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Original [CNPNKM___T3A].bin` | `.BIN` | `2,621,440` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Original [CPQDDGMCXXXSDU50].bin` | `.BIN` | `2,752,528` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Original [CPQWDEMCXXXSDU50].bin` | `.BIN` | `2,621,440` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Original [CPQWDGMCXXXSDU50D].bin` | `.BIN` | `2,621,440` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Original [JSNNJMK__S2A].bin` | `.BIN` | `2,621,440` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Original [JSNNKMK__S2A].bin` | `.BIN` | `2,621,440` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Original [OSPNKM___T3A].bin` | `.BIN` | `2,621,440` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |

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
