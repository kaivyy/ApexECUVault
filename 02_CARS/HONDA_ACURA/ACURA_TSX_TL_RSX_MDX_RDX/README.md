# ACURA TSX TL RSX MDX RDX - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/ACURA_TSX_TL_RSX_MDX_RDX`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `58 files` (0 binary dumps, 58 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ACURA_TSX_TL_RSX_MDX_RDX` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `37805-5YF-A430_Acura_RDX_2020_SH-AWD_2.0L_L4_-_Gas.xdf` | `.XDF` | `52,363` bytes | Honda Keihin Factory Calibration Package `37805-5YF-A430` |
| `37805-5YF-A880_Acura_RDX_2019_SH-AWD_2.0L_L4_-_Gas.xdf` | `.XDF` | `52,363` bytes | Honda Keihin Factory Calibration Package `37805-5YF-A880` |
| `37805-PND-4160_Acura_RSX_2006_Base_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | Honda Keihin Factory Calibration Package `37805-PND-4160` |
| `37805-PND-4250_Acura_RSX_2005_Base_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | Honda Keihin Factory Calibration Package `37805-PND-4250` |
| `37805-PND-A090_Acura_RSX_2005_Base_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | Honda Keihin Factory Calibration Package `37805-PND-A090` |
| `37805-PND-A590_Acura_RSX_2004_Base_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | Honda Keihin Factory Calibration Package `37805-PND-A590` |
| `37805-PND-A660_Acura_RSX_2004_Base_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | Honda Keihin Factory Calibration Package `37805-PND-A660` |
| `37805-PNF-3050_Acura_RSX_2006_Base_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | Honda Keihin Factory Calibration Package `37805-PNF-3050` |
| `37805-PRB-3060_Acura_RSX_2002_2003_Type-S_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,597` bytes | Honda Keihin Factory Calibration Package `37805-PRB-3060` |
| `37805-PRB-4250_Acura_RSX_2006_Type-S_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,592` bytes | Honda Keihin Factory Calibration Package `37805-PRB-4250` |
| `37805-PVJ-3050_Acura_RSX_2004_Type-S_2.0L__L4_-_Gas.xdf` | `.XDF` | `1,592` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-3050` |
| `37805-R8A-A660_Acura_RDX_2013_2014_2015_Base_3.5L__V6_-_Gas___ECU_Acura_RDX.xdf` | `.XDF` | `7,396` bytes | Honda Keihin Factory Calibration Package `37805-R8A-A660` |
| `37805-R8A-X540_Acura_RDX_2013_2014_2015_Base_3.5L__V6_-_Gas.xdf` | `.XDF` | `7,246` bytes | Honda Keihin Factory Calibration Package `37805-R8A-X540` |
| `37805-RBB-A210_Acura_TSX_2007_2008_Base_2.4L_L4_-_Gas.xdf` | `.XDF` | `111,515` bytes | Honda Keihin Factory Calibration Package `37805-RBB-A210` |
| `37805-RBB-A710_Acura_TSX_2007_2008_Base_2.4L_L4_-_Gas.xdf` | `.XDF` | `110,905` bytes | Honda Keihin Factory Calibration Package `37805-RBB-A710` |
| `37805-RBJ-3090_Acura_TSX_2006_Base_2.4L__L4_-_Gas.xdf` | `.XDF` | `7,234` bytes | Honda Keihin Factory Calibration Package `37805-RBJ-3090` |
| `37805-RDA-A120_Acura_TL_2004_Base_3.2L__V6_-_Gas.xdf` | `.XDF` | `4,465` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A120` |
| `37805-RDA-A240_Acura_TL_2005_Base_3.2L__V6_-_Gas.xdf` | `.XDF` | `4,465` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A240` |
| `37805-RDA-A570_Acura_TL_2006_Base_3.2L__V6_-_Gas.xdf` | `.XDF` | `4,465` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A570` |
| `37805-RDA-A620_Acura_TL_2004_Base_3.2L__V6_-_Gas.xdf` | `.XDF` | `4,465` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A620` |
| `37805-RDA-A730_Acura_TL_2005_Base_3.2L__V6_-_Gas.xdf` | `.XDF` | `4,465` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A730` |
| `37805-RDA-A850_Acura_TL_2006_Base_3.2L__V6_-_Gas.xdf` | `.XDF` | `9,518` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A850` |
| `37805-RDB-A040_Acura_TL_3.5_16v_SH7058_1Mb.xdf` | `.XDF` | `9,510` bytes | Honda Keihin Factory Calibration Package `37805-RDB-A040` |
| `37805-RDB-A120_Acura_TL_2007_Type-S_3.5L__V6_-_Gas.xdf` | `.XDF` | `9,520` bytes | Honda Keihin Factory Calibration Package `37805-RDB-A120` |
| `37805-RDB-A560_Acura_TL_2008_Type-S_3.5L__V6_-_Gas.xdf` | `.XDF` | `9,520` bytes | Honda Keihin Factory Calibration Package `37805-RDB-A560` |
| `37805-RJA-A840_Acura_RL_2006_2007_Base_3.5L__V6_-_Gas.xdf` | `.XDF` | `7,796` bytes | Honda Keihin Factory Calibration Package `37805-RJA-A840` |
| `37805-RJA-A930_Acura_RL_2005_Base_3.5L__V6_-_Gas.xdf` | `.XDF` | `7,791` bytes | Honda Keihin Factory Calibration Package `37805-RJA-A930` |
| `37805-RJA-X550_Acura_RL_2006_2007_Base_3.5L__V6_-_Gas.xdf` | `.XDF` | `7,796` bytes | Honda Keihin Factory Calibration Package `37805-RJA-X550` |
| `37805-RJE-A840_Honda_Ridgeline_2006_2007_RT__RTL__RTS__RTX_RT__RTL__RTS_3.5.xdf` | `.XDF` | `8,501` bytes | Honda Keihin Factory Calibration Package `37805-RJE-A840` |
| `37805-RJE-A960_Honda_Ridgeline_2009_2010_2011_RT__RTL__RTS_3.5L__V6_-_Gas.xdf` | `.XDF` | `7,822` bytes | Honda Keihin Factory Calibration Package `37805-RJE-A960` |
| `37805-RKG-A560_Acura_RL_3.5_16v_SH7058_1Mb.xdf` | `.XDF` | `9,510` bytes | Honda Keihin Factory Calibration Package `37805-RKG-A560` |
| `37805-RKG-A720_Acura_RL_2009_2010_Base_3.7L__V6_-_Gas.xdf` | `.XDF` | `7,802` bytes | Honda Keihin Factory Calibration Package `37805-RKG-A720` |
| `37805-RKG-U520_Acura_RL_2011_2012_Base_3.7L__V6_-_Gas.xdf` | `.XDF` | `9,523` bytes | Honda Keihin Factory Calibration Package `37805-RKG-U520` |
| `37805-RL5-A030_Acura_TSX_2009_2010_Base_2.4L_L4_-_Gas.xdf` | `.XDF` | `85,484` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A030` |
| `37805-RL5-A070_Acura_TSX_2.4_16v_SH7058_1Mb.xdf` | `.XDF` | `83,631` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A070` |
| `37805-RL5-A120_Acura_TSX_2011_2012_2013_2014_Special_Edition_Base_2.4L__L4_.xdf` | `.XDF` | `5,060` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A120` |
| `37805-RL5-A560_Acura_TSX_2009_2010_Base_2.4L__L4_-_Gas___ECU_Acura_TSX_2.4_.xdf` | `.XDF` | `83,130` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A560` |
| `37805-RL5-A710_Acura_TSX_2011_2012_2013_2014_Base__Special_Edition_Base_2.4.xdf` | `.XDF` | `85,519` bytes | Honda Keihin Factory Calibration Package `37805-RL5-A710` |
| `37805-RL5-X020_Acura_TSX_2009_2010_Base_2.4L__L4_-_Gas.xdf` | `.XDF` | `5,034` bytes | Honda Keihin Factory Calibration Package `37805-RL5-X020` |
| `37805-RL5-X520_37805-RL5-X520.xdf` | `.XDF` | `5,007` bytes | Honda Keihin Factory Calibration Package `37805-RL5-X520` |
| `37805-RL8-A520_37805-RL8-A520.xdf` | `.XDF` | `8,332` bytes | Honda Keihin Factory Calibration Package `37805-RL8-A520` |
| `37805-RL8-A730_Acura_TSX_2010_V6_3.5L__V6_-_Gas.xdf` | `.XDF` | `7,795` bytes | Honda Keihin Factory Calibration Package `37805-RL8-A730` |
| `37805-RL8-X520_Acura_TSX_2011_2012_2013_2014_V6_3.5L__V6_-_Gas.xdf` | `.XDF` | `8,367` bytes | Honda Keihin Factory Calibration Package `37805-RL8-X520` |
| `37805-RL8-X730_37805-RL8-X730.xdf` | `.XDF` | `7,775` bytes | Honda Keihin Factory Calibration Package `37805-RL8-X730` |
| `37805-RP6-A640_Acura_ZDX_2010_2011_Base_3.7L__V6_-_Gas.xdf` | `.XDF` | `7,803` bytes | Honda Keihin Factory Calibration Package `37805-RP6-A640` |
| `37805-RP6-A760_Acura_ZDX_2012_Base_3.7L__V6_-_Gas___ECU_Acura_ZDX_3.7_V6_30.xdf` | `.XDF` | `7,917` bytes | Honda Keihin Factory Calibration Package `37805-RP6-A760` |
| `37805-RP6-A840_Acura_ZDX_2010_2011_Base_3.7L__V6_-_Gas.xdf` | `.XDF` | `7,803` bytes | Honda Keihin Factory Calibration Package `37805-RP6-A840` |
| `37805-RP6-X560_Acura_ZDX_2012_Base_3.7L__V6_-_Gas.xdf` | `.XDF` | `7,798` bytes | Honda Keihin Factory Calibration Package `37805-RP6-X560` |
| `37805-RRB-A140_Acura_CSX_2.0_16v_SH7058_1Mb.xdf` | `.XDF` | `204,428` bytes | Honda Keihin Factory Calibration Package `37805-RRB-A140` |
| `37805-RWC-A570_Acura_RDX_2.3_16v_SH7058_1Mb.xdf` | `.XDF` | `83,994` bytes | Honda Keihin Factory Calibration Package `37805-RWC-A570` |
| `37805-RWC-A620_Acura_RDX_2007_2008_2009_Base_2.3L__L4_-_Gas___ECU_Acura_RDX.xdf` | `.XDF` | `80,537` bytes | Honda Keihin Factory Calibration Package `37805-RWC-A620` |
| `37805-RWC-A720_Acura_RDX_2010_2011_SH-AWD_2.3L__L4_-_Gas.xdf` | `.XDF` | `10,084` bytes | Honda Keihin Factory Calibration Package `37805-RWC-A720` |
| `37805-RWC-A810_Acura_RDX_2012_SH-AWD_2.3L_L4_-_Gas.xdf` | `.XDF` | `79,864` bytes | Honda Keihin Factory Calibration Package `37805-RWC-A810` |
| `37805-RYE-A590_Acura_MDX_2011_Base_3.7L__V6_-_Gas___ECU_Acura_MDX_3.7_V6_30.xdf` | `.XDF` | `8,533` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A590` |
| `37805-RYE-A630_Acura_MDX_2007_Base_3.7L__V6_-_Gas___ECU_Acura_MDX_3.7_V6_30.xdf` | `.XDF` | `8,458` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A630` |
| `37805-RYE-A750_Acura_MDX_2008_2009_Base_3.7L__V6_-_Gas.xdf` | `.XDF` | `7,803` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A750` |
| `37805-RYE-A850_Acura_MDX_2010_2011_Base_3.7L__V6_-_Gas.xdf` | `.XDF` | `7,803` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A850` |
| `37805-RYE-X580_Acura_MDX_2010_2011_Base_3.7L__V6_-_Gas.xdf` | `.XDF` | `8,359` bytes | Honda Keihin Factory Calibration Package `37805-RYE-X580` |

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
