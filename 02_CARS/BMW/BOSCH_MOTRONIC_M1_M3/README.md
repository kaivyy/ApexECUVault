# BOSCH MOTRONIC M1 M3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/BOSCH_MOTRONIC_M1_M3`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `52 files` (25 binary dumps, 27 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `BOSCH_MOTRONIC_M1_M3` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `0261200402_1267358599_silver.bin` | `.BIN` | `32,768` bytes | Bosch Motronic Hardware ID `0261200402` |
| `0261200404-1267357689.bin` | `.BIN` | `65,536` bytes | Bosch Motronic Hardware ID `0261200404` |
| `059_dme_BMW.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `153stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `318i_175_soft1267356378.bin` | `.BIN` | `32,768` bytes | Bosch Calibration Software ID `1267356378` |
| `318i_ecu990_soft070.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `403NV.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `413 Silver Label 1995.bin` | `.BIN` | `65,536` bytes | Binary Firmware / Calibration Dump |
| `745i_64K_bin_013DME.bin` | `.BIN` | `8,192` bytes | Binary Firmware / Calibration Dump |
| `745i_64K_modded_boost_013DME.bin` | `.BIN` | `8,192` bytes | Binary Firmware / Calibration Dump |
| `745i_singleCHIP_64K.xdf` | `.XDF` | `33,850` bytes | TunerPro Binary Definition Map |
| `750iL_156.xdf` | `.XDF` | `23,664` bytes | TunerPro Binary Definition Map |
| `BMW173Chip.xdf` | `.XDF` | `53,999` bytes | TunerPro Binary Definition Map |
| `BMW173HakenTTBiggerMapsV11.xdf` | `.XDF` | `31,705` bytes | TunerPro Binary Definition Map |
| `BMW173Hakentt_bigger_mapsv11.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `BMW87_E30_153dme.xdf` | `.XDF` | `46,849` bytes | TunerPro Binary Definition Map |
| `BMW94_413redlabel_1267357623.bin` | `.BIN` | `65,536` bytes | Bosch Calibration Software ID `1267357623` |
| `BMW_0261200153_1267355367.bin` | `.BIN` | `32,768` bytes | Bosch Motronic Hardware ID `0261200153` |
| `BMW_027_DME_E30_4K.xdf` | `.XDF` | `15,111` bytes | TunerPro Binary Definition Map |
| `BMW_059_DME_M30_4KChip.xdf` | `.XDF` | `21,628` bytes | TunerPro Binary Definition Map |
| `BMW_175_318i_soft378.xdf` | `.XDF` | `47,199` bytes | TunerPro Binary Definition Map |
| `BMW_179.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `BMW_405_1740352_1267357951.bin` | `.BIN` | `65,536` bytes | Bosch Calibration Software ID `1267357951` |
| `BMW_850i_ecu352_soft566.xdf` | `.XDF` | `32,085` bytes | TunerPro Binary Definition Map |
| `BMW_990_318i_soft070.xdf` | `.XDF` | `35,684` bytes | TunerPro Binary Definition Map |
| `BMW_DME_179.xdf` | `.XDF` | `28,741` bytes | TunerPro Binary Definition Map |
| `BMW_E30_081.bin` | `.BIN` | `8,192` bytes | Binary Firmware / Calibration Dump |
| `BMW_E30_081.xdf` | `.XDF` | `19,062` bytes | TunerPro Binary Definition Map |
| `BMW_M3_506_soft965.xdf` | `.XDF` | `46,786` bytes | TunerPro Binary Definition Map |
| `BMW_S14_E30_M3_dme071.xdf` | `.XDF` | `21,968` bytes | TunerPro Binary Definition Map |
| `BMW_dme405_soft951.xdf` | `.XDF` | `25,106` bytes | TunerPro Binary Definition Map |
| `BMW_dme_404.xdf` | `.XDF` | `11,584` bytes | TunerPro Binary Definition Map |
| `BMW_ecu402_soft599.xdf` | `.XDF` | `16,178` bytes | TunerPro Binary Definition Map |
| `BMW_ecu403_soft.950.xdf` | `.XDF` | `15,463` bytes | TunerPro Binary Definition Map |
| `BMWdme282Chip626.xdf` | `.XDF` | `31,362` bytes | TunerPro Binary Definition Map |
| `Bmw 850i 5.0i 300HP 0261200352 356566.bin` | `.BIN` | `32,768` bytes | Bosch Motronic Hardware ID `0261200352` |
| `Bmw M-3 (USA) 0261203506-1267357965 (6fbb).bin` | `.BIN` | `65,536` bytes | Bosch Motronic Hardware ID `0261203506` |
| `E36_EuroM3_dme075.xdf` | `.XDF` | `17,360` bytes | TunerPro Binary Definition Map |
| `M3-2300Original.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `M3-MSS50_1_5_WK9.xdf` | `.XDF` | `35,401` bytes | TunerPro Binary Definition Map |
| `M3E36DME075_soft081.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `M50_S50_DME413_silverLbl.xdf` | `.XDF` | `86,498` bytes | TunerPro Binary Definition Map |
| `MS430037_64kb_Final_Eng.xdf` | `.XDF` | `3,578,590` bytes | Siemens / Continental DME Calibration Data |
| `MS430055_64kb_Final_Eng.xdf` | `.XDF` | `3,578,590` bytes | Siemens / Continental DME Calibration Data |
| `MS430056_64kb_Final_Eng.xdf` | `.XDF` | `3,548,859` bytes | Siemens / Continental DME Calibration Data |
| `MS430056_Logger_EWSSignatur_CHK5off.bin` | `.BIN` | `524,288` bytes | Siemens / Continental DME Calibration Data |
| `MS430056_Logger_EWSSignatur_CHK5off_Partial.bin` | `.BIN` | `65,536` bytes | Siemens / Continental DME Calibration Data |
| `MS430066_64kb_Final_Eng.xdf` | `.XDF` | `3,578,594` bytes | Siemens / Continental DME Calibration Data |
| `MS430069_64kb_Final_Eng.xdf` | `.XDF` | `3,578,590` bytes | Siemens / Continental DME Calibration Data |
| `bmw_027.bin` | `.BIN` | `4,096` bytes | Binary Firmware / Calibration Dump |
| `mss54hp_7842981.bin` | `.BIN` | `65,536` bytes | Siemens / Continental DME Calibration Data |
| `stock173.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |

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
