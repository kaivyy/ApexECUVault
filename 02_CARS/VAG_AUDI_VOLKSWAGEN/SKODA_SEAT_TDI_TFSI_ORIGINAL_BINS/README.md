# SKODA & SEAT - VAG Group TDI & TFSI Original Calibration Dumps

**Repository Path**: `02_CARS/VAG_AUDI_VOLKSWAGEN/SKODA_SEAT_TDI_TFSI_ORIGINAL_BINS`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `206 files` (206 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Koleksi 206 berkas biner original hardware dumps (.ori/.bin) untuk jajaran kendaraan platform VAG merk Skoda (Octavia I/II, Fabia I/II, Superb I/II, Roomster) dan Seat (Leon 1M/1P, Ibiza 6L/6J, Toledo, Altea, Cordoba). Meliputi mesin 1.4 TDI, 1.9 TDI (Pumpe Düse PD100, PD105, PD130, PD150, PD160 Cupra), 2.0 TDI (PD140, PD170), 1.8T 20V (150/180/210/225 PS), dan 2.0 TFSI/TSI EA113/EA888. Berbagi arsitektur ECU dan engine block 100% dengan Volkswagen Golf/Passat dan Audi A3/A4.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Bosch EDC15P, EDC15VM+, EDC16U1, EDC16U34, Motronic ME7.5, MED9.1, MED17`
- **Arsitektur MCU & Memori**: `Infineon C167 / ST10F275 / Motorola MPC562 / MPC564 / Tricore TC1766 512KB-2MB Flash`
- **Protokol Diagnostik & Flashing**: `KWP1281 / KWP2000 (TP 2.0 over CAN) / UDS (ISO 14229) / BDM100`

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
| `0281001849_038906018BQ_.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `0281001967_312.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001967_313.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `032FC.BIN` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `032QN.std` | `.STD` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `1Z0907115-0261S02114-orig.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `1Z0907115A-0261S02339-orig.BIN` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `2806.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `354563.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `356587.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `356588.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `746.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `747.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `FAbia 1.4 036906034CB .ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Fabia 1.4 75HP 047906033D 5WP4419.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Octavia 2.0TDI 140HP 03G906021AN  03G906021TC 393521.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat Altea 1.9TDI 105HP 03G906016HB 0281012288 372776.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat Arosa 1.7 SDI 50hp 038906013L 0281001748 1834 HHH.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Seat Arosa 1.7 SDI 50hp 038906013L 0281001748 1834 LLL.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Seat Ibiza 1.9 TDI 110hp ASV 0281010006 038906018FB.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat Inca 1.4i 58HP 6K0906032AE 0261207230 1037360307.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat Leon 1.9TDI 105HP 03G906021JN 382685.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat Leon 2 1.6 06A906033FF-5WP40217-01.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat alhambra 1.8T AJH 150HP 06A906018BT 0261204683 358171.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat alhambra 1.9TDI 115HP 038906019ET 0281010630 360459.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat alhambra 1.9TDI 115HP 038906019PA 0281012932 380184.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat alhambra 1.9TDI AJM 115HP 038906019J 0281010216 354462.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat alhambra 1.9TDI ASZ 130HP 038906019BH 0281011199 366689.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat alhambra 2.0TDI 140HP 03G906016JN 381823.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat altea 1.9TDI 105HP 0281011885  03G906016DG 370803.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat altea 1.9TDI 105HP 03G906021AN 382082.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat altea 2.0TDI 140HP 0281012278 1037372610.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat althea 1.9TDI 105HP 03G906016DH 0281011864 370804.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 0261204593 357494.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.4TDI 75HP 045906019BQ 0281012708 377262.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.4TDI AMF 75HP 045906019BG 0281011244 368177.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.4TDI BNM 68HP 45906019BS 0281012319 375931.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.8T 150HP 0261206023 352176.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.8T 180HP 06A906032RP 0261208521 371739.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.8T AYP 150HP 6K0906032AA 0261207071 354562.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI AFN 110HP 028906021EK 0281001584.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI ALH 90HP 038906018EE 0281001916.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI ASV 110HP 038906018FB 0281010006 352282.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI ASZ 130HP 038906019DQ 0281010891 363556.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI ASZ 130HP 038906019NF 0281011825 369971.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI ATD 100HP 038906019HQ 0281010957 363252.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI ATD 100HP 038906019NE 0281011824 371258.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI BLT 130HP 038906019NJ 0281011823 375966.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TDI BLT 130HP 038906019NJ 0281011823 389851.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 1.9TID 100HP 038906019NL 0281012276 377186.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza 90HP 038906018EC 0281001914 356953.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza cupra 1.9TDI 160HP 0281011852 370651.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat ibiza cupra 1.9TDI 160HP 038906019NT 0281012668 378813.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat lean 1.9TDI ASV 110HP 038906012HD 0281011312 367049.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.8T 180HP 0261206866 0261206866 360165.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.8T 180HP 06A906032BE 0261206551 352772.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.8T AUQ 180HP 06A906032MJ 0261208115 366379.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.8T AUQ 180HP 06A906032SJ 0261208531 369040.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.8T BAM 225HP 1ML906032A 0261208221 367220.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9SDI 68HP 038906012R 0281010058 354413.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI 03G906021LK 0281012262 377150ori.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Seat leon 1.9TDI 105HP 03G906021AN 382081.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI 110HP ASV 038906012AT 0281010062 1037350161.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI AFN 110HP 038906012BT 0281010229 352279.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI ALH 90HP 038906012FN 0281010686 360533.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI ARL 150HP 038906019FK 0281010687 362484.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI ARL 150HP 038906019FK 0281010687 362707.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI ARL 150HP 038906019HK 0281010985 363170.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI ARL 150HP 038906019HK 0281010985 363170_1.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI ASV 110HP 0281011997 0281011997 371261.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 1.9TDI ASV 110HP 038906012FK 0281010683 360530.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 2.0TDI 140HP 03G906021LL 0281013280 381350.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 2.0TDI 140HP 03G906021LL 1037381350.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 2.0TDI 140HP 03G906021LL 381350.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 2.0TDI 140HP edc16u31 03G906021AN 390153.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 2.0TDI 170HP 03G906018D.ori` | `.ORI` | `249,856` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 2.0TFSI 185HP 1P0907115D 0261S02289 377624.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon 2.0TFSI 1P0907115 0261S02113 386675.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon cupra 1.8T 180HP 06A906032T 0261206545 352761.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon cupra 2.0TFSI 240HP 1P0907115C  0261S02337 386637.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat leon-2.0TDI-140hp-03G906016AJ-0281011730.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat toledo 1.9TDI AFN 110HP 028906021EF 0281001582 357749.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat toledo 1.9TDI AFN 110HP 038906012BT 0281010229 352279.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat toledo 1.9TDI AFN 110HP 038906012T 0281001060 352232.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat toledo 1.9TDI AGR 90HP 038906012S 0281010059 359845.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat toledo 1.9TDI AGR 90HP 038906021BS 0281010228 352278.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat toledo 1.9TDI AHU 90HP 028906021FN 0281001604 746-747.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat toledo 1.9TDI AHU 90HP 038906018BT 0281001926 926687.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Alhambra_D1900_R4V2T_66kW_0281001252_028906021P_D3E_xx896_crc90FBE681.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Alhambra_D1900_R4V2T_66kW_0281001252_028906021P_D3E_xx897_crcBFE76479.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Alhambra_D1900_R4V2T_81kW_0281001731_028906021GS_1904_1037357730_731_crcD3E232EF.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Alhambra_D1900_R4V2T_81kW_0281001736_028906021HB_1907_1037356006.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Alhambra_D1900_R4V2T_81kW_0281001968_028906021JK_2017_1037350315.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Alhambra_D1900_R4V2T_81kW_0281001968_028906021JK_2019_1037352608.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Arosa_D1400_R3V2T_55kW_0281001804_045906019T_1209_1037354619.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Arosa_D1400_R3V2T_55kW_0281010211_045906019M_1043_1037352639_crcA6662AA0.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Ibiza_1,8T_180PS_0261208370_06A906032QN_371181.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Ibiza_D1900_R4V2T_110kW_0281010687_038906019FK_1469_1037362707_crc967A48EA.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Ibiza_D1900_R4V2_47kW_0281001689_038906013E_1513_xxx234_235_crc0A82DEC6.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Ibiza_D1900_R4V2_47kW_0281001701_028906021HA_1439_1037357738_739_crcC2011619.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Leon_B1800_R4V5T_154kW_0261207952_1ML906032_0001_1037363579_crc01BDF485.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Leon_B1800_R4V5_92kW_0261204969_06A906032CS_0005_1037354813_crcE01D8FC9.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Leon_B1800_R4V5_92kW_0261206587_06A906018GC_V01_1037352129_crc27C747C1.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Leon_B1800_R4V5_92kW_0261207648_06A906032JF_0002_1037362901_crcE40BCF28.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Toledo_B1800_R4V5_92kW_0261204970_06A906032CR_0005_1037354812_crc94607445.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Toledo_B1800_R4V5_92kW_0261206588_06A906018GD_V01_1037352130_crc6B3FD532.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Toledo_D1900_R4V2T_66kW_0281001604_028906021FN_1417_1037357258_259_crc0B3C861E.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Toledo_D1900_R4V2T_66kW_0281001864_038906018DQ_2146_1037356835_836_crcB3581B58.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Seat_Toledo_D1900_R4V2T_81kW_0281001582_038906021EF_1419_1037357262_263_crc5DB05C9A.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda 2.0TDI 140HP 03G906021AB 390602.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Fabia 1.2 40KW 03D906032A.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Fabia 1.4 16V  03C906024B 03C906024F 0896 MARELLI 4HV.ori` | `.ORI` | `917,504` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Fabia 1.4 16V  03C906024R 03C906024F 2489 MARELLI 4HV.ori` | `.ORI` | `917,504` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Fabia 1.4 16V 03C906024B 4115  MARELLI 4HV .ori` | `.ORI` | `917,504` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Fabia 1.4 16V 03C906024R 4117 MARELLI 4HV.ori` | `.ORI` | `917,504` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Faleicia 1.3i 40KW 5WP4248.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 1.6MPi 75PS 032906014A.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 1.6MPi 75PS 032906014F.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 1.6i 100HP 5WP4428 01 06A906019BT.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 1.9 TDI 105HP 03G906021RH 389825.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 1.9TDI 100HP 0281010517 038906019R 360060.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 1.9TDI 105HP 03G906021RR 391862.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 2  1.4i 036906032BF.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 2  2.0FSI 150PS 0261S02259 378588.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 2.0 170HP RS 03G906018EL  9953.ori` | `.ORI` | `249,856` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 2.0FSI 0261S02018 06F906056R 372560.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 2.0TDI 140HP 03G906021LD_0281013187_391532.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia 2.0TDI 140HP 03G906021LD_0281013187_Skoda Octavia 2.0TDI 140HP 03G906021LD_0281013187_381024.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia Scount 2.0TDI 140HP 03G906021MC 390602.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Octavia-1.8T-06A906032HJ-0261207436-1037362287.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Skoda Octavia-1.8T-06A906032HJ-0261207436-1037366426.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Skoda Superb 2.0TDI 140HP 03G906016GT 387090.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda Superb 2.8 1 02612085471 3B0907551DD 369310.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.4 16V 100HP 036906034BK IAW 4LV.C.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.4 68HP 5WP40179 047906033H.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.4TDI 70HP 045906019BR 0281012318 377261.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.9SDI 64HP 038906012AN 0281010107 354365.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.9SDI 64HP 038906012GD 0281010861 362792.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.9SDI 64HP 038906012HR 0281011321 1037367058.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.9TDI 105HP 038906019NS 0281013082 386363.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.9TDI 130HP 038906019 0281011217 366587.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.9TDI ASZ 130HP 038906019LA 0281011217 368406.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.9TDI ASZ 130HP 038906019NF 0281011825 372304.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda fabia 1.9TDI ATD 100HP 038906019KT 0281011219 368184.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda ocatavia 1.9TDI AHF 110HP 038906012G 0281010128 360549.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.6 06A906019BH 5WP4860.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.6 AEE 032906030AG.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.6i 06A906033BG 5WP4015.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.8T AGU 150HP 06A906018CF 0261206141 5663756.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.8T AGU 150HP 06A906018GA 261206519 352013.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.8T AGU 150HP 06A906018GB 0261206520 350785.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.8T ANB 150HP 4B0906018AC 0261206452 352160.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9SDI 68HP 038906012E 0281010105 360446.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI 105HP 03G906016K 0281012237 372601.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI 105HP 03G906021LB 382414.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI 130HP 038906019EG 0281010928 351906.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI 90HP 038906012F 0281010127 350855.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI 90HP 038906012F 0281010127 360546.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AGR 90HP 038906012F 0281010127 1037350855.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AGR 90HP 038906012H 0281010129 350857.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AGR 90HP 038906018AG 0281001695 357789.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AGR 90HP 038906018BC 0281001755 357868.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AGR 90HP 038906018GM 0281010181 350932.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AHF 110HP 038906012G 0281010128 350856.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AHF 110HP 038906018AM 0281001707 242.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AHF 110HP 038906018GN 0281010182 110934.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI AHU 90HP 038906018B 0281001602 355556.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI ASV 110HP 038906012BA 0281010130 352668.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI ASV 110HP 038906012CL 0281010380 354322.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI ASV 110HP 038906012CL 0281010380 362160.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI ASV 110HP 038906012HC 0281011311 367048.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI ASZ 130HP 038906019HJ 0281010977 366272.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI ATD 100HP 038906019DL 0281011077 363696.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI ATD 100HP 038906019FJ 0281010789 362146.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 1.9TDI BJB 105HP 03G906016AG 0281011658 370256.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 110HP AHF 038906018BR 0281001850 597-598.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 2.0TDI 140HP 03G906021LD 379738.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 2.0TDI BKD 140HP 03G906016DS 0281011953 372775.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 2.0TDI BMM 140HP 03G906021JC 382441.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia 2.0TDI-03G906021JC-AB-7GG-BMM-1037392969.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Skoda octavia II 2.0TDI 140HP 03G906016F 0281011391 370892.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia RS 03G906018HB.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia RS 1.8T 180HP 06a906032bj 0261206892 360288.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia RS 1.8T AUQ 06A906032SG 0261208532 369039.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda octavia RS 2.0TFSI 200HP 1Z0907115A 0261S02339 386859.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda oktavia 1.9TDI 90HP 038906012HA 0281011309 367046.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda oktavia 1.9TDI AGR 90HP 038906012H 02810101291037360547.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda roomster 1.4TDI - 69HP 045906019CJ 0281013180 382690.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda roomster 1.9TDI 105HP 038906019NR 0281013081 381002.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda superb 1.8T 180HP 8E0909018A 0261207929 1037366458.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda superb 1.9TDI 105HP 3G906021QN 1037395404.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda superb 1.9TDI 130HP 038906019EG 0281010928 363744.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Fabia_D1900_R4V2T_74kW_0281010289_038906019AF_1056_1037352972_crc146360EC.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Fabia_D1900_R4V2T_74kW_0281010289_038906019AF_1110_1037354466_crcCBCBF822.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Octavia_1,9_TDI_105PS_0281011883_03G906016DJ_6250_1037371259.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Octavia_2,0TFSI_200PS_0261S02114_1Z0907115_377701.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Octavia_B1800_R4V5_92kW_0261204373_06A906018H_V05_1037358798_crc2ABE377E.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Octavia_B1800_R4V5_92kW_0261204681_6A906018AM_V02_1037358186_crcAAFD2CBF.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Octavia_D1900_R4V2T_74kW_0281011077_038906019DL_1548_1037363696_crc87D4BD87.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Octavia_D1900_R4V2T_84kW_0281010517_038906019R_1275_1037360480_CRC1934580e.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Superb_B1800_R4V5T_110kW_0261207928_8E0909018A_P0000_1037363930_crc97A78B5B.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Skoda_Superb_D2500_V6V4T_114kW_0281010905_3U0907401_D09_1037366618_crc08B732A0.ori` | `.ORI` | `524,290` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Sokda Fabia 1.4 68HP  047906033 5WP4419.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `WinOLS (Seat Leon Cupra (Original) as (All elements) - 386637).bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `WinOLS (Skoda New Octavia (Original) as Eprom - 379738).bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `ibiza_org_038_906_019_LA.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |

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
