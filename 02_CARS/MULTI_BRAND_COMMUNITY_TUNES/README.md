# MULTI BRAND COMMUNITY TUNES - ECU Calibration Suite

**Repository Path**: `02_CARS/MULTI_BRAND_COMMUNITY_TUNES`  
**Classification**: `Complete Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `227 files` (137 binary dumps, 90 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MULTI_BRAND_COMMUNITY_TUNES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `'01 C1500 LM7 os12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `'01 GMC c1500 LM7 os 12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `'01 K1500 4.8 LR4 os12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `'01 K2500 8.1L18 0s12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `'01 LM7 os12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `'01C1500 LM7 os12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `'01K2500 6.0L os12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `00_File_Dropoff_Zone_01 chevy MPV 4x4 Half T LM7 os12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `00_File_Dropoff_Zone_12208322 - 2001 512k.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12208322` |
| `01 chevy MPV 4x4 Half T LM7 os12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `04 Chevy 1500 4x2 LM7 12606960.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12606960` |
| `04_hummer_lq4.bin` | `.BIN` | `1,048,576` bytes | Binary Firmware / Calibration Dump |
| `05 Escalade 4x4 6.0L os12592618 (bad read unknown file).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12592618` |
| `12202088 - 2001 512k.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12202088` |
| `12202088_1GCCS19W218000000.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12202088` |
| `12202088_1GKEK13T31J000000.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12202088` |
| `12202088_1GTHC29U21E142995.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12202088` |
| `12202088_2G2FV22G112102638.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12202088` |
| `12202088_6H8VXL69F2L000000.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12202088` |
| `12202088_release.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12202088` |
| `12208322 - 2001 512k.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12208322` |
| `12208322_1GCHK29G91E696969.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `12208322_release.xdf` | `.XDF` | `632,290` bytes | General Motors Operating System ID `12208322` |
| `12209203_release.xdf` | `.XDF` | `602,221` bytes | General Motors Operating System ID `12209203` |
| `12212156_1G1YY22G6X5111143.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `12212156_1G1YY22GX25000000.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `12212156_2G1FP22G422116016.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `12212156_release.xdf` | `.XDF` | `602,206` bytes | General Motors Operating System ID `12212156` |
| `12212456_1GCEC14VX2Z163908.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212456` |
| `12216125_1GCHK24G12E144906.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12216125` |
| `12216125_1GNEC13Z32R141325.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12216125` |
| `12216125_1GNEK13Z12J195448.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12216125` |
| `12216125_1GNEK13Z12J274831.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12216125` |
| `12216125_2GCEC19T721149335.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12216125` |
| `12216125_TCS.xdf` | `.XDF` | `695` bytes | General Motors Operating System ID `12216125` |
| `12221588_1G1YY32G335103629.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12221588` |
| `12221588_2G1FP22G5Y2131942.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12221588` |
| `12579405_1GCEK19T83Z169590.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12579405` |
| `12579405_1GCGC13U53F206572.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12579405` |
| `12579405_1GCHC29U83E120616.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12579405` |
| `12579405_1GCHG35U331236717.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12579405` |
| `12579405_1GNEC13V63R276233.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12579405` |
| `12579405_2GCEK19N031360785.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12579405` |
| `12579405_3GNEC16ZX3G288853.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12579405` |
| `12585950_1GCHK29U64E114043.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12585950` |
| `12585950_2GCEK19N741126869.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12585950` |
| `12585950_2GCEK19N941123424.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12585950` |
| `12587603_1GBHC29U44E392439.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_1GCEC14T64Z187804.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_1GCEC14T64Z346451.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_1GCEK14V14Z268035.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_1GNEK13Z44R249913.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_1GTGG25V141136017.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_1GTJK33G34F202522.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_1GYEC63T64R228179.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_2GTEC19T231296115.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_3GNEK12T84G241360.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `12587603_RC1.xdf` | `.XDF` | `801,440` bytes | General Motors Operating System ID `12587603` |
| `12587603_release.xdf` | `.XDF` | `632,058` bytes | General Motors Operating System ID `12587603` |
| `12587604_6G2VX12G14L000000.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587604` |
| `12587811_1GBHC24UX6E168635.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587811` |
| `12587811_1GKFK66U46J133580.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587811` |
| `12587811_2GCEK13T661195420.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587811` |
| `12592433_1G6DN57S040162128.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592433` |
| `12592433_6G1ZK54F55L000000.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592433` |
| `12592433_Beta_metric.xdf` | `.XDF` | `597,935` bytes | General Motors Operating System ID `12592433` |
| `12592433_beta_imperial.xdf` | `.XDF` | `605,011` bytes | General Motors Operating System ID `12592433` |
| `12592618_1G6DN56S350111175.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_1GCEC19T75Z242416.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_1GCEK14V05Z146817.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_1GCEK19B25Z111288.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_1GCGG29U751203383.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_1GKGC26U85R119031.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_1GNEC13V95J131348.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_1GNEK13T65J129980.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_1GTJK39U85E181333.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_2GCEK13T351221762.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_2GCEK19NX51167871.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_3GNEK12Z35G151684.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_3GYFK66NX5G204649.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_5GRGN23U25H106645.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12592618` |
| `12592618_alpha.xdf` | `.XDF` | `27,449` bytes | General Motors Operating System ID `12592618` |
| `12593058_1GKET16P436178491.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12593058` |
| `12593058_2GCEK19N331361459.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12593058` |
| `12606807_1GCGG25V561221591.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12606807` |
| `12606807_1GCHK24U16E257895.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12606807` |
| `12606807_1GCHK29U26E235719.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12606807` |
| `12606807_3GCEC14X26G262682.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12606807` |
| `12613246_1GBHC24UX6E168635.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12613246` |
| `12613246_1GCHK24U16E257895.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12613246` |
| `12613246_1GCHK29U26E235719.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12613246` |
| `12613246_2GCEK13T661195420.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12613246` |
| `12619623_1GCEC19Z26Z287138.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12619623` |
| `12619623_1GNEK13Z66R166194.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12619623` |
| `12624402_6G2EC57Y18L120977.bin` | `.BIN` | `2,097,152` bytes | General Motors Operating System ID `12624402` |
| `12624402_6G2EC57Y69L123456.bin` | `.BIN` | `2,097,152` bytes | General Motors Operating System ID `12624402` |
| `12639270_6G1EK4EY1AL403616.bin` | `.BIN` | `2,097,152` bytes | General Motors Operating System ID `12639270` |
| `12652955_2G1FS1EP0C9801174.bin` | `.BIN` | `2,097,152` bytes | General Motors Operating System ID `12652955` |
| `145_1.4_16V_TS_0261204481_1037358388.xdf` | `.XDF` | `459,610` bytes | Bosch Motronic Hardware ID `0261204481` |
| `145_1.6_16V_TS_0261200695_1267358244.xdf` | `.XDF` | `392` bytes | Bosch Motronic Hardware ID `0261200695` |
| `145_1.7_16V_0261203354_1267358146.xdf` | `.XDF` | `124,326` bytes | Bosch Motronic Hardware ID `0261203354` |
| `145_1.7_16V_0261203849_358699.xdf` | `.XDF` | `127,918` bytes | Bosch Motronic Hardware ID `0261203849` |
| `145_2.0_16V_TS_0261204478_1037358492.xdf` | `.XDF` | `172,604` bytes | Bosch Motronic Hardware ID `0261204478` |
| `15166853_1GCHK23132F225610.bin` | `.BIN` | `524,288` bytes | Binary Firmware / Calibration Dump |
| `15186006_1GCHK23192F219021.bin` | `.BIN` | `524,288` bytes | Binary Firmware / Calibration Dump |
| `15189044_1GTHK23124F108622.bin` | `.BIN` | `524,288` bytes | Binary Firmware / Calibration Dump |
| `155_1.7_TS_0261200536_1267357669.xdf` | `.XDF` | `174,531` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_1.8_16V_TS_0261203846_1267358560.xdf` | `.XDF` | `148,958` bytes | Bosch Motronic Hardware ID `0261203846` |
| `155_1.8_16V_TS_0261204168_355197.xdf` | `.XDF` | `172,482` bytes | Bosch Motronic Hardware ID `0261204168` |
| `155_1.8_TS_0261200536_1267356588.xdf` | `.XDF` | `187,477` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_1.8_TS_0261200536_1267357151.xdf` | `.XDF` | `187,488` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_1.8_TS_0261200536_1267357963.xdf` | `.XDF` | `178,714` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_2.0_16V_TS_0261203862_355410.xdf` | `.XDF` | `159,408` bytes | Bosch Motronic Hardware ID `0261203862` |
| `155_2.0_16V_TS_0261203993_355908.xdf` | `.XDF` | `159,450` bytes | Bosch Motronic Hardware ID `0261203993` |
| `155_2.0_TS_0261200536_1267357094.xdf` | `.XDF` | `187,510` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_2.0_TS_0261200536_1267357151.xdf` | `.XDF` | `187,488` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_2.0_TS_0261200536_1267357669.xdf` | `.XDF` | `174,531` bytes | Bosch Motronic Hardware ID `0261200536` |
| `155_2.5_V6_0261200537_1267356596.xdf` | `.XDF` | `108,630` bytes | Bosch Motronic Hardware ID `0261200537` |
| `155_2.5_V6_0261203829_1267358578.xdf` | `.XDF` | `131,243` bytes | Bosch Motronic Hardware ID `0261203829` |
| `164_2.0_TS_0261200108_1267355452.xdf` | `.XDF` | `221,766` bytes | Bosch Motronic Hardware ID `0261200108` |
| `164_2.0_TS_0261200108_1267355604.xdf` | `.XDF` | `221,818` bytes | Bosch Motronic Hardware ID `0261200108` |
| `164_2.0_TS_0261200108_1267356191.xdf` | `.XDF` | `221,851` bytes | Bosch Motronic Hardware ID `0261200108` |
| `164_3.0_12V_0261200117_1267355710.xdf` | `.XDF` | `218,444` bytes | Bosch Motronic Hardware ID `0261200117` |
| `164_3.0_12V_0261200117_1267356096.xdf` | `.XDF` | `217,659` bytes | Bosch Motronic Hardware ID `0261200117` |
| `164_3.0_12V_0261200117_1267356310.xdf` | `.XDF` | `217,659` bytes | Bosch Motronic Hardware ID `0261200117` |
| `1997 5.7L LT1 Camaro BTZB M6 Manual.bin` | `.BIN` | `524,288` bytes | Binary Firmware / Calibration Dump |
| `2001 5.3 Auto OS12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `2001 8.1 12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `2001 Chevrolet Silverado Truck Automatic LQ4 6.0 Litre (12208322).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `2001 Chevy 1500 4x2 4.8 LR4 12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `20014.84x4 12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `2001_6.0_OS12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `2002 Chevrolet Express Van Automatic L31 5.7L 4L60e 2wd (12212156) Lean Cruise (1).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002 Chevrolet Express Van Automatic L31 5.7L 4L60e 2wd (12212156) Lean Cruise.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002 Chevrolet Express Van L31 5.7 Litre 4L80E(12212156).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002 Chevrolet Silverado Truck Auto LM7 5.3L (12212156) (1).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002 Chevrolet Silverado Truck Auto LM7 5.3L (12212156).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002 Chevrolet Silverado Truck Manual LM7 5.3 Litre (12212156) (1).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002 Chevrolet Silverado Truck Manual LM7 5.3 Litre (12212156).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002 Chevy S-10 L35 4.3L 4L60E (12212156).bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002 Chevy S-10 L35 4.3L 4L60E (12212156)Lean Cruise.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `2002Silverado-53-4L60E-stock.bin` | `.BIN` | `524,288` bytes | Binary Firmware / Calibration Dump |
| `2004 4.3L LU3 Manual Full Size Truck 4x2 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 4.8L LR4 DBC 4L80E Express Van 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 4.8L LR4 DBW Manual NV3500 4x4 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 5.3L L59 DBW 4L60E 4x4 Flex Fuel 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 5.3L LM4 GMC Envoy 4x4 12587603 OS Stock.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 6.0L LQ4 DBC 4L80E Express Van 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 6.0L LQ4 DBW 4L65E 4x4 Yukon 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 6.0L LQ4 DBW 4L80E 4x4 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 6.0L LQ4 DBW Manual NV4500 4x4 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 6.0L LQ9 DBW 4L65E AWD Silverado SS 12587603 OS STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 Blazer 4.3L (12587603).bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2004 Corvette M6 Stock (bad read unknown file).bin` | `.BIN` | `13,895,779` bytes | Binary Firmware / Calibration Dump |
| `2004-4.8L-LR4-DBC-4L80E-Express-Van-12587603-OS-STOCK.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12587603` |
| `2005 Grand Am GT LA1 12594385.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12594385` |
| `2006_stock_4.8_4x4 os 12606807.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `12606807` |
| `2007 Holden Commodore Sedan Automatic L98 6.0 Litre (12612381).bin` | `.BIN` | `2,097,152` bytes | General Motors Operating System ID `12612381` |
| `2013_Sonic_ABMW_Flex_Stock.bin` | `.BIN` | `3,145,728` bytes | Binary Firmware / Calibration Dump |
| `2015_Cruz_Turbo_Stock_AB67.bin` | `.BIN` | `3,145,728` bytes | Binary Firmware / Calibration Dump |
| `52373027_1GCHC24U55E245471.bin` | `.BIN` | `1,048,576` bytes | General Motors Operating System ID `52373027` |
| `75_3.0_12V_0261200141_1267356097.xdf` | `.XDF` | `211,491` bytes | Bosch Motronic Hardware ID `0261200141` |
| `8D0907551M-20190711.xdf` | `.XDF` | `503,633` bytes | TunerPro Binary Definition Map |
| `AM28F010_DUCATI_900_SS_EU.bin` | `.BIN` | `131,072` bytes | Binary Firmware / Calibration Dump |
| `Acura_NSX_and_Legend.xdf` | `.XDF` | `637,576` bytes | TunerPro Binary Definition Map |
| `BMW_ECM_Designation_copy_for_new_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `BPL9.xdf` | `.XDF` | `5,958` bytes | TunerPro Binary Definition Map |
| `BUEIA_V5.xdf` | `.XDF` | `118,815` bytes | TunerPro Binary Definition Map |
| `Ducati_M15_3.xdf` | `.XDF` | `28,677` bytes | TunerPro Binary Definition Map |
| `E92-2016-sierra-5.3-auto-ECMonly.bin` | `.BIN` | `4,194,304` bytes | Binary Firmware / Calibration Dump |
| `E92A-2018-Sierra-5.3-auto-ECM.bin` | `.BIN` | `4,194,304` bytes | Binary Firmware / Calibration Dump |
| `Escalade 2004 LQ9 6.0_4L60E.bin` | `.BIN` | `1,048,576` bytes | Binary Firmware / Calibration Dump |
| `GTV_2.0_16V_TS_0261203671_355934.xdf` | `.XDF` | `159,425` bytes | Bosch Motronic Hardware ID `0261203671` |
| `GTV_2.0_V6_TURBO_0261203869_1267358696.xdf` | `.XDF` | `145,136` bytes | Bosch Motronic Hardware ID `0261203869` |
| `GTV_2.0_V6_TURBO_0261203883_1037358648.xdf` | `.XDF` | `145,594` bytes | Bosch Motronic Hardware ID `0261203883` |
| `General_Motors_E38_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `General_Motors_E54_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `General_Motors_E67_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `General_Motors_E67_Software_00_File_Dropoff_Zone_2005 Grand Am GT LA1 12594385.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12594385` |
| `General_Motors_E92_Hardware_12589162-example_readme.xml` | `.XML` | `170` bytes | General Motors Operating System ID `12589162` |
| `General_Motors_E92_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `General_Motors_P01_Hardware_12589162-example_readme.xml` | `.XML` | `170` bytes | General Motors Operating System ID `12589162` |
| `General_Motors_P01_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `General_Motors_P04_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `General_Motors_P04_Software_00_File_Dropoff_Zone_2005 Grand Am GT LA1 12594385.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12594385` |
| `General_Motors_P59_Hardware_12589162_readme.xml` | `.XML` | `170` bytes | General Motors Operating System ID `12589162` |
| `General_Motors_P59_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `General_Motors_P59_Software_12587603_Operating_System_12587603_release.xdf` | `.XDF` | `632,058` bytes | General Motors Operating System ID `12587603` |
| `General_Motors_P59_Software_12592433_Operating_System_Lean Cruise.xdf` | `.XDF` | `2,032` bytes | General Motors Operating System ID `12592433` |
| `LS1A-1998-Fbody.bin` | `.BIN` | `524,288` bytes | Binary Firmware / Calibration Dump |
| `Lean Cruise.xdf` | `.XDF` | `2,032` bytes | TunerPro Binary Definition Map |
| `No Password - 12587603_release.xdf` | `.XDF` | `631,750` bytes | General Motors Operating System ID `12587603` |
| `No Password - OS12212156 - 2002 512kB PCM - v5_old.xdf` | `.XDF` | `1,272,938` bytes | General Motors Operating System ID `12212156` |
| `No Password - Operating System 12202088 - 512Kb PCM - 2001 model year.xdf` | `.XDF` | `620,841` bytes | General Motors Operating System ID `12202088` |
| `No Password - Operating System 12208322 - 512Kb PCM - 2001 model year.xdf` | `.XDF` | `620,841` bytes | General Motors Operating System ID `12208322` |
| `No Password - Operating System 12209203 - 512Kb PCM - 2002 model year.xdf` | `.XDF` | `618,128` bytes | General Motors Operating System ID `12209203` |
| `No Password - Operating System 12216125 - 512Kb PCM - 2002 model year - 5.3L Flex Fuel and 8.1L engines.xdf` | `.XDF` | `643,408` bytes | General Motors Operating System ID `12216125` |
| `No Password - Operating System 12221588 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | `.XDF` | `623,195` bytes | General Motors Operating System ID `12221588` |
| `No Password - Operating System 12225074 - 512Kb PCM - 2001 to 2004 Holden model years.xdf` | `.XDF` | `618,194` bytes | General Motors Operating System ID `12225074` |
| `No Password - Operating System 12593358 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | `.XDF` | `623,195` bytes | General Motors Operating System ID `12593358` |
| `No Password - XDF for Operating System 12202088 - 2001 512Kb PCM - Version 5.xdf` | `.XDF` | `632,026` bytes | General Motors Operating System ID `12202088` |
| `No Password - XDF for Operating System 12208322 - 2001 512Kb PCM - Version 5.xdf` | `.XDF` | `632,026` bytes | General Motors Operating System ID `12208322` |
| `No Password - __Operating System 12212156 - 512Kb PCM - 2002 model year.xdf` | `.XDF` | `618,112` bytes | General Motors Operating System ID `12212156` |
| `OS12212156 - 2002 512kB PCM - v5_old.xdf` | `.XDF` | `1,273,255` bytes | General Motors Operating System ID `12212156` |
| `OS12212156 - 2002 512kB PCM - v6 - no password.xdf` | `.XDF` | `1,687,463` bytes | General Motors Operating System ID `12212156` |
| `OldBlueFactory.bin` | `.BIN` | `1,048,576` bytes | Binary Firmware / Calibration Dump |
| `Operating System 12202088 - 512Kb PCM - 2001 model year.xdf` | `.XDF` | `621,149` bytes | General Motors Operating System ID `12202088` |
| `Operating System 12208322 - 512Kb PCM - 2001 model year.xdf` | `.XDF` | `621,149` bytes | General Motors Operating System ID `12208322` |
| `Operating System 12209203 - 512Kb PCM - 2002 model year.xdf` | `.XDF` | `618,436` bytes | General Motors Operating System ID `12209203` |
| `Operating System 12216125 - 512Kb PCM - 2002 model year - 5.3L Flex Fuel and 8.1L engines.xdf` | `.XDF` | `643,716` bytes | General Motors Operating System ID `12216125` |
| `Operating System 12221588 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | `.XDF` | `623,503` bytes | General Motors Operating System ID `12221588` |
| `Operating System 12225074 - 512Kb PCM - 2001 to 2004 Holden model years.xdf` | `.XDF` | `618,502` bytes | General Motors Operating System ID `12225074` |
| `Operating System 12593358 - 512Kb PCM - Corvette 2001 to 2003 model years.xdf` | `.XDF` | `623,503` bytes | General Motors Operating System ID `12593358` |
| `P01-2001-Express-5.7-4L60E-12208322.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12208322` |
| `P01-2002-Express-5.0-4L60E-12212156.bin` | `.BIN` | `524,288` bytes | General Motors Operating System ID `12212156` |
| `P59-2003-Silverado-8.1-Allison-PCMonly.bin` | `.BIN` | `1,048,576` bytes | Binary Firmware / Calibration Dump |
| `P7_GuzziDiag_16k_V1.26.xdf` | `.XDF` | `35,393` bytes | TunerPro Binary Definition Map |
| `Peugeot_205_TURBO.xdf` | `.XDF` | `26,398` bytes | TunerPro Binary Definition Map |
| `S13RT.xdf` | `.XDF` | `125,319` bytes | TunerPro Binary Definition Map |
| `SZ_3.0_12V_0261200141_1267355737.xdf` | `.XDF` | `211,675` bytes | Bosch Motronic Hardware ID `0261200141` |
| `Stock_2004_GMC_Sierra_1500_4x4_Lm7_4l60e_truck_copy.bin` | `.BIN` | `1,048,576` bytes | Binary Firmware / Calibration Dump |
| `Volvo_ECM_Designation_copy_for_new_Hardware_CopyThisFolderForNewHardwareID_readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `XDF for Operating System 12202088 - 2001 512Kb PCM - Version 5.xdf` | `.XDF` | `632,321` bytes | General Motors Operating System ID `12202088` |
| `XDF for Operating System 12208322 - 2001 512Kb PCM - Version 5.xdf` | `.XDF` | `632,321` bytes | General Motors Operating System ID `12208322` |
| `readme.xml` | `.XML` | `170` bytes | RomRaider / EcuFlash XML Definition |
| `sr20det.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `~~Operating System 12212156 - 512Kb PCM - 2002 model year.xdf` | `.XDF` | `618,420` bytes | General Motors Operating System ID `12212156` |

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
