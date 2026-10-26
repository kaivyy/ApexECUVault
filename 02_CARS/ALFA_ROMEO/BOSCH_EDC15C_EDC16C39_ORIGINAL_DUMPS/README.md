# ALFA ROMEO - Bosch EDC15C, EDC16C39 & ME7 Original Calibration Dumps

**Repository Path**: `02_CARS/ALFA_ROMEO/BOSCH_EDC15C_EDC16C39_ORIGINAL_DUMPS`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `106 files` (106 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Koleksi 106 berkas biner original hardware dumps (.ori/.bin) untuk kendaraan Alfa Romeo (145, 146, 147, 156, 159, 166, Brera, GT, Spider) dengan varian mesin 1.9 JTD/JTDM 8V/16V, 2.4 JTD/JTDM 10V/20V, 1.6/1.8/2.0 Twin Spark, dan 2.5/3.2 Busso V6. Unit ECU Bosch EDC16C39 pada Alfa Romeo secara teknis berbagi arsitektur firmware dan struktur peta kalibrasi yang identik dengan kendaraan Fiat, Opel (1.9 CDTI), Saab (1.9 TiD), dan Suzuki (1.9 DDiS).

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Bosch EDC15C, EDC15C-7, EDC16C8, EDC16C39, Motronic ME7.3.1, M1.5.5`
- **Arsitektur MCU & Memori**: `Infineon C167 / Motorola MPC555 / MPC562 / ST10F275 512KB-2MB Flash`
- **Protokol Diagnostik & Flashing**: `K-Line (ISO 9141 / KWP2000) / CAN-Bus (ISO 15765) / BDM100`

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
| `032-355_476.bin` | `.BIN` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `147original.txt.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `166 V6Turbo 706_349.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `166-24mjtd-1400055200785-0281010989-1037374160.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `ALFA 147 2000 16V 150CV 707_443.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `ALFA 156 1.9JTDM 140HP 0281011425 7372039.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `ALFA 156 2.4JTD 24C04 0281001863.bin` | `.BIN` | `512` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `ALFA 156 2.4JTD 29F400BT 0281001863.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `ALFA ROMEO 147 1.6 16V TS ME7.3.1  120HP  0261206715 1277356446.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `ALFA ROMEO 147 2.0 16V TS ME7.3.1  0261206708 1277356444.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `ALFA_75_B2000_R4V2_107kW_0261200108_1622411042_xxx_1267356191_crcE01C1F89.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 145 1.9JTD 105HP 0281001936 351190.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 145 1.9JTD 105HP 0281001936 354263.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 145 2.0TS 0261204478 358492.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 146 1.9JTD 105HP 0281001936 1037356777.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 115HP 0281010332 351962.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 115HP 0281010332 354624.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 115HP 0281010332 366536.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 115HP 0281010332 366688.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 115HP 0281011488 372060.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 115bhp 0281010332 1037366536.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 140HP 0281010455 367333.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 140HP 0281011429 372044.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 140HP 0281011511 370467.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 140HP 370596.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 150HP 0281011896 372047.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTD 150HP 0281012883 1037379006.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTDM 0281011429 370467.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTDM 0281012882 379005.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTDM 140HP 0281010455 367333.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTDM 140HP 0281011429 368421.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTDM 140HP 0281011429 372044.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 1.9JTDM 8V 120HP 0281012858 377779.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 GTA 3.2i 250HP 0261207967 367088.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 147 ducati 1.9JTDM 170HP 0281015228 395299.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 155 1.8TS 144HP 0261200536 357963.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 155 2.0TS 0261203862 355410.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 155 2.5TD 125HP 0281001191 358304.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 155 2.5TD 125HP 0281001191 358305.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.8TS 0261204947 350390.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.8i 144HP 0261204732 352977.ori` | `.ORI` | `122,396` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 0281010986 367332.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 0281011425 370469.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 105HP 0281001587 1037357648.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 105HP 0281001891 356733.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 105HP 0281010020 1037359785.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 105HP 0281010020 354262.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 105HP 0281010020 359785.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 110HP 0281010335 351965.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 110HP 0281010335 362436.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 115HP 0281010332 351962.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 115HP 0281010740 366796.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 115HP 0281011488 369116.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 1.9JTD 115HP 0281011491 372061.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.0 155HP 0261204270 359650.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTD 0281010022 359786.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTD 0281010988 372042.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTD 136HP 0281001661 1037358008.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTD 136HP 0281001890 356734.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTD 140HP 0281010336 1037362086.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTD 150HP 0281010336 354394.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTD 150HP 0281010741 363243.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTD 150HP 0281010741 366800.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.4JTDM 175HP 0281010988 369430.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 156 2.5i 0261206168 359733.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 159 1.9JTD 120HP 0281012888 378873.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 159 1.9JTDM 150 0281013138 380494.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 159 1.9JTDM 150HP 0281012144 377871.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 159 2.4JTDM 200HP 0281012146 392277.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 159 2.4JTDM 200HP 0281013417 383773.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 159 2.4JTDM 210HP 0281014459 390927.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 159 JTD_org- 389889.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Alfa 159 brera 2.4JTD 200HP 0281012145 377554.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 1.9JTD 110HP 0281010335 351517.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 1.9JTD 110HP 0281010335 362436.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 2.4JTD 136HP 0281001787 351423.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 2.4JTD 136HP 0281001787 352209.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 2.4JTD 136HP 0281001787 359736.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 2.4JTD 140HP 0281010340 363752.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 2.4JTD 150HP 0281010340 363752.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 2.4JTD 150HP 0281011503 371897.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 166 3.0i sportronic 0261204032 359706.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa 75 1.6 0261200124 356311.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa GT 1.9JTD 150HP 0281011511 372048.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa GT 1.9JTD 150HP 0281011511370466.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa GT 1.9JTD 150HP 0281012298 377778.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa GT 1.9JTDM 150HP 0281013533 386727.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa GTV 2.0 TS 0261206061.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa Romeo 147 2.0i 0261206708 356444.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa Romeo 156 1.6 TS 120HP 0261204772 357849.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa Romeo 156 1.9JTD 110HP 0281010740 363242.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa Romeo 156 2.4JTD 136HP 0281001588 358064.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa Romeo 159 2.2JTS 0261S01045 378597.ori` | `.ORI` | `917,504` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa Romeo GTV-Spider 1.8L TS 16v 144hp AR32201 0261206060 1037350387.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa romeo 155 2.5 V6 166HP 0261200537 356464.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa romeo 155 V6 166HP 0261200537 356596.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa romeo GT 1.9JTD 150HP 0281011511 372048.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa_166_D2400_R4V2T_110kW_0281010340_46759586_xxx_1037354395_crcDE404202.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa_166_D2400_R4V2T_110kW_0281010340_46821768_0074_1037362085_crcE52C811A.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa_166_D2400_R4V2T_110kW_0281010340_73501858_0092_1037363752_crcE73C2D85.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa_75_B2000_R4V2_107KW_0261200108_1622411042_xxx_1267356106_crc6880df39.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa_GT_bosch_0261208571_1037368772.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Alfa_Mito_78cv_1037398162.bin` | `.BIN` | `851,968` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `OkAlfa649B.947.BIN` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `alfa_007.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `alfaromeo_394001.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |

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
