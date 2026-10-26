# LANCER EVOLUTION TEPHRAMOD - ECU Calibration Suite

**Repository Path**: `02_CARS/MITSUBISHI/LANCER_EVOLUTION_TEPHRAMOD`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `142 files` (0 binary dumps, 142 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `LANCER_EVOLUTION_TEPHRAMOD` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `22580006 1998 JDM Lancer Evo 5 GSR.xml` | `.XML` | `15,742` bytes | RomRaider / EcuFlash XML Definition |
| `22580007 1998 JDM Lancer Evo 5 GSR.xml` | `.XML` | `17,488` bytes | RomRaider / EcuFlash XML Definition |
| `23490006 1998-1999 JDM Lancer Evo 5-6.xml` | `.XML` | `17,511` bytes | RomRaider / EcuFlash XML Definition |
| `23490007 1998 JDM Lanver Evo 5.xml` | `.XML` | `15,312` bytes | RomRaider / EcuFlash XML Definition |
| `24430002 1999 JDM Lancer Evo 6 RS.xml` | `.XML` | `17,819` bytes | RomRaider / EcuFlash XML Definition |
| `24440002 1999 JDM Lancer Evo 6 GSR.xml` | `.XML` | `17,451` bytes | RomRaider / EcuFlash XML Definition |
| `25570000 1998-1999 JDM Lanver Evo 5-6 Ralliart MT.xml` | `.XML` | `17,041` bytes | RomRaider / EcuFlash XML Definition |
| `25580000 1999 JDM Lancer Evo 6 RSII MT.xml` | `.XML` | `15,813` bytes | RomRaider / EcuFlash XML Definition |
| `25770000 1998-1999 JDM Lancer Evo 5-6.xml` | `.XML` | `18,281` bytes | RomRaider / EcuFlash XML Definition |
| `27370001 2000 JDM Lancer Evo TME GSR.xml` | `.XML` | `18,068` bytes | RomRaider / EcuFlash XML Definition |
| `27380001 2000 JDM Lancer Evo TME RS.xml` | `.XML` | `16,718` bytes | RomRaider / EcuFlash XML Definition |
| `50845084 2014 EDM Lancer Evolution X 5MT.xml` | `.XML` | `14,090` bytes | RomRaider / EcuFlash XML Definition |
| `52350012 2008 JDM Lancer Evolution X 5MT.xml` | `.XML` | `12,596` bytes | General Motors Operating System ID `52350012` |
| `52350018 2008 JDM Lancer Evolution X 5MT.xml` | `.XML` | `20,728` bytes | General Motors Operating System ID `52350018` |
| `52360016 2008 JDM Lancer Evolution X 5MT.xml` | `.XML` | `12,596` bytes | General Motors Operating System ID `52360016` |
| `52360018 2008 JDM Lancer Evolution X 5MT.xml` | `.XML` | `23,393` bytes | General Motors Operating System ID `52360018` |
| `52370023 2008 JDM Lancer Evolution X SST.xml` | `.XML` | `15,309` bytes | General Motors Operating System ID `52370023` |
| `52370024 2008 JDM Lancer Evolution X SST.xml` | `.XML` | `27,760` bytes | General Motors Operating System ID `52370024` |
| `52550003 2008 EDM Lancer Evolution X 5MT.xml` | `.XML` | `12,794` bytes | General Motors Operating System ID `52550003` |
| `52680015 2008 USDM Lancer Evolution X 5MT.xml` | `.XML` | `30,031` bytes | General Motors Operating System ID `52680015` |
| `52680016 2008 USDM Lancer Evolution X 5MT.xml` | `.XML` | `918` bytes | General Motors Operating System ID `52680016` |
| `52680017 2008 USDM Lancer Evolution X 5MT.xml` | `.XML` | `918` bytes | General Motors Operating System ID `52680017` |
| `52680018 2008 USDM Lancer Evolution X 5MT.xml` | `.XML` | `918` bytes | General Motors Operating System ID `52680018` |
| `52680019 2008 USDM Lancer Evolution X 5MT.xml` | `.XML` | `918` bytes | General Motors Operating System ID `52680019` |
| `52680020 2008 USDM Lancer Evolution X 5MT.xml` | `.XML` | `918` bytes | General Motors Operating System ID `52680020` |
| `52680022 2008 USDM Lancer Evolution X 5MT.xml` | `.XML` | `918` bytes | General Motors Operating System ID `52680022` |
| `52680024 2008 USDM Lancer Evolution X 5MT.xml` | `.XML` | `23,645` bytes | General Motors Operating System ID `52680024` |
| `52690019 2008 USDM Lancer Evolution X SST.xml` | `.XML` | `34,089` bytes | General Motors Operating System ID `52690019` |
| `52690021 2008 USDM Lancer Evolution X SST.xml` | `.XML` | `918` bytes | General Motors Operating System ID `52690021` |
| `52690022 2008 USDM Lancer Evolution X SST.xml` | `.XML` | `918` bytes | General Motors Operating System ID `52690022` |
| `52690024 2008 USDM Lancer Evolution X SST.xml` | `.XML` | `22,813` bytes | General Motors Operating System ID `52690024` |
| `53040007 2008 EDM Lancer Evolution X 5MT.xml` | `.XML` | `14,334` bytes | RomRaider / EcuFlash XML Definition |
| `53040008 2008 EDM Lancer Evolution X 5MT.xml` | `.XML` | `917` bytes | RomRaider / EcuFlash XML Definition |
| `53040010 2008 EDM Lancer Evolution X 5MT.xml` | `.XML` | `24,157` bytes | RomRaider / EcuFlash XML Definition |
| `53050006 2008 EDM Lancer Evolution X SST.xml` | `.XML` | `13,847` bytes | RomRaider / EcuFlash XML Definition |
| `53050007 2008 EDM Lancer Evolution X SST.xml` | `.XML` | `917` bytes | RomRaider / EcuFlash XML Definition |
| `53050009 2008 EDM Lancer Evolution X SST.xml` | `.XML` | `29,142` bytes | RomRaider / EcuFlash XML Definition |
| `53050011 2008 EDM Lancer Evolution X SST.xml` | `.XML` | `21,260` bytes | RomRaider / EcuFlash XML Definition |
| `53050012 2008 EDM Lancer Evolution X SST.xml` | `.XML` | `917` bytes | RomRaider / EcuFlash XML Definition |
| `53600008 2009 USDM Lancer Ralliart SST.xml` | `.XML` | `26,766` bytes | RomRaider / EcuFlash XML Definition |
| `53600009 2009 USDM Lancer Ralliart SST.xml` | `.XML` | `915` bytes | RomRaider / EcuFlash XML Definition |
| `53600010 2009 USDM Lancer Ralliart SST.xml` | `.XML` | `915` bytes | RomRaider / EcuFlash XML Definition |
| `53610009 2009 EDM Lancer Ralliart SST.xml` | `.XML` | `24,489` bytes | RomRaider / EcuFlash XML Definition |
| `53610010 2009 EDM Lancer Ralliart SST.xml` | `.XML` | `914` bytes | RomRaider / EcuFlash XML Definition |
| `53610012 2009 EDM Lancer Ralliart SST.xml` | `.XML` | `26,271` bytes | RomRaider / EcuFlash XML Definition |
| `53610013 2009 EDM Lancer Ralliart SST.xml` | `.XML` | `914` bytes | RomRaider / EcuFlash XML Definition |
| `54060007 2009 EDM Lancer Evolution X 5MT.xml` | `.XML` | `13,650` bytes | RomRaider / EcuFlash XML Definition |
| `54060008 2009 EDM Lancer Evolution X 5MT.xml` | `.XML` | `917` bytes | RomRaider / EcuFlash XML Definition |
| `54070006  2009 EDM Lancer Evolution X SST.xml` | `.XML` | `20,658` bytes | RomRaider / EcuFlash XML Definition |
| `54070007 2009 EDM Lancer Evolution X SST.xml` | `.XML` | `917` bytes | RomRaider / EcuFlash XML Definition |
| `54550003 2009 JDM Lancer Evolution X SST.xml` | `.XML` | `12,148` bytes | RomRaider / EcuFlash XML Definition |
| `54560003 2009 JDM Lancer Evolution X 5MT.xml` | `.XML` | `12,364` bytes | RomRaider / EcuFlash XML Definition |
| `55570005 2010 USDM Lancer Evolution X 5MT.xml` | `.XML` | `26,470` bytes | RomRaider / EcuFlash XML Definition |
| `55570006 2010 USDM Lancer Evolution X 5MT.xml` | `.XML` | `918` bytes | RomRaider / EcuFlash XML Definition |
| `55580005 2010 USDM Lancer Evolution X SST.xml` | `.XML` | `35,048` bytes | RomRaider / EcuFlash XML Definition |
| `55580006 2010 USDM Lancer Evolution X SST.xml` | `.XML` | `918` bytes | RomRaider / EcuFlash XML Definition |
| `55590006 2010 USDM Lancer Ralliart SST.xml` | `.XML` | `33,612` bytes | RomRaider / EcuFlash XML Definition |
| `55590007 2010 USDM Lancer Ralliart SST.xml` | `.XML` | `915` bytes | RomRaider / EcuFlash XML Definition |
| `56180001 2010 JDM Lancer Evolution X 5MT.xml` | `.XML` | `20,583` bytes | RomRaider / EcuFlash XML Definition |
| `56180002 2010 JDM Lancer Evolution X 5MT.xml` | `.XML` | `917` bytes | RomRaider / EcuFlash XML Definition |
| `56190002 2010 JDM Lancer Evolution X SST.xml` | `.XML` | `18,832` bytes | RomRaider / EcuFlash XML Definition |
| `56870008 2011 JDM Lancer Evolution X 5MT.xml` | `.XML` | `22,226` bytes | RomRaider / EcuFlash XML Definition |
| `56880005 2011 JDM Lancer Evolution X SST.xml` | `.XML` | `20,898` bytes | RomRaider / EcuFlash XML Definition |
| `56880009 2011 JDM Lancer Evolution X SST.xml` | `.XML` | `22,235` bytes | RomRaider / EcuFlash XML Definition |
| `56890007 2011 USDM Lancer Evolution X 5MT.xml` | `.XML` | `25,315` bytes | RomRaider / EcuFlash XML Definition |
| `56890009 2011 USDM Lancer Evolution X 5MT.xml` | `.XML` | `28,454` bytes | RomRaider / EcuFlash XML Definition |
| `56890010 2011 USDM Lancer Evolution X 5MT.xml` | `.XML` | `918` bytes | RomRaider / EcuFlash XML Definition |
| `56890013 2011 USDM Lancer Evolution X 5MT.xml` | `.XML` | `22,975` bytes | RomRaider / EcuFlash XML Definition |
| `56890109 2011 USDM Lancer Evolution X 5MT.xml` | `.XML` | `733` bytes | RomRaider / EcuFlash XML Definition |
| `56900007 2011 USDM Lancer Evolution X SST.xml` | `.XML` | `13,303` bytes | RomRaider / EcuFlash XML Definition |
| `56900009 2011 USDM Lancer Evolution X SST.xml` | `.XML` | `27,748` bytes | RomRaider / EcuFlash XML Definition |
| `56900010 2011 USDM Lancer Evolution X SST.xml` | `.XML` | `918` bytes | RomRaider / EcuFlash XML Definition |
| `56910007 2011 EDM Lancer Evolution X 5MT.xml` | `.XML` | `25,142` bytes | RomRaider / EcuFlash XML Definition |
| `56910009 2011 EDM Lancer Evolution X 5MT.xml` | `.XML` | `21,229` bytes | RomRaider / EcuFlash XML Definition |
| `56920006 2011 EDM Lancer Evolution X SST.xml` | `.XML` | `28,667` bytes | RomRaider / EcuFlash XML Definition |
| `56920008 2011 EDM Lancer Evolution X SST.xml` | `.XML` | `28,351` bytes | RomRaider / EcuFlash XML Definition |
| `56940007 2011 USDM Lancer Ralliart SST.xml` | `.XML` | `22,437` bytes | RomRaider / EcuFlash XML Definition |
| `56940009 2011 USDM Lancer Ralliart SST.xml` | `.XML` | `10,344` bytes | RomRaider / EcuFlash XML Definition |
| `56940010 2011 USDM Lancer Ralliart SST.xml` | `.XML` | `915` bytes | RomRaider / EcuFlash XML Definition |
| `56950006 2011 EDM Lancer Ralliart SST.xml` | `.XML` | `18,158` bytes | RomRaider / EcuFlash XML Definition |
| `57140001 2011 EDM Lancer Evolution X SST.xml` | `.XML` | `34,443` bytes | RomRaider / EcuFlash XML Definition |
| `57140003 2011 EDM Lancer Evolution X SST.xml` | `.XML` | `27,730` bytes | RomRaider / EcuFlash XML Definition |
| `58010005 2012 USDM Lancer Evolution X 5MT.xml` | `.XML` | `23,447` bytes | RomRaider / EcuFlash XML Definition |
| `58020005 2012 USDM Lancer Evolution X SST.xml` | `.XML` | `28,828` bytes | RomRaider / EcuFlash XML Definition |
| `58030005 2012 USDM Lancer Ralliart SST.xml` | `.XML` | `25,198` bytes | RomRaider / EcuFlash XML Definition |
| `58030006 2012 USDM Lancer Ralliart SST.xml` | `.XML` | `655` bytes | RomRaider / EcuFlash XML Definition |
| `58045804 2014 EDM Lancer Evolution X 5MT.xml` | `.XML` | `10,878` bytes | RomRaider / EcuFlash XML Definition |
| `58640002 2012 EDM Lancer Ralliart SST.xml` | `.XML` | `25,241` bytes | RomRaider / EcuFlash XML Definition |
| `59570004 2013 USDM Lancer Ralliart SST.xml` | `.XML` | `29,281` bytes | RomRaider / EcuFlash XML Definition |
| `59580004 2013 USDM Lancer Evolution X 5MT.xml` | `.XML` | `29,432` bytes | RomRaider / EcuFlash XML Definition |
| `59580005 2013 USDM Lancer Evolution X 5MT.xml` | `.XML` | `923` bytes | RomRaider / EcuFlash XML Definition |
| `59590004 2013 USDM Lancer Evolution X SST.xml` | `.XML` | `30,845` bytes | RomRaider / EcuFlash XML Definition |
| `59590005 2013 USDM Lancer Evolution X SST.xml` | `.XML` | `923` bytes | RomRaider / EcuFlash XML Definition |
| `80700010 2002 JDM Lancer Evo 7 AT.xml` | `.XML` | `24,261` bytes | RomRaider / EcuFlash XML Definition |
| `80920002 2005 JDM Lancer Evolution MT.xml` | `.XML` | `13,128` bytes | RomRaider / EcuFlash XML Definition |
| `88570008 2005 JDM Lancer Evolution MT.xml` | `.XML` | `21,789` bytes | RomRaider / EcuFlash XML Definition |
| `88580013 2006 ADM Lancer Evolution MT.xml` | `.XML` | `13,873` bytes | RomRaider / EcuFlash XML Definition |
| `88580014 2007 ADM Lancer Evolution MT.xml` | `.XML` | `747` bytes | RomRaider / EcuFlash XML Definition |
| `88580015 2006 JDM Lancer Evolution MT.xml` | `.XML` | `12,915` bytes | RomRaider / EcuFlash XML Definition |
| `88590013 2006 USDM Lancer Evolution MT.xml` | `.XML` | `11,320` bytes | RomRaider / EcuFlash XML Definition |
| `88590014 2006 USDM Lancer Evolution MT.xml` | `.XML` | `676` bytes | RomRaider / EcuFlash XML Definition |
| `88590015 2006 USDM Lancer Evolution MT.xml` | `.XML` | `18,043` bytes | RomRaider / EcuFlash XML Definition |
| `88590016 2006 USDM Lancer Evolution MT.xml` | `.XML` | `742` bytes | RomRaider / EcuFlash XML Definition |
| `88780004 2008 JDM Lancer Evolution AT.xml` | `.XML` | `26,798` bytes | RomRaider / EcuFlash XML Definition |
| `88840013 2006 EDM Lancer Evolution MT.xml` | `.XML` | `9,126` bytes | RomRaider / EcuFlash XML Definition |
| `88840016 2006 EDM Lancer Evolution MT.xml` | `.XML` | `11,474` bytes | RomRaider / EcuFlash XML Definition |
| `88840017 2006 EDM Lancer Evolution MT.xml` | `.XML` | `11,568` bytes | RomRaider / EcuFlash XML Definition |
| `89280002 2006 JDM Lancer Evolution MT.xml` | `.XML` | `13,566` bytes | RomRaider / EcuFlash XML Definition |
| `89960000 2005 JDM Lancer Evolution MT.xml` | `.XML` | `17,729` bytes | RomRaider / EcuFlash XML Definition |
| `89980000 2006 JDM Lancer Evolution MT.xml` | `.XML` | `13,556` bytes | RomRaider / EcuFlash XML Definition |
| `90550001 2001 EDM Lancer Evo 7 5MT.xml` | `.XML` | `8,420` bytes | RomRaider / EcuFlash XML Definition |
| `90551001 2001 EDM Lancer Evo 7 5MT.xml` | `.XML` | `917` bytes | RomRaider / EcuFlash XML Definition |
| `92460000 2001 JDM Lancer Evo 7 Ralliart 6MT.xml` | `.XML` | `10,315` bytes | RomRaider / EcuFlash XML Definition |
| `93390000 2001 JDM Evo 7 MT.xml` | `.XML` | `16,172` bytes | RomRaider / EcuFlash XML Definition |
| `93660005 2004 JDM Lancer Evo 8 FQ300 MT.xml` | `.XML` | `9,001` bytes | RomRaider / EcuFlash XML Definition |
| `93670005 2004 JDM Lancer Evo 8 MR RS MT.xml` | `.XML` | `13,529` bytes | RomRaider / EcuFlash XML Definition |
| `94170008 2004 USDM Lancer Evo 8 MT.xml` | `.XML` | `8,801` bytes | RomRaider / EcuFlash XML Definition |
| `94170014 2004 USDM Lancer Evo 8 MT.xml` | `.XML` | `9,497` bytes | RomRaider / EcuFlash XML Definition |
| `94170015 2004 USDM Lancer Evo 8 MT.xml` | `.XML` | `9,555` bytes | RomRaider / EcuFlash XML Definition |
| `96260007 2004 JDM Lancer Evo 8 MT.xml` | `.XML` | `14,949` bytes | RomRaider / EcuFlash XML Definition |
| `96260009 2004 JDM Lancer Evo 8 MT.xml` | `.XML` | `38,365` bytes | RomRaider / EcuFlash XML Definition |
| `96420007 2004 USDM Lancer Evo 8 MT.xml` | `.XML` | `8,839` bytes | RomRaider / EcuFlash XML Definition |
| `96420008 2004 USDM Lancer Evo 8 MT.xml` | `.XML` | `8,741` bytes | RomRaider / EcuFlash XML Definition |
| `96420011 2004 USDM Lancer Evo 8 MT.xml` | `.XML` | `8,665` bytes | RomRaider / EcuFlash XML Definition |
| `96530006 2005 ADM Lancer Evo 8 MT.xml` | `.XML` | `29,970` bytes | RomRaider / EcuFlash XML Definition |
| `96940011 2005 USDM Lancer Evo 8 MT.xml` | `.XML` | `13,050` bytes | RomRaider / EcuFlash XML Definition |
| `97250001 2004 JDM Lancer Evo 8 GSR MT.xml` | `.XML` | `11,823` bytes | RomRaider / EcuFlash XML Definition |
| `97470001 2005 JDM Lancer Evo 8 MT.xml` | `.XML` | `666` bytes | RomRaider / EcuFlash XML Definition |
| `98640014 2002 JDM Lancer Evo 7 MT.xml` | `.XML` | `22,255` bytes | RomRaider / EcuFlash XML Definition |
| `98640016 2002 JDM Lancer Evo 7 MT.xml` | `.XML` | `15,535` bytes | RomRaider / EcuFlash XML Definition |
| `98650012 2001 EDM Lancer Evo 7 5MT.xml` | `.XML` | `16,093` bytes | RomRaider / EcuFlash XML Definition |
| `98650014 2001 JDM Lancer Evo 7 MT.xml` | `.XML` | `618` bytes | RomRaider / EcuFlash XML Definition |
| `98650015 2001 EDM Lancer Evo 7 5MT.xml` | `.XML` | `21,550` bytes | RomRaider / EcuFlash XML Definition |
| `98650017 2001 EDM Lancer Evo 7 5MT.xml` | `.XML` | `27,064` bytes | RomRaider / EcuFlash XML Definition |
| `99270000 2004 EDM Lancer Evo 8 MT.xml` | `.XML` | `12,149` bytes | RomRaider / EcuFlash XML Definition |
| `99860002 2001 JDM Lancer Evo 7 MT.xml` | `.XML` | `10,149` bytes | RomRaider / EcuFlash XML Definition |
| `DM401702 2004 USDM Lancer Evo 8 ACD.xml` | `.XML` | `544` bytes | RomRaider / EcuFlash XML Definition |
| `SM5237.xml` | `.XML` | `3,869` bytes | RomRaider / EcuFlash XML Definition |
| `evo10base.xml` | `.XML` | `97,344` bytes | RomRaider / EcuFlash XML Definition |
| `evo5base.xml` | `.XML` | `25,493` bytes | RomRaider / EcuFlash XML Definition |
| `evo7base.xml` | `.XML` | `53,095` bytes | RomRaider / EcuFlash XML Definition |
| `evo9base.xml` | `.XML` | `56,454` bytes | RomRaider / EcuFlash XML Definition |

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
