# DEFINITIONS XDF - ECU Calibration Suite

**Repository Path**: `02_CARS/NISSAN_INFINITI/DEFINITIONS_XDF`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `190 files` (0 binary dumps, 190 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `DEFINITIONS_XDF` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `1KA6A.xml` | `.XML` | `762` bytes | RomRaider / EcuFlash XML Definition |
| `1KE6C.xml` | `.XML` | `763` bytes | RomRaider / EcuFlash XML Definition |
| `1KE9C.xml` | `.XML` | `763` bytes | RomRaider / EcuFlash XML Definition |
| `1KN0B.xml` | `.XML` | `762` bytes | RomRaider / EcuFlash XML Definition |
| `4ME6B.xml` | `.XML` | `762` bytes | RomRaider / EcuFlash XML Definition |
| `5W502.xml` | `.XML` | `631` bytes | RomRaider / EcuFlash XML Definition |
| `5Y005.xml` | `.XML` | `712` bytes | RomRaider / EcuFlash XML Definition |
| `5Y700.xml` | `.XML` | `714` bytes | RomRaider / EcuFlash XML Definition |
| `5Y701.xml` | `.XML` | `420` bytes | RomRaider / EcuFlash XML Definition |
| `5Y702.xml` | `.XML` | `398` bytes | RomRaider / EcuFlash XML Definition |
| `5Y703.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `5Y711.xml` | `.XML` | `493` bytes | RomRaider / EcuFlash XML Definition |
| `5Y712.xml` | `.XML` | `421` bytes | RomRaider / EcuFlash XML Definition |
| `5Y713.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `5Y724.xml` | `.XML` | `8,081` bytes | RomRaider / EcuFlash XML Definition |
| `6W505.xml` | `.XML` | `3,768` bytes | RomRaider / EcuFlash XML Definition |
| `6W570.xml` | `.XML` | `714` bytes | RomRaider / EcuFlash XML Definition |
| `6Y300.xml` | `.XML` | `791` bytes | RomRaider / EcuFlash XML Definition |
| `6Y303.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `6Y310.xml` | `.XML` | `710` bytes | RomRaider / EcuFlash XML Definition |
| `6Y314.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `6Y321.xml` | `.XML` | `598` bytes | RomRaider / EcuFlash XML Definition |
| `6Y324.xml` | `.XML` | `4,768` bytes | RomRaider / EcuFlash XML Definition |
| `6Z55A.xml` | `.XML` | `7,790` bytes | RomRaider / EcuFlash XML Definition |
| `6Z68A.xml` | `.XML` | `796` bytes | RomRaider / EcuFlash XML Definition |
| `7S875.xml` | `.XML` | `7,955` bytes | RomRaider / EcuFlash XML Definition |
| `7Y001.xml` | `.XML` | `711` bytes | RomRaider / EcuFlash XML Definition |
| `7Y006.xml` | `.XML` | `396` bytes | RomRaider / EcuFlash XML Definition |
| `7Y210.xml` | `.XML` | `3,218` bytes | RomRaider / EcuFlash XML Definition |
| `8J160.xml` | `.XML` | `367` bytes | RomRaider / EcuFlash XML Definition |
| `8J164.xml` | `.XML` | `7,261` bytes | RomRaider / EcuFlash XML Definition |
| `8U023.xml` | `.XML` | `397` bytes | RomRaider / EcuFlash XML Definition |
| `8U073.xml` | `.XML` | `397` bytes | RomRaider / EcuFlash XML Definition |
| `8U07A.xml` | `.XML` | `3,212` bytes | RomRaider / EcuFlash XML Definition |
| `8U07B.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `8U320.xml` | `.XML` | `707` bytes | RomRaider / EcuFlash XML Definition |
| `8U42D.xml` | `.XML` | `2,623` bytes | RomRaider / EcuFlash XML Definition |
| `8U50B.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `8U51B.xml` | `.XML` | `397` bytes | RomRaider / EcuFlash XML Definition |
| `8U523.xml` | `.XML` | `397` bytes | RomRaider / EcuFlash XML Definition |
| `8U52B.xml` | `.XML` | `4,804` bytes | RomRaider / EcuFlash XML Definition |
| `8U901.xml` | `.XML` | `394` bytes | RomRaider / EcuFlash XML Definition |
| `8U906.xml` | `.XML` | `3,923` bytes | RomRaider / EcuFlash XML Definition |
| `8U92A.xml` | `.XML` | `3,562` bytes | RomRaider / EcuFlash XML Definition |
| `8Y004.xml` | `.XML` | `715` bytes | RomRaider / EcuFlash XML Definition |
| `8Y106.xml` | `.XML` | `2,703` bytes | RomRaider / EcuFlash XML Definition |
| `9DA0D.xml` | `.XML` | `623` bytes | RomRaider / EcuFlash XML Definition |
| `9J003.xml` | `.XML` | `6,043` bytes | RomRaider / EcuFlash XML Definition |
| `9J074.xml` | `.XML` | `5,169` bytes | RomRaider / EcuFlash XML Definition |
| `9J081.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `9W400.xml` | `.XML` | `709` bytes | RomRaider / EcuFlash XML Definition |
| `9W73B.xml` | `.XML` | `627` bytes | RomRaider / EcuFlash XML Definition |
| `9W84A.xml` | `.XML` | `8,919` bytes | RomRaider / EcuFlash XML Definition |
| `9Y410.xml` | `.XML` | `709` bytes | RomRaider / EcuFlash XML Definition |
| `9Y412.xml` | `.XML` | `709` bytes | RomRaider / EcuFlash XML Definition |
| `9Y510.xml` | `.XML` | `714` bytes | RomRaider / EcuFlash XML Definition |
| `A2L.xml` | `.XML` | `138,148` bytes | RomRaider / EcuFlash XML Definition |
| `AC011.xml` | `.XML` | `8,288` bytes | RomRaider / EcuFlash XML Definition |
| `AC012.xml` | `.XML` | `8,558` bytes | RomRaider / EcuFlash XML Definition |
| `AC200.xml` | `.XML` | `470` bytes | RomRaider / EcuFlash XML Definition |
| `AC300.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `AC301.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `AC305.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `AC306.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `AC30A.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `AC31A.xml` | `.XML` | `9,488` bytes | RomRaider / EcuFlash XML Definition |
| `AC400.xml` | `.XML` | `388` bytes | RomRaider / EcuFlash XML Definition |
| `AC401.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `AC405.xml` | `.XML` | `388` bytes | RomRaider / EcuFlash XML Definition |
| `AC406.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `AC40A.xml` | `.XML` | `388` bytes | RomRaider / EcuFlash XML Definition |
| `AC510.xml` | `.XML` | `402` bytes | RomRaider / EcuFlash XML Definition |
| `AC610.xml` | `.XML` | `601` bytes | RomRaider / EcuFlash XML Definition |
| `AC700.xml` | `.XML` | `386` bytes | RomRaider / EcuFlash XML Definition |
| `AC705.xml` | `.XML` | `389` bytes | RomRaider / EcuFlash XML Definition |
| `AC810.xml` | `.XML` | `394` bytes | RomRaider / EcuFlash XML Definition |
| `AC81A.xml` | `.XML` | `9,584` bytes | RomRaider / EcuFlash XML Definition |
| `AL902.xml` | `.XML` | `711` bytes | RomRaider / EcuFlash XML Definition |
| `AM603.xml` | `.XML` | `8,190` bytes | RomRaider / EcuFlash XML Definition |
| `AM604.xml` | `.XML` | `7,933` bytes | RomRaider / EcuFlash XML Definition |
| `AM607.xml` | `.XML` | `395` bytes | RomRaider / EcuFlash XML Definition |
| `AM900.xml` | `.XML` | `393` bytes | RomRaider / EcuFlash XML Definition |
| `AM905.xml` | `.XML` | `6,280` bytes | RomRaider / EcuFlash XML Definition |
| `AM90A.xml` | `.XML` | `401` bytes | RomRaider / EcuFlash XML Definition |
| `AM91A.xml` | `.XML` | `3,261` bytes | RomRaider / EcuFlash XML Definition |
| `AQ001.xml` | `.XML` | `708` bytes | RomRaider / EcuFlash XML Definition |
| `AQ806.xml` | `.XML` | `798` bytes | RomRaider / EcuFlash XML Definition |
| `AQ860.xml` | `.XML` | `2,709` bytes | RomRaider / EcuFlash XML Definition |
| `AZ01A.xml` | `.XML` | `581` bytes | RomRaider / EcuFlash XML Definition |
| `CC00A.xml` | `.XML` | `715` bytes | RomRaider / EcuFlash XML Definition |
| `CC00B.xml` | `.XML` | `715` bytes | RomRaider / EcuFlash XML Definition |
| `CC020.xml` | `.XML` | `715` bytes | RomRaider / EcuFlash XML Definition |
| `CC02A.xml` | `.XML` | `715` bytes | RomRaider / EcuFlash XML Definition |
| `CC06A.xml` | `.XML` | `715` bytes | RomRaider / EcuFlash XML Definition |
| `CD000.xml` | `.XML` | `740` bytes | RomRaider / EcuFlash XML Definition |
| `CD001.xml` | `.XML` | `571` bytes | RomRaider / EcuFlash XML Definition |
| `CD002.xml` | `.XML` | `571` bytes | RomRaider / EcuFlash XML Definition |
| `CD003.xml` | `.XML` | `571` bytes | RomRaider / EcuFlash XML Definition |
| `CD006.xml` | `.XML` | `565` bytes | RomRaider / EcuFlash XML Definition |
| `CD007.xml` | `.XML` | `565` bytes | RomRaider / EcuFlash XML Definition |
| `CD008.xml` | `.XML` | `567` bytes | RomRaider / EcuFlash XML Definition |
| `CD100.xml` | `.XML` | `391` bytes | RomRaider / EcuFlash XML Definition |
| `CD101.xml` | `.XML` | `391` bytes | RomRaider / EcuFlash XML Definition |
| `CD102.xml` | `.XML` | `8,531` bytes | RomRaider / EcuFlash XML Definition |
| `CD405.xml` | `.XML` | `389` bytes | RomRaider / EcuFlash XML Definition |
| `CD406.xml` | `.XML` | `391` bytes | RomRaider / EcuFlash XML Definition |
| `CD415.xml` | `.XML` | `7,222` bytes | RomRaider / EcuFlash XML Definition |
| `CD416.xml` | `.XML` | `4,546` bytes | RomRaider / EcuFlash XML Definition |
| `CD515.xml` | `.XML` | `8,757` bytes | RomRaider / EcuFlash XML Definition |
| `CD700.xml` | `.XML` | `393` bytes | RomRaider / EcuFlash XML Definition |
| `CD800.xml` | `.XML` | `436` bytes | RomRaider / EcuFlash XML Definition |
| `CE405.xml` | `.XML` | `10,358` bytes | RomRaider / EcuFlash XML Definition |
| `CE406.xml` | `.XML` | `1,094` bytes | RomRaider / EcuFlash XML Definition |
| `CE805.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `CE806.xml` | `.XML` | `9,112` bytes | RomRaider / EcuFlash XML Definition |
| `CE810.xml` | `.XML` | `9,106` bytes | RomRaider / EcuFlash XML Definition |
| `CE811.xml` | `.XML` | `9,781` bytes | RomRaider / EcuFlash XML Definition |
| `CE860.xml` | `.XML` | `5,385` bytes | RomRaider / EcuFlash XML Definition |
| `CF000.xml` | `.XML` | `9,312` bytes | RomRaider / EcuFlash XML Definition |
| `CF010.xml` | `.XML` | `397` bytes | RomRaider / EcuFlash XML Definition |
| `CF020.xml` | `.XML` | `520` bytes | RomRaider / EcuFlash XML Definition |
| `CF065.xml` | `.XML` | `13,160` bytes | RomRaider / EcuFlash XML Definition |
| `CF115.xml` | `.XML` | `14,790` bytes | RomRaider / EcuFlash XML Definition |
| `CF170.xml` | `.XML` | `8,780` bytes | RomRaider / EcuFlash XML Definition |
| `CF40A.xml` | `.XML` | `617` bytes | RomRaider / EcuFlash XML Definition |
| `CF40C.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `CF40D.xml` | `.XML` | `13,004` bytes | RomRaider / EcuFlash XML Definition |
| `CF40E.xml` | `.XML` | `793` bytes | RomRaider / EcuFlash XML Definition |
| `CF41A.xml` | `.XML` | `613` bytes | RomRaider / EcuFlash XML Definition |
| `CF41B.xml` | `.XML` | `613` bytes | RomRaider / EcuFlash XML Definition |
| `CF41D.xml` | `.XML` | `613` bytes | RomRaider / EcuFlash XML Definition |
| `CF41E.xml` | `.XML` | `5,136` bytes | RomRaider / EcuFlash XML Definition |
| `CF42A.xml` | `.XML` | `394` bytes | RomRaider / EcuFlash XML Definition |
| `CF42C.xml` | `.XML` | `10,834` bytes | RomRaider / EcuFlash XML Definition |
| `CF43A.xml` | `.XML` | `569` bytes | RomRaider / EcuFlash XML Definition |
| `CF43D.xml` | `.XML` | `15,259` bytes | RomRaider / EcuFlash XML Definition |
| `CF44A.xml` | `.XML` | `402` bytes | RomRaider / EcuFlash XML Definition |
| `CF44B.xml` | `.XML` | `636` bytes | RomRaider / EcuFlash XML Definition |
| `CF44C.xml` | `.XML` | `636` bytes | RomRaider / EcuFlash XML Definition |
| `CF44D.xml` | `.XML` | `608` bytes | RomRaider / EcuFlash XML Definition |
| `CF48D.xml` | `.XML` | `17,805` bytes | RomRaider / EcuFlash XML Definition |
| `CF49A.xml` | `.XML` | `18,156` bytes | RomRaider / EcuFlash XML Definition |
| `CF50A.xml` | `.XML` | `687` bytes | RomRaider / EcuFlash XML Definition |
| `CF90A.xml` | `.XML` | `570` bytes | RomRaider / EcuFlash XML Definition |
| `CF92A.xml` | `.XML` | `10,588` bytes | RomRaider / EcuFlash XML Definition |
| `CL110.xml` | `.XML` | `9,476` bytes | RomRaider / EcuFlash XML Definition |
| `CL72A.xml` | `.XML` | `537` bytes | RomRaider / EcuFlash XML Definition |
| `CM30A.xml` | `.XML` | `392` bytes | RomRaider / EcuFlash XML Definition |
| `CM30B.xml` | `.XML` | `398` bytes | RomRaider / EcuFlash XML Definition |
| `CM30C.xml` | `.XML` | `670` bytes | RomRaider / EcuFlash XML Definition |
| `CM31C.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `CM32B.xml` | `.XML` | `394` bytes | RomRaider / EcuFlash XML Definition |
| `CM32C.xml` | `.XML` | `662` bytes | RomRaider / EcuFlash XML Definition |
| `CM37A.xml` | `.XML` | `396` bytes | RomRaider / EcuFlash XML Definition |
| `CM40A.xml` | `.XML` | `392` bytes | RomRaider / EcuFlash XML Definition |
| `CM40B.xml` | `.XML` | `392` bytes | RomRaider / EcuFlash XML Definition |
| `CM40C.xml` | `.XML` | `392` bytes | RomRaider / EcuFlash XML Definition |
| `CM41A.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `CM41B.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `CM41C.xml` | `.XML` | `390` bytes | RomRaider / EcuFlash XML Definition |
| `EC80A.xml` | `.XML` | `642` bytes | RomRaider / EcuFlash XML Definition |
| `EC82A.xml` | `.XML` | `720` bytes | RomRaider / EcuFlash XML Definition |
| `EC87A.xml` | `.XML` | `720` bytes | RomRaider / EcuFlash XML Definition |
| `EM62B.xml` | `.XML` | `769` bytes | RomRaider / EcuFlash XML Definition |
| `EM63A.xml` | `.XML` | `720` bytes | RomRaider / EcuFlash XML Definition |
| `EV13B.xml` | `.XML` | `389` bytes | RomRaider / EcuFlash XML Definition |
| `EV15A.xml` | `.XML` | `2,672` bytes | RomRaider / EcuFlash XML Definition |
| `EV16A.xml` | `.XML` | `393` bytes | RomRaider / EcuFlash XML Definition |
| `EV18A.xml` | `.XML` | `12,851` bytes | RomRaider / EcuFlash XML Definition |
| `EV19B.xml` | `.XML` | `828` bytes | RomRaider / EcuFlash XML Definition |
| `JK03A.xml` | `.XML` | `759` bytes | RomRaider / EcuFlash XML Definition |
| `M5113.xml` | `.XML` | `12,255` bytes | RomRaider / EcuFlash XML Definition |
| `ScalingData.xml` | `.XML` | `59,123` bytes | RomRaider / EcuFlash XML Definition |
| `ZB010.xml` | `.XML` | `791` bytes | RomRaider / EcuFlash XML Definition |
| `ZB070.xml` | `.XML` | `15,001` bytes | RomRaider / EcuFlash XML Definition |
| `ZB075.xml` | `.XML` | `537` bytes | RomRaider / EcuFlash XML Definition |
| `ZC060.xml` | `.XML` | `705` bytes | RomRaider / EcuFlash XML Definition |
| `ZC070.xml` | `.XML` | `618` bytes | RomRaider / EcuFlash XML Definition |
| `ZD85E.xml` | `.XML` | `716` bytes | RomRaider / EcuFlash XML Definition |
| `ZD89A.xml` | `.XML` | `397` bytes | RomRaider / EcuFlash XML Definition |
| `ZG59B.xml` | `.XML` | `12,831` bytes | RomRaider / EcuFlash XML Definition |
| `ZH98A.xml` | `.XML` | `392` bytes | RomRaider / EcuFlash XML Definition |
| `ZH98C.xml` | `.XML` | `392` bytes | RomRaider / EcuFlash XML Definition |
| `ZH99A.xml` | `.XML` | `391` bytes | RomRaider / EcuFlash XML Definition |
| `ZJ05B.xml` | `.XML` | `7,365` bytes | RomRaider / EcuFlash XML Definition |
| `ZK01B.xml` | `.XML` | `393` bytes | RomRaider / EcuFlash XML Definition |
| `ZK03A.xml` | `.XML` | `712` bytes | RomRaider / EcuFlash XML Definition |
| `ZR35B.xml` | `.XML` | `3,104` bytes | RomRaider / EcuFlash XML Definition |
| `ZX10B.xml` | `.XML` | `821` bytes | RomRaider / EcuFlash XML Definition |
| `ZY70A.xml` | `.XML` | `758` bytes | RomRaider / EcuFlash XML Definition |

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
