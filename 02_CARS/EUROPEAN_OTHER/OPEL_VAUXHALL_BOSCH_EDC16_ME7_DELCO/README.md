# OPEL & VAUXHALL - Bosch EDC16, Motronic ME7.6 & Delco Multec Suite

**Repository Path**: `02_CARS/EUROPEAN_OTHER/OPEL_VAUXHALL_BOSCH_EDC16_ME7_DELCO`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `116 files` (116 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Koleksi 116 berkas biner hardware dumps (.ori/.bin) untuk kendaraan Opel dan Vauxhall (Astra G/H, Corsa C/D, Vectra B/C, Zafira A/B, Meriva, Insignia, Frontera) dengan mesin 1.3 CDTI, 1.7 CDTI/DTI, 1.9 CDTI, 2.0 DTI, serta varian bensin 1.6/1.8/2.0 Turbo (Z20LET/LEH). Pengontrol Bosch EDC16C39 pada Opel 1.9 CDTI (Z19DTH) adalah varian platform bersama General Motors yang identik dengan arsitektur ECU Fiat JTDm dan Saab TiD.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Bosch EDC15M, EDC16C9, EDC16C39, Motronic ME7.6.2, Siemens Simtec, Delco Multec`
- **Arsitektur MCU & Memori**: `Infineon ST10 / Motorola MPC555 / MPC562 / MPC564 512KB-2MB Flash`
- **Protokol Diagnostik & Flashing**: `K-Line (ISO 14230 KWP2000) / CAN-Bus (GMLAN / ISO 15765) / BDM100`

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
| `0-281-001-793_Opel_Frontera_22DTi_HHH.16B.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `0-281-010-026_Opel_Frontera_22DTi.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0-281-010-448_Opel_Frontera_2.2DTi.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `001632h.ori.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `001632l.ori.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `0281001214 2537355342 .Ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001214 2537355394 .Ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001634 051 LLL.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001634 052 HHH.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281010267- B585300016ABB HHH.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281010267- B585300016ABB LLL.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281013409_1037A50286_Vectra_CDTI_120PS.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `1.7 CDTI 0281011380-1037370433.ORI` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.7 CDTI 0281011380-1037374424.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.7 CDTI 0281011943-1037372298.BIN` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `1.7 CDTI 0281011943-1037374425.ORI` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.7 CDTI 0281012694-1037376412.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281011448-1037370816.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281011449-1037372385.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281011449-1037379356.ORI` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281011667-1037379413.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281011914-1037371351.ORI` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281011914-1037372745.ORI` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281011914-1037379357.ORI` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281011915-1037372742.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1.9 CDTI 0281012533-1037379019.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `90569370.bin` | `.BIN` | `114,688` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `ASTRA CDTI 1,9-0281012122-1037371870.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Astra 1.9 CDTI 150HP 0281011667 371868.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Astra 2.0 16V GSi 0261200487 357099.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Bosch_EDC16_OPEL_0281012549_1037379426.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Cosa D_0261208940_1037381910 ori.bin` | `.BIN` | `851,968` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `DTI-SHH.873.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `DTI-SLL.873.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `F22-SHH.023.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `F22-SLL.023.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `OPEL 1.9 CDTI EDC16+ 0281013567-1037380490.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `OPEL ASTRA 1.9 CDTI 0281013409-1037383690.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `OPEL ASTRA 1.9 CDTI 0281014025-383480.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `OPEL ASTRA 1.9 CDTI-0281013409-1037379432.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `OPEL ASTRA CDTI 1,9-0281012548-379085.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Opel 1.9 CDTi 150bhp - 0281014451 - 1037387386.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel 1.9CDTI 0281012548 378432.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel 1.9CDTI 150HP 0281011915 379081.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel Astra 2.0 16v (C20XE) 0261203017 357369.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel Astra-G 1.6 16V 75HP 16227049 D98003 CNHR.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel Frontera 2.2DTI_0281010023 VU2M2S30.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel Monvano 2.5DCI  0281011432 368929.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel Vectra 1.9CDTI 150HP 0281013408 379428.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel Vectra B 1.8i 115HP 5WK9073 GM90506365.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel Vivaro 2.5 CDTI 2006 - 370878.zip.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Opel Vivaro 2.5CDTI 145HP 386228.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel Zafira  1.9CDTI 120HP 0281012549 1037A50292.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 1.7CDTI 0281011943 382477.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 1.7CDTI 90HP 0281010859 367182.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 1.7DTI 75HP DCWB Delco.ori` | `.ORI` | `212,992` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 1.7DTI 75HP DHCR - delco.ori` | `.ORI` | `212,992` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 1.7DTI 75HP DMRW Delco.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 1.7DTI 75HP DYRX  Delco.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 1.9 CDTI 150HP 0281012867 380280.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 2.0 16V 0261200487 356590.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 2.0DTI 100HP 0281001869 vtomw060.ori` | `.ORI` | `196,608` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 2.0DTI 100HP 0281001874.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra 2.0T 193HP 0261206332 354961.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra G 1.7CDTI 80HP 0281010859 367182.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra H 1.7CDTI 80HP 0281011943 372298.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra H 1.9CDTI 120HP 0281012123 372342.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra H 1.9CDTI 120HP 0281014025 383480.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra H 1.9CDTI 150HP 0281011668 1037372341.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel astra coupe 2.0T 193HP 0261206332 360526.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel calibra 2.0T 204HP 0261203014 357220.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel calibra 2.5 V6 170HP 0261203080 358003.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel combo 1.7DT 100HP Z17DTH.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel corsa 1.0 12V 0261204058 (EAE6).ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel corsa 1.2i 16V 0261207960 363893.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel corsa 1.2i 75HP 0261207962 370316.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel corsa 1.3CDTI 01246JO01D 1320X375.ori` | `.ORI` | `462,848` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel corsa 1.4 16v 16214239 JS D96017 BWJN.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel kadet 2.0 0261200186 356500.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel kadet 2.0 0261200372 356158.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel kadet 2.0 16V 0261200185 355631.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel kadett 2.0 16V 0261200185 355474.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel kadett GSI 2.0 16V 0261200185 356242.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel kadett GSI 2.0 16V 0261200185 356397.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel omega 2.2DTI 0281010274.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel omega 2.5TD 115HP 0281001215 2287358809.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel omega 2.5TD 130HP 0281001427 355007.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel omega 3.0 V6 205HP 0261203589 358933.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel signum 1.9CDTI 150HP 0281011449 1037370821.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel sintra 2.2DTI 0281001637.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 1.9CDTI  0281012534 383687.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 1.9CDTI 120HP 0281012534 377187.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 1.9CDTI 150HP 0281011448 372750.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 1.9CDTI 150HP 0281012869 384337 BDM.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 2.0DTI 0281001633 356489.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 2.0DTI 0281010269.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 2.0DTI 100HP 0281001871 CT 09136116.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 2.0DTI 100HP 0281010269.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra 2.2DTI 0281010271.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vectra B 2.0 16V 136HP 5WK9073 X20XEV.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel vivaro 2.0CDTI 114HP 386540.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel zafira 1.9CDTI 120HP 0281014452 387387.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel zafira 1.9CDTI 1540HP 0281014452 389374.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel zafira 2.0DTI 0281010021 VM0M1010.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel zafira 2.0DTI 0281010268.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel_Astra_D1700_R4V2T_55kW_0113386350_97240621_DLCC_9391249_crcAF2F28F6.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel_Astra_D1700_R4V4T_55kW_0113386350_97227225_DLNB_0939429_crcA432D8C9.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel_Frontera_D2200_R4V2T_85kW_0281010025_09173933_VU2M2W30_xxx_crc52CD7F87.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel_Zafira_B2000_R4V4T_141kW_0261207448_xxx_xxx_1037362726_crcE45766C9.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel_Zafira_R4V2_D2000_59kW_0281010268_96171442_HM7M4010_xxx_crc14d4a7c5.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Opel_Zafira_R4V2_D2000_59kW_0281010268_96171442_KM7M3020_xxx_crc8dbf7fef.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Vauxhall -Opel Astra G 1.7dti 97240621 EADLNF.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Vectra 1.9CDTI 120PS 0281014450 1037390674P48 ORI.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `eeprom.bin` | `.BIN` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `mpc555.bin` | `.BIN` | `462,848` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `z13dt.ori.bin` | `.BIN` | `458,752` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |

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
