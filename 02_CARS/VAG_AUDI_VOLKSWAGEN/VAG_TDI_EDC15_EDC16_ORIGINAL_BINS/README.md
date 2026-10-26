# VOLKSWAGEN & AUDI - Bosch EDC15, EDC16 & Motronic ME7 Original Master Suite

**Repository Path**: `02_CARS/VAG_AUDI_VOLKSWAGEN/VAG_TDI_EDC15_EDC16_ORIGINAL_BINS`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `882 files` (880 binary dumps, 2 definition maps)  

---

## 1. Technical Platform Overview

Pustaka master terbesar kalibrasi biner asli pabrikan dengan 882 berkas biner terverifikasi (.ori/.bin) untuk kendaraan Volkswagen (Golf IV/V, Passat B5/B6, Bora, Jetta, Polo, Sharan, Touareg, Transporter T4/T5, Crafter) dan Audi (A3 8L/8P, A4 B5/B6/B7, A6 C5/C6, TT 8N/8J). Meliputi varian mesin diesel 1.9 TDI VP/PD (AGR, ALH, ASV, ATD, AXR, AJM, ASZ, ARL), 2.0 TDI PD/CR (BKD, BKP, BMM, BMH, BMN), 2.5 TDI V6, 3.0 TDI V6, serta varian bensin 1.8 Turbo 20V (AGU, AUM, AUQ, BAM, APX) dan 2.0 TFSI (AXX, BWA, BWE, CDL).

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Bosch EDC15V, EDC15VM, EDC15P, EDC16U1, EDC16U31, EDC16U34, EDC16CP34, ME7.5, MED9.1`
- **Arsitektur MCU & Memori**: `Infineon C167CR / ST10F275 / Motorola MPC555 / MPC562 / MPC564 256KB-2MB Flash`
- **Protokol Diagnostik & Flashing**: `KWP1281 / KWP2000 (ISO 14230 / TP 2.0) / UDS / BDM100`

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
| ` VW Golf V 2.0 TFSI 1K0907115T 387445.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `._8E0909518AF_0261207939_7366883_0003_1_8L_R4_5VT__audi_170_5s.std` | `.STD` | `491` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `0-281-011-666_all_BDM_EEprom.bin` | `.BIN` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `0-281-011-666_all_BDM_Flash.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `0-281-011-666_all_BDM_Mic.bin` | `.BIN` | `459,008` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `001566h.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `001566l.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `016FEorg.127.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `018AT_0003.ORI` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `019CJ.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `019EP.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `021906258B.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `021906258BK.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `021906258BS_0261203215_v358227_OEM.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `021906258CK.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `021906258CP.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `021906258DJ_0261203045_v358341_OEM.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `021CG_high.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `021CG_low.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `021DL_H.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `021DL_L.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `022906032CS_0261207881_v368604_ME_7.1.1_OEM.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `0261204022 355640.ori` | `.ORI` | `8,192` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0261208268 8N0906018CG 369579.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0261S02291_386852.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001242_698.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001242_699.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001324_551.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001324_552.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001652-821.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281001652-822.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281010159_401Q_D66_351132_LL.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281010159_401Q_D66_351133_HH.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `0281011672 - 1037370516 - 03G906016AP - Meu Golf 2.0 TDI DSG 140hp.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `028906021AF 0281001309 867.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `028906021AF 0281001309 868.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `028906021CK-0281001423424-1037355221.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `028906021CK-0281001423424-1037355222.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `028906021CS_0281001664.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `028906021GQ_0281001682_MSA15_OEM.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `028906021GQ_0281001682_v357271_HHH683_MSA15_OEM.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `034BH_M_4MV.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `038906016H_0281011146_v371297_EDC16U31_OEM.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `038906016L_0281011433_v370476_EDC16U31_2004AT_OEM.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `038906016Q_0281011812_v371296_EDC16U31_OEM.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `038906018EB_HHH_A_0.BIN` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `038906018EB_LLL_A_0.BIN` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `038906019GC_0281010892_1037362795_A3_ATD.Bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `03G906016AB_0281012238_v376708_EDC16U34_MT_OEM.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `03G906016AC_0281012239_v376707_EDC16U34_DSG_OEM.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `03G906016GD 9577-orig.BIN` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `03L906022NH-1037399332-Q5-2,0 edc17.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `057x.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `05Golf101_195_292.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `06A90601AK.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `06A906032DS_0261207080_v360930_ME7.5_MT_OEM.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `06A906032LP_0261207955_v367518_ME7.5-1M_Jetta-1.8T-MT_OEM.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `070906016AN_368585 ori.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `1.9TDI AVF 130HP 038906019GF 0281010812 362603.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1037355659_orig.BIN` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `1037355660_orig.BIN` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `1037393968org.ori` | `.ORI` | `659,364` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `1K0907115A.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `206580.ORG.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `206619.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `2706.ori` | `.ORI` | `524,290` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `27c010.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `27æ010.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `29BL1MB.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `29BL802.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `29bl802.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `350751.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `352633.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `352634.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `354008.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `355.827.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `355.828.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `355054.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `355055.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `356791.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `356792.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `357791.ori.BIN` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `357792.ori.BIN` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `357_871.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `357_872.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `358022.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `358389.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `358390.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `359_834.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `359_835.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `360647.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `371-ECU1.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `386826.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `3C0907115S_0261S02510_v391093_MED9.1_2007AT_OEM.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `496_hhh.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `496_lll.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `4B0906018CH_0261207216_v360101_ME7.5_1M_Audi_A4_MT_OEM.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `4B0907401T-0281010153-1037352631.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `4B0907401T-0281010153-1037352632.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `4F9910401B.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `4L0907401 379749.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `887.BIN` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `888.BIN` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `8E0909518AF_0261207939_7366883_0003_1_8L_R4_5VT__audi_170_5s.std` | `.STD` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `8E0910115M_0261S02223_v387401_MED9.1_2006MT_OEM.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `8E0910115N_0261S02211_1037376490_0020.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `93C56.BIN` | `.BIN` | `256` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `A4_2.0tdi_170ps_03G906018AQ_ppd1.3_orig.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `A6 EEPROM.ori` | `.ORI` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `A6 flash.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `A6 mcu.ori` | `.ORI` | `259,606` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `A6TD7549.ORI` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `A6TD7550.ORI` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `A6_2.0L_98y_024D.bin` | `.BIN` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `A8 4_0 V8 275Ks org.binS.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `AM29F800B_1c.BIN` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `AM29F800B_2.BIN` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `AT156ES.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `AUDI A4 2.5TDI 150HP 0281001945 8D0907401F 766-767.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `AUDI S4 2.7 V6  0261206376  8D0907551E 350221.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `AUDI TT RS 340 CV 0261S02601_1037503608.ORI` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `AUDI_A2_D1200_R3V2T_44kw_0281011239_045906019BL_1037366716_crcC0956A22.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `AVPD6AF.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi  A3 1.8T 180PS 0261206269  06A906032AF 350034.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi  A6 3.0TDI 225HP 0281012269  4f0907401b_375256.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi 100 4.2 V8 280HP 4A0907557A 0261203143 357764.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi 80 1.9TDI 0281001317_875.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi 80 1.9TDI 0281001317_876.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi 80 1.9TDI 1Z 90HP 028906021GC 0281001668 357787.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi 80 1.9TDI 90HP 028906021D 0281001198.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi 80 TDI 1.9L 0281001133-2287357911-4A0907401A(Diesel).std` | `.STD` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi 80 TDI 1.9L 0281001133-2287357912-4A907401A(Turbo).std` | `.STD` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi 80 TDI 1.9L 0281001317-2537355581-021906028AP(Diesel).std` | `.STD` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi 80 TDI 1.9L 0281001317-2537355582-021906028AP(Turbo).std` | `.STD` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi 80 TDI 1.9L 0281001319-2287357877-021906028AQ(Diesel).std` | `.STD` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi 80 TDI 1.9L 0281001319-2287357878-021906028AQ(Turbo).std` | `.STD` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi 80 TDI 1.9L 0281001441-2537355890-028906021DQ(Diesel).std` | `.STD` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi 80 TDI 1.9L 0281001441-2537355891-028906021DQ(Turbo).std` | `.STD` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi A2 1.4TDI 75HP 045906019BP 0281012194 376317.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A2 1.4TDI 75HP 045906019G 0281010220 360497.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A2 1.4TDI AMF 75HP 045906019AT 0281011100 366249.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A2 1.4TDI AMF 75HP 045906019BA 0281011404 367361.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A2 1.4TDI AMF 75HP 045906019F 0281011607 368969.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A2 1.4TDI AMF 75HP 045906019G 0281010220 363201.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.6FSI 115HP 03C906056CP 0261S02187 381976.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T 06A906032BB 0261206268 350033.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T 06A906032HN 0261207440 363908.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T 150HP 06A906018AQ 0261204678 358108.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T 150HP 06A906032AS 0261206435 352354.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T 150HP 06A906032CL 0261206552 1037354003.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T 150HP 06A906032S 0261206197 359598.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T AGN 125HP 06A906018C 0261204127 355961.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T AGU 150HP 06A906018AQ 0261204678 350010.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T AGU 150HP 06A906018AQ 0261204678 359525.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T AGU 150HP 06A906018AR 0261204679 359522.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T AGU 150HP 06A906018CG 0261206518 352127.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T AGU 150HP 06A906018D 0261204254 357459.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T ARZ 150HP 0261206435 352757.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.8T AUQ 180HP 06A906032BJ 0261206892 360288.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI 038906016H.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI 105HP 03G906016J 0281011383 368596.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI 105HP 03G906021AB 389826.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI 110HP 038906012BB 0281010123 350851.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI 90HP 038906012B 0281010121 350849 2802.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI 90HP 038906012C 0281010122 1037350850.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI 90HP 038906018AK 0281001728 357704.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI AGR 90HP 038906018BB 0281001757 358253.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI AHF 110HP 038906012A 0281010120 1037350848.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI AHF 110HP 038906018BP 0281001848.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI AHU 90HP 038906018A 0281001410 355828.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI ASZ 130HP 038906019CK 0281010308 360763.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI ASZ 130HP 038906019CK 0281010308 362845.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI ASZ 130HP 038906019FT 0281010981 363228.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI ASZ 130HP 038906019FT 0281010981 366273.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI BKC 105HP 03G906016CC 0281011832 371093.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 1.9TDI BKD 105HP 03G906016J 0281011383 369261.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0T 8P0907115K 0261S02220 386817.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI 140HP 03G906016G 0281011364 367950.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI 140HP 03G906016G 0281011364 368156.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI 140HP 03G906016G 0281011364 368508.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI 140HP 03G906021AN.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI BKD 03G906016FF 0281011905 371366.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI BKD 140HP 0281011905 371366.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI BKD 140HP 03G906016AT 0281011453 369901.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI BKD 140HP 03G906016FF 0281011905 370634.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI BKD 140HP 03G906016FF 0281011905 375970.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 2.0TDI BKD 140HP 03G906016G 0281011364 369819.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3 BLS 03G906021HP 382669.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A3_1.8TQ_206434_0261206434.ori` | `.ORI` | `199,048` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8 0261204774 8D0907558B 357973.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8 0261204957 8D0907558T 356670.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 150HP 4B0906018P 0261206537 352750.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 150HP 8D0907557 0261203550 355966.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 150HP 8D0907557P 0261204258 350269.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 150HP 8D0907557T 0261204185 1037358703.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 150HP 8D0907557T 0261204185 358761.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 150HP 8D0907559 0261204963 359127.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 150HP 8D0907559C 0261206315 350004.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 150HP 8E0909518M 0261207778 363466.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 163HP 8E0909518AA 0261207934 366381.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 180HP 8E0906018B 0261206868 360990.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 190HP 8E0909518AN 0261208285 368075.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 4B0906018R 0261206539 354735.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 4B0906018R 0261206539 354801.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 8D0907558DA 0261206429 350714.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 8E0909018 0261207435 362521.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 8E0909518AK 0261208230 368072.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T 8E0909518AS 0261208500 369011.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T AEB 150HP 8D0907557 0261203551 355800.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T AJL 8D0907558D 0261204778 358150.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T APU 150HP 4B0906018AR 0261206524 352053.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T AWT 4B0906018CG 0261207215 360306.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T BEX 192HP 8E0909518AH 0261207941 366871.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T BFB 163HP 8E0909518AA 0261207934 366494.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.8T BFB 163HP 8E0909518AL 0281208228 369311.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 100HP 038906019LF 0281011210 366506.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 105HP 03G906016HA 390133.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 110HP 038906012AH 0281010200 1037352636.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 110HP 038906012AH 0281010200 352255.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 110HP 038906012BL 0281010199 352254.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 115HP 0281011887 03G906016CJ 1037371805.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 115HP 03G906016FE 0281012127 390131.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 130HP 038906019F 0281012187 372301.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 130HP 038906019FP 0281010729 362614.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 130HP 038906019FP 0281010729 363740.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 1Z 90HP 028906021F 0281001367 355586.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI 90HP 0281010197 038906012AF 352621.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AFN 110HP 028906021CE 0281001426 355217.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AFN 110HP 028906021CE 0281001426 355304.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AFN 110HP 028906021GN 0281001660 357272.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AFN 110HP 028906021GN 0281001660 357833.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AFN 110HP 038906018S 0281001721 356817.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AFN 110HP 038906018S 0281001721 358381.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AHH 90HP 038906012AJ 0281010202 352257.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AHH 90HP 038906012AJ 0281010202 352625.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AHU 90HP 028906021BD 0281001439 438-439.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AHU 90HP 028906021GM 0281001658 355274.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AHU 90HP 028906021GM 0281001658 357835.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AHU 90HP 038906018R 0281001726 727820.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AJM 115HP 038906019AN 0281010094 354607.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AJM 115HP 038906019BR 0281010226 354265.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AVB 100HP 038906019JP 0281011141 366049 1569.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AVF 130HP 038906019JL 0281011036 363230.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AVF 130HP 038906019JT 0281011138 366048.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AVF 130HP 038906019KA 0281011140 367021.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AVF 130HP 038906019LJ 0281011222 366508.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AVF 130HP 038906019LJ 0281011222 370445.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AWX 130HP 038906019CG 0281010406 362036.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AWX 130HP 038906019FP 0281010729 362705.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 1.9TDI AWX 130HP 038906019GD 0281010844 362628.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 19TDI AFN 110 038906018S 0281001721 357593.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.0TDI 140HP 03G906016JD 0281012654 378340.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.0TDI 140HP 03G906016LR 0281012726 386343.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.0TDI BPW 140 03G906016KN 391503.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.0TDI BPW 140HP 03G906016KN 382430.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.0TDI BRD 170HP 03G906018AQ 5WP4554.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.0TFSI 8E0907115D 0261S02211 386863.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5 TDI 180HP O8E0907401 0281011386 1037367176.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 150HP 0281010152 4B0907401R 1037351651.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 150HP 8D0907401H 0281001834 356764.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 150HP 8D0907401P 0281010158.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 150HP 8D0907401Q 0281010159 351133.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 155HP 4B1907401D 0281010494 351926.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 155HP 8D1907401A 0281010100 352924.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 163HP 8E0907401AF 0281012142 375555.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 163HP 8E0907401S 0281011435 369443.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 163HP E0907401M 0281011255 368106.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 180HP 8E0907401C 0281010493 362493.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 180HP 8E0907401D 0281010823 366614.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 180HP 8E0907401D 0281010823 367154.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI 8E0907401T 0281011444 367801.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI AFB 150HP 8D0907401L 0281010155 145-146.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI AKE 180HP 8E0907401B 0281010446 360545.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI BDG 163HP 8E0907401M 0281011255 369444.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.5TDI V6 150HP 8D0907401D 0281001812 359339.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 2.8 V6 4D0907551F 0261204687 357491.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 3.0TDI 204HP 8E0907401AJ 377113.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 3.0TDI 233HP 8K0907401 0281014014 392914.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 quattro 2.5TDI 180HP 8E0907401C 0281010493 362493.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A4 tdi 155ps orig.dat.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Audi A4_D1900_R4V2T_66kW_0281010065_038906018FF_2150_xx167_168_crc9DA33691.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.8T 150HP 4B0906018DC 0261207636 362358.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.8T AEB 150HP 4B0907557A 0261204256 357473.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.8T AND 150HP 4B0906018L 0261206320 350703.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.9 TDI 038906018DG 0281001808 356001.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.9TDI 115HP 03G906016JA 0281012723 1037377587.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.9TDI 130HP 038906019CF 0281010405 362175.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.9TDI AFN 110HP 038906012AB 281010203 352258.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.9TDI AJM 115HP 038906019BS 0281010224 360072.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.9TDI AVF 130HP 038906019HM 0281011046 367002.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 1.9TDI AVF 130HP 038906019LM 0281011213 367408.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.0TDI 136HP 03G906016HQ 0281012555 383820.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.0TDI 140HP 03G906016BF_382716.BIN` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Audi A6 2.0TDI 140HP 03G906016GB 0281012112 383724.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.0TDI 140HP 03G906016MG 393553.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.2T AAN 230HP 4A0907551D 0261203603 358374.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.4 V6 177HP 3B0907552J 0261206122 350079.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5L 103kw 0281001478-2537355737.std` | `.STD` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi A6 2.5L 103kw 0281001478-2537355738.std` | `.STD` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (STD) |
| `Audi A6 2.5TDI 140HP 0281001321 355498.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 140HP 4A0907401F 0281001255 358724.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 150HP 0281010156 8D0907401M.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 150HP 4B0907401C 0281001836 359393.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 150HP 4B0907401H 0281001781 357690.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 150HP 4B0907401J 0281001772 357667.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 150HP 4B0907401Q 0281010151 1037352649.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 150HP 4B0907401R 0281010152 1037351323.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 150HP 4B1907401A 0281010095 354255.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 150HP 8D0907401N 0281010157 351050.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 163HP  0281011255 8E0907401M 370841.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 163HP 8E0907401M 0281011255 367774.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 163HP 8E0907401P 0281011136 366619.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 163HP 8E0907401Q 0281011135 366644.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 4B2907401 0281010096 037354665.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 4B2907401 0281010096 350319.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 4B2907401 0281010096 354337.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 4B2907401B 0281010098 354335.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 4B2907401F 0281010443 362485.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 4B2907401J 0281010822 362761.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 4B2907401J 0281010822 367153.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 4Z7907401A 0281010445 362124.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 8E0907401J 0281011387 367568.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 8E0907401J 0281011387 367927.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP 8E0907401N 0281011386 369512.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 180HP allroad 4Z7907401A 0281010445 354376.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI 4B0907401K 0281001931 350601.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI AEL 140HP 4A0907401P 0281001321 355245.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI AEL 140HP 4A0907401P 0281001321 355246.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI AFB 150HP 4B0907401AC 0281010399 351313.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI AFB 150HP 4B0907401S 0281010148 351032.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI AKE 180HP 4B2907401D 0281010395 354333.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI AKE 4B2907401J 0281010822 366611.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI AYM 155HP 4B1907401D 0281010494 363776.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI-180HP-AKE-0281010822-4B2907401J-1037363777.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI-4B2907401E-0281010394-1037354332.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.5TDI-4B2907401E-0281010394-1037360719 .ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.6 ABC 150HP4 A0907473D.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.7 TDI  180hp 0281012560 4F0907401B 7377319.orig.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.7T 265HP 4B0907551F 0261206378 350239.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.7T AJK 230HP 4B0907551G 0261206380 354065.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.7TDI 163HP 4F0907401B 4F2910401S 377107.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 2.7TDI 180HP 4F2910401R 377106.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 233HP 4F0910402E 381388.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 233HP 4F9910401L 389130.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 3.0TDI 224HP 4F0907401B 1037374416.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 3.0TDI 4F0907401A 0281011569 371077.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 3.0TDI 4F0907401A 372123.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 3.0TDI 4F0910401F 371077.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 4.2 V8 4D0907558S 0261206204 352486.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 4.2i 4D0907560AE 0261206843 354728.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 C4 2.5TDI 140HP 0281001321 355329.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 allroad 2.5TDI 180HP 4Z7907401B 0281010897 366613.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 allroad 2.5TDI AKE 180HP 4Z7907401A 0281010445 362124.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 allroad 2.7T 263HP 4Z7907551N 0261207766 366367.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 allroad 2.7T 265HP 4Z7907551D 0261207137 354846.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6 allroad 2.7T BEL 250HP 4Z7907551R.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A6-TDI 2,0 BLB-03G906016GN-0281012113-376101.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 2.5TDI 150HP 4D0907401G 0281001773 093.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 2.5TDI 180HP 4D2907401 0281010160 354334.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 2.5TDI 180HP 4D2907401 0281010160 354666.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 2.5TDI AFB 150HP 4D0907401N 0281010397 351308.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 3.3TDI 225HP 4D0907409C 0281010900 1037351707.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 3.3TDI AKF 224HP 4D0907409A 0281001867 351497.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 4.2 V8 380HP 4D0907557G 0261204205 355159.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 4.2 V8 4D0907557B 0261203300 358194.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8 6.0-450HP-4E0906018-0261208203-370953.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi A8_4.2_368674_208493_4E0910560K.ori` | `.ORI` | `376,621` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi Q5 2.0TDI 170HP 03L906022B 03L906022Q 500144.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi Q7 3.0TDI 4L0907401 390614.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi Q7 4.2TDI 326HP 4E1907409B 0281013013.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi R8_0 261 S02 234_1037390288_MED91_4.2L V8 ori.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Audi RS4 2.7T 380HP 8D0907551Q 0261207141 360388.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi RS4 2.7T 8D0907551F 0261206635 354531.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi RS4 4.2FSI 8E1907560 0261S02165 379578.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi RS6+ 4D1907558F 0261208728 373709.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S2 2.2 ABH 220HP 0261203143 357360.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 (8L) 1.8 BAM-8N0906018BH-0261207751-1037362999.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 (8L) 1.8-AMK-8N0906018CH-0261208269-367511.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 1.8T 210HP 8L0906018K 0261206442 352377.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 1.8T 210HP 8L0906018K 0261206442 352465.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 1.8T 210HP 8N0906018J 0261206794 360284.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 1.8T 210HP 8N0906018J 0261206794 360314.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 1.8T 210HP AMK 8N0906018AG 0261207213 360320.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 1.8T APY 210HP 8L0906018N 0261206796 352820.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 2.0TFSI 265HP 8P0907115H 0261S02342 384214.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 210HP 8L0906018N 0261206796 354092.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S3 225HP 8N0906018BP 0261208054 366474.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.2T 260HP 4A0907551A 0261200465 356703.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.2T 260HP 4A0907551AA 0261200465 356711.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.2T 260HP 4A0907551AA 0261200465 357248.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.2T 260HP 4A0907551AA 0261200465 357391.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.2T AAN 230HP 4A0907551B 0261203005 357249.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.7 8D0907551G 0261206776 360855.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.7T 250HP 8D0907551D 0261206382 350243.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.7T 265HP 8D0907551A 0261206110 352345.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.7T 265HP 8D0907551A 0261206110 352741.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.7T 265HP 8D0907551L 0261207004 354145.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 2.7T 265HP 8DO907551C 0261206108 350093.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S4 4.2i 8E0907560H 0261208776 1037374035.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S5 4.2 V8 8T0907560 0261S02329 390268.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S6 4.2 V8 290HP 4A0907557B 0261203645 358378.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S6 4.2 V8 290HP 4A0907557C 0261203599 355858.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S8 4.2 V8 4D0907557N 0261204563 358953.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi S8 4.2i 360HP 4D0907559G  0261206096 352379.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT  1.8TFSI 160PS 0261201948 1037398687 ORI.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Audi TT 1.8 225HP 8N0906018F 0261206105 356615.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 150HP 8D0907557T 0261204185 357482.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 180HP 8N0906018AB 0261207027 354503.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 180HP 8N0906018AQ 0261207416 363478.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 180HP 8N0906018BR 0261208005 363675.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 180HP 8N0906018Q 0261206439 354510.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 225HP 8L0906018M 0261206797 352821.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 225HP 8L0906018M 0261206797 354094.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 225HP 8N0906018AN 0261207418 362588.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 225HP 8N0906018T 0261206228 354508.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T 8N0906018BR 0261208005 369398.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T AJQ 180HP 8N0906018A 0261204898 359559.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T AJQ 180HP 8N0906018B 0261204962 350294.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T APX 225HP 8N0906018AE 0261207030 354178.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T AUQ 180HP 8L0906018Q 0261206790 360287.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T AUQ 8L0906018Q 0261206790 354029.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TT 1.8T BAM 225HP 8N0906018H 0261206795 360313.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi TTS 2.0TFSI 272HP 8J0907115Q  0261S02581 393740.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi a2 1,4 tdi 497.mod` | `.MOD` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (MOD) |
| `Audi a3 1.9TDI AFN 110HP 038906018BA 0281001756 357284.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi a3 1.9TDI AHF 110HP 038906018AJ 0281001694 357590.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi a3 19TDI AGR 90HP 0281001693 0381001693 357319.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi a3 19TDI AGR 90HP 038906018AH 0281001693 357791.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi a4 1.9TDI AFN 110HP 028906021EA 0281001490 355111.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi a4 quattro 1.9TDI AFN 110HP 028906021EM 0281001554 355538.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_200_B2200_R5V4T_162kW_0261200451_447907404AA_xxx_1267356260_crcF50660DA.ori` | `.ORI` | `8,192` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_200_B2200_R5V4T_162kW_0261200451_447907404AA_xxx_1267356462_crc0AE3CACD.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_200_B2200_R5V4T_162kW_0261200451_447907404A_xxx_1267356259_crcE66098C8.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001133_8A0907401A_D06_2287357598.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001133_8A0907401A_D06_2287357599.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001186_8A0907401B_D09_2287357913_crc94FCAED3.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001186_8A0907401B_D09_2287357914_crc0E0D2C00.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001198_028906021D_D21_2287358771_crc1DA0C54E.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001222_028906021E_D56_2287358725_crcD444EC2E.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001222_028906021E_D56_2287358726_crcD444EC2E.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001330_028906021AR_D63_2287357893_crc69802A17.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001330_028906021AR_D63_2287357894_crc841064DB.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_80_D1900_R4V2T_66kW_0281001568_028906021FD_KD04_1037358669_670_crc8A7DA418.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A3_1_9l_TDI_PD_Bosch_EDC_16U1.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Audi_A3_B1800_R4V5T_165kW_0261206438_06A906032R_0002_1037352355_crc9C3CED82.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Audi_A3_D1900_R42VT_96kW_0281010308_038906019CK_1243_1037360044_crc33B3CFFC.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A3_D1900_R42VT_96kW_0281010561_038906019EF_1331_1037360585_crc3ED18F25.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A3_D1900_R4V2T_96kW_0281001308_038906019CK_1243_1037360044_crcF03BD0AF.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A3_D1900_R4V2T_96kW_0281010308_038906019CK_1477_1037362845_crc97223402.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A3_D1900_R4V2T_96kW_0281010981_038906019FT_1577_1037366273_crc9881DFF6.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A3_D2000_R4V4T_103kW_0281011450_03G906016AL_5249_1037368223_crcCFBDEB5B.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A4_B1800_R4V5T_110kW_0261207854_8E0909518P_0001_1037363386_crc087E0E4B.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A4_D1900_ATJ_R4V2T_85kW_0281010094_038906019AN_1063_1037354264.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A6_AAT_0281001254_1037355048.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A6_AAT_0281001254_1037355049.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_A6_TDI_150PS_0281010005_8D1907401_354256_.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Audi_Org_A4_TDI.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Audi_Q7_TDI_V6_30_235_383721_4L0910401M_0030.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `B4 Passat - GQ - 357270 - LLL683 8.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `B4 Passat - GQ - 357271 - HHH683 8.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Caddy_1_9_TDI_PD_105PS_03G906021HS_381007.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `E2PROM.bin` | `.BIN` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Eeprom.bin` | `.BIN` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `G3-s827.564.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `G3-s828.564.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `GTI325P.FST.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Golf 3 90PS 0 261 203 593-594 original.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Golf7045.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `HHH 0281001650_028906021GG_1443.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `HHH 028906021DF_0801.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `HHH_868_ Orig.BIN` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `IAW 4MV.DR 036906034DR golf 4 1.6 .ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `KD35.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `LLL 0281001650_028906021GG_1443.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `LLL 028906021DF_0801.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `LLL_867_ Orig.BIN` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `MPC555.bin` | `.BIN` | `238,314` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `MPC555_1.bin` | `.BIN` | `237,712` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `OriginalAudi706B.833.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `OriginalAudi707B.833.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `PassatPd130.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Proc.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Q 7 full.bin` | `.BIN` | `773,215` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Sander_AUDI_TT_2001_224hp_Q.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `T4 AMV 022906032B_0261206239_354081.Bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Tiguan_2.0TDi_CR_EDC17_3L906022G_sw106.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VOLKSWAGEN POLO 1300 1267356773 0261200306 27C256 E0D4.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW  NEW BEETLE 1.9TDI 100HP 0281011539 038906019KR 368191.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW 1.6i 06A906033L 5WP4004.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW 1.8T G60 Digifant 037997022B - WINOLS.ols` | `.OLS` | `59,105` bytes | ECU Parameter Definition Map (OLS) |
| `VW 2.0TDI CFGB 170HP EDC17C46 03L907309R 03L906018BC 1037524625 9784.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Beetle 1.8T 0261207341 06A906032FT 362333.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Beetle 1.9TDI 5spd ALH 90HP 038906012GQ 0281011035 366235.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Beetle 1.9TDI auto 038906012FF 0281001655 362776.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Bora 1.8T-150HP-06A906032DR-0261206887-1037360128.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Caddy 1.9TDI 105HP 03G906021PD 389297.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Caddy2 1.9TDI BJB 105HP 03G906016DM 0281011882 371251.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Crafter 2.5 TDI  074906032BB 503934.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Crafter EDC16CP34 BDM 0281014133 1037386337.ori` | `.ORI` | `458,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW GOLF 1.9-100hp-0281011065-1037363709.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW GOLF3 1.8-90hp-0261200784-1H0907311H.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Golf 150PS 1.8L R45VT-06A906018R-0261204673-358109.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Golf 2.3 V5 AGZ 150hp 071906018 0261204753 359144.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Golf 5 1.9TDI BKC 105HP 03G906016CB 0281011900 371429.ori` | `.ORI` | `1,511,680` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Golf 5 3.2 VR6 260HP 022906032CE 0261208468 377419.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Golf IV ALH 90hp 038906012FA 0281010650 360773.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Golf VII GTI 2.0TFSI Simos18.1 5G0906259 0005 SC800F8300000.ori` | `.ORI` | `4,718,592` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Golf4 1.8T 0261206518 352127.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Golf4 1.8T 06A906032DL 0261206890 354821 Original.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Golf4 1.9 TDI 90hp ALH 0281001979 038906012M 2813.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Golf4-(1J)-1,9-AGR-90HP-038906018D-0281001611.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Golf5 1.9TDI 105HP 0281012220 03G906016R 374183.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Golf5 1.9TDI 105HP 03G906021KH 0281013226 382083.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW GolfV (1K) TDI 1,9 BKC-105hp-03G906016CB-0281011900-371094.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW LT 2.5TDI 109HP 074906021AG 0281010088 893HHH.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW LT 2.5TDI 109HP 074906021AG 0281010088 893LLL.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW LT 2.5TDI AHD 102HP 074906021AK 0281010086.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW LT 2.5TDI AHD 102HP 074906021J 0281001600 358946.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW LT35 2.5TDI AVR 109HP 074906018BK 0281011385 367887.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW LT35 2.8TDI 158HP 2D0906019A 0281010588 365048.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW LT35 TDI 889 021AP HHH Original.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW LT35 TDI 889 021AP LLL Original.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Lupo 1.4l 16V 100HP 036906034AT IAW4LV.VA 61600.540.05.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW PAssat 2.0 140PS 0281012119 394115.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW PAssat 2.0 CR 140HP  03L906022BL 4145 399883.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW PAssat 2.0 CR 140HP 03L906022BL 6221 507677.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW POLO GTI 110KW_0261 201 628_1037 38 2997.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat  1.9TDI 105HP 3G906021LR 380420.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 1.8T  4B0 906 018 DF  AWT ME7.5 0261207639 original.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Passat 1.8T 8D0907558E 0261204805 358123.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Passat 1.9TDI 105HP 03G906021AB 381562.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 1.9TDI 105HP 03G906021NK 382417.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0 TDI BHW 136HP 038906016R 0281011982 371877.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0FSI 150HP 06F906056AN 0261S02135 376502.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0TDI  170HP 3L906022BM 396091.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0TDI 140HP  03G906021AB 03G906021MT 382427.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0TDI 140HP 0281012925_03G906021AD_378328.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0TDI 140HP 03G906018CD 9627.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0TDI 140HP 03G906021AB 03G906021NK 399388.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0TDI 140HP 03G906021NK 1037394904.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0TDI 170HP PPD 03G906018ER.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.0TDI BKP 140.0PS 03G906018CD  SN000F7600000.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Passat 2.3 V5 0261206508 071906018AC 352012.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 2.3 V5 906018AE 0261206620.ORI` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 3.6 FSI 03H906032C  0261S02169 376323 FSI.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Passat 3C 19 105ps BKC 0281012085 03G906021AN 374452.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Passat V8 4.0 BDN 07D906018C 0261207019 366337.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Phaeton 3.2V6 AYT 241HP 022906032BN 0261207688 366305.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Polo 1.7 SDI 44kW 038906013K 0281001749 1808 HHH.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Polo 1.7 SDI 44kW 038906013K 0281001749 1808 LLL.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW T4 2.5TDI 102HP 038906018AM 0281010458 360078.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T4 2.5TDI 102HP 074906018AH 0281010681 362448.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T4 2.5TDI 102HP 074906018AL 0281010459 360077.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T4 2.5TDI 88HP 074906018AK 0281010462 360076.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T4 2.5TDI 88HP 074906018B 0281010084.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T4 2.5TDI ACV 102HP 074906018C 0281010082.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T4 2.5TDI ACV 102HP 074906021L 0281001640 357796.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T5 2.5TDI 130HP 070997016C 0281012931 1037378311.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T5 2.5TDI 130HP 070997016M 390979.e2p` | `.E2P` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (E2P) |
| `VW T5 2.5TDI 130HP 070997016M 390979.mpc` | `.MPC` | `257,857` bytes | Raw OEM Factory Binary / Hardware Read (MPC) |
| `VW T5 2.5TDI 130HP 070997016M 390979.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T5 2.5TDI 174HP  070906016BA 0281011664 372365.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T5 2.5TDI 174HP  070906016EB 0281014892 1037394113.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T5 2.5TDI 174HP 070906016BD 0281011835 372944.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW T5 2.5TDI BNZ 130.0PS 070906016EC  394114.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Tiguan 2.0 170 HP 03L906022G 395496.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Tiguan 2.0TDI 03L906022G 396096 edc17p14.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touareg 2.5TDI BAC 174HP 070997016E 0281012926 381353.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touareg 3.0l TDI 0281013686 7L0907401D 386372.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touareg 4.2V8 AXQ 310hp 4D0907560BR 0261208009 367701.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touareg 5.0V10TDI AYH 313hp 070906016AA 0281011481 368703.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Touareg 5.0V10TDI AYH 313hp 070906016D 0281010736 367461.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Touran  2.0TDI 140HP  0281011907 03G906016FK 371267.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 1.9TDI 105HP 0281012361  03G906016HP 374119.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 1.9TDI 105HP 03G906021AB 03G906021MG 383708.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 1.9TDI 105HP 03G906021AN 03G906021KC 382090.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 1.9TDI 105HP 03G906021HK 394990.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 1.9TDI 105HP 03G906021ND 396444.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 1.9TDI AVQ 105HP 03G906016A 0281010731 368159.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 2.0SDI 0281012272 03G906016HN 376308.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 2.0TDI 140HP 03G906021AB 03G906021MJ 383709.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 2.0TDI 140HP 03G906021GB 378847.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Touran 2.0TDI 140HP 03G906021KF 381020.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Transporter 2.5TDI AXD 131HP 070906016AJ 0281011568 372363.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Transporter T5 1.9PD 85HP 0389060106AH 1037381380.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Transporter T5 1.9TDI 105HP   038906016AJ 390638.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Transporter T5 1.9TDI 74KW  0281012761 038906016T 384631.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW Tuareg 3.0L BKS 7L0907401F  0281013686.bin` | `.BIN` | `787,075` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW Tuareg 3.0L BKS 7L0907401F  0281013692.bin` | `.BIN` | `786,480` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW beetle 1.8T 150HP 06A906032GQ 0261207349 360345.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW beetle 1.9TDI 100HP 038906019MT 0281011413 367412.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW beetle 1.9TDI 100HP 038906019NN 0281011391 368225.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW beetle 1.9TDI ALH 90HP 038906012FH 0281010657 362437.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW beetle 1.9TDI ALH 90HP 038906012Q 0281010133 352571.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW beetle 1.9TDI ALH 90HP 038906018AP 0281001732 357743.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW beetle 1.9TDI ALH 90HP 038906018M 0281001696 356243.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW bora 1.6 BFQ 06A906033BN 5WP4019 4667.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW bora 1.6i 06A906033AQ 5WP4013.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW bora 1.8T 180HP 06A906032SL 0261208529 371155.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW bora 1.9TDI 115HP 038906019H 0281001910 350172.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW bora 1.9TDI AGR 90HP 038906012FD 0281010653 362774.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW bora 2.0 APK 06A906018FK 0261206261 485757.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW caddy 1.9SDI 03G906016GP 0281012168 372600.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW caddy 1.9SDI 68HP 038906012GJ 0281010965 363111.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW caddy 1.9TDI 105HP 03G906021AQ 0281012390 377585.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW caddy 1.9TDI 105HP 03G906021CG 0281012746 393550.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW caddy 2.0SDI 75HP 0281011541 03G906016N 369948.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW corrado 1.8T PG G60 160HP 037906022B.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW corrado 2.9i VR6 ABV 021906258AG 0261203109 357531.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW crafter 2.5TDI  0281014133 074906032AT 10373386337.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW crafter 2.5TDI 074906032AG 1037383306.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW crafter 2.5TDI 074906032E  0281012543 381010.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW eos  2.0TDI 140HP DPF 03G906021AB 383799.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.4i AXP 036906032P 0261207179 354828.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.6i 06A906033AF 5WP4013.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.6i 06A906033BN 5WP4015.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.8 AGN 130HP 06A906018CL 0261206076 359100.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.8T  06A906032LQ 0261207956 367519.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.8T 150HP 06A906018R 0261204673 359591.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.8T 150HP 06A906032AR 0261206436 1037352758.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.8T ARZ 150HP 06A906032AR 0261206436 352357.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.8T AWV 150HP 06A906032SK 0261208528 371152.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9 110HP 028906021JG 0281001860 356933.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9SDI 68HP 038906012DB 0281010373 354379.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9SDI 68HP 038906013 0281001759 356428.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 028906021ED 0281001541 357815.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 105HP 03G906016B 0281011478 375902.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 105HP 03G906021AB 391847.ori` | `.ORI` | `2,097,154` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 105HP 03G906021AN 382414.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 105HP 03G906021AN 389140.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 105HP 03G906021KH 0281013226 380437.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 105HP 03G906021KH 380437.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 1Z 90HP 028906021BF 0281001422 355103.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 90HP 038906018GR 0281010245 352615.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 90HP 038906018GR 0281010245 352616.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 90HP 03G906016FS 0281011955 370811.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI 90HP ALH 038906018AE 0281001851.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI AFN 110HP 028906021GT 0281001735.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI AGR 90HP 038906018BL 0281001845 359499.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI AHF 110 HP 038906018GP 0281010246 350618.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI AHU 90HP 028906021GG 0281001650 357824.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI AJM 115HP 038906019FC 0281010751 362699.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ALE 90HP 028906021HD 0281001729 357948.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ALH 90HP 038906012CP 0281010385 354327.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ALH 90HP 038906012GK 0281010864 362681.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ARL 150HP 038906019AQ 0281010048 1037360004.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ARL 150HP 038906019FE 0281010744 362470.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ARL 150HP 038906019FE 0281010744 362684.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ARL 150HP 038906019HH 0281010976 363171.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ARL 150HP 038906019HH 0281010976 366661.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ASZ 130HP 038906019HJ 0281010977 363142.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ASZ 130HP 038906019KJ 0281011216 368577.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ATD 100HP 038906019AT 0281010974 366203.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ATD 100HP 038906019CR 0281010663 362817.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI ATD 100HP 038906019FF 0281010662 362734.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI AUY 115HP 038906019AM 0281010091 350875.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI AXR 100HP 038906019KP 0281011191 366912.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI BKC 105HP 03G906016B 0281011478 368926.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 1.9TDI BKC 105HP 03G906016B 0281011478 369564.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0 TFSI 200HP 1K0907115F 0261S02217 377837.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0GTI 037906024D FALA03001390.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TDI 140HP 03G906016AN 0281011477 368925.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TDI 140HP 03G906016HJ 0281012253 372673.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TDI 140HP 03G906021PP 1037389263 1264.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TDI 140HP 03G906021PR 1037387083.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TDI 170HP 03G906018FB.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TDI BKD 140HP 03G906021KK 0281013228 1037381019.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TFSI 1K0907115 0261S02078 387570.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TFSI 200HP 1K0907115 0261S02078  377862.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TFSI 200HP 1K0907115 0261S02078 372620.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.0TFSI 200HP 1K0907115J 0261S02331 386464.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.8 VR6 021906258CL 0261203559 358929.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.8 VR6 AAA 021906258A 0261200496 357205.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 2.8V6 174HP 021906018R 0261206814 360624.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 3 1.9SDI 028906021FJ 0281001560 781-782.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 3 1.9TDI 90HP 028906021C 0281001171.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 3 1.9TDI 90HP 028906021HG 0281001730 357946.ORI` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 3 1.9TDI AFN 110HP 028906021GH 0281001652 358905.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 3 2.8 VR6 174HP 021906258CH 0261203569 358928.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 3 2.8V6 174HP 021906256 0261203969 559385.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 3 VR6 2.8 174HP 0261203117 021906258AF 357529.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 3.2 VR6 250HP 022906032EG 0261208344 373693.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 4 1.6 06A906019AK 5WP4417 (1B6F).ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 4 1.6 5WP4448.03 (7001).ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 4 1.6 5WP4872.03 (2704).ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 4 1.9TDI 130HP 038906019FG 0281010702 362796.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 4 1.9TDI AHF 110HP 038906012L 0281010112 352566.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 4 1.9TDI AWX 130HP 038906019JQ 0281011142 366047.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 4 16 5WP4426.02 (6A4E).ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 5 1.9SDI 0281011617 03G906016M 370652.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 5 1.9SDI 69HP 03G906016GJ 0281012221 372340.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 5 1.9TDI 038906016H 0281011146 371297.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 5 2.0TDI 140HP 03G906016ET 0281011843 375890.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 5 2.0TFSI 200HP 1K0907115 0261S02078 374094.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf 5 R32 022906032CD 0261208467 377452.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf IV 1.9TDI AHF 110HP 038906018J 0281001613.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf IV 1.9TDI AJM 115HP 038906019CJ 0281010302 352930.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf IV 1.9TDI ARL 150HP 038906019FE 0281010744 362706.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf IV 1.9TDI ASV 110HP 038906012AP 0281010126 352577.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf V 2.0TDI 140HP DPF 03G906021JG 394134.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf4 AHF 110hp 038906018BM 0281001846 356590.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf4 ALH 90HP 038906012M 0281001979 352564.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf4 ALH P0HP 038906018AN 0281001733.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf5 2.0TFSI 1K0907115K 0261S02332 380991.ori` | `.ORI` | `2,099,200` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW golf5 2.0TFSI DSG 1K0907115E 0261S02082 387576.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW industrial engine 1.9TDI AFD 82HP 028906021JQ 0281010266.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW jetta 1.8T AWD 150HP 06A906032CL 0261206552 1037354128.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW jetta 2.0TDI CBEA 03L906022KS 397837.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW jetta 2.8 VR6 021906018M 0261206486 352765.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW lupo 1.2TDI 61HP 045906019Q 0281010258 1037352679.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW lupo 1.2TDI 61HP 045906019Q 0281010258 352999.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW lupo 1.4TDI 75HP 045906019L 0281010049 352592.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW lupo 3L 1.2TDI 61HP 0281010015 045906019K 1211 354603.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW lupo 3L 1.2TDI 61HP 0281010505 045906019AA 1313 360520.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW lupo 3L 1.2TDI 61HP 0281010628 045906019AE 1508 351992.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW lupo 3L 1.2TDI 61HP 0281010628 045906019AE 1537 363567.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW pasat 2.5TDI 150HP 3B1907401F 0281010444 354375.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.8T 150HP 4B0906018AG 0261206453 352151.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.8T 163HP 8E0909018A 0261207928 366497.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.8T 4B0906018CC 0261206871 354009.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.8T ADR 8D0907558S 0261204956 356669.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.8T ANB 150HP 4B0906018BF 0261206525 352710.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.8T APU 150HP 4B0906018B 0261206050 350229.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.8i APT 125HP 8D0906018F 0261204875 350087.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 100HP 038906019BM 0281010307 1037360022.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 100HP 038906019BM 0281010307 1037360476.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 115HP 038906019AJ 0281010303 352975.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 130HP 038906019EP 0281010701 362631.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 130HP 038906019EQ 0281010700 362632.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 1Z 90HP 0281001328 355573.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 1Z 90HP 0281001328 355574.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 1Z 90HP 028906021AT 0281001369 355101.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI 90HP 038906018FG 0281010063 350164.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AFN 110HP 028906021GL 0281001656 357830.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AFN 110HP 038906018FE 0281010064.bin` | `.BIN` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW passat 1.9TDI AFN 110HP 038906018GA 0281010170 920.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AFN 110HP 038906018P 0281001720 356815.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AFN 110HP 038906018P 0281001720 358385.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AHH 90HP 038906018AS 0281001724 359461.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AHU 028906021EG 0281001558 355806.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AHU 90HP 028906021GG 0281001650 357824.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AHU 90HP 028906021GK 0281001654 357832.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AHU 90HP 028906021GK 0281001654.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AHU 90HP 038906018FQ 0281001172 350924.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AJM 115HP 038906019A 0281001691 350100.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AJM 115HP 038906019AJ 0281010303 354614.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AJM 115HP 038906019BJ 0281010176 350953.ori` | `.ORI` | `524,290` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AJM 115HP 038906019BK 0281010305 352976.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AJM 115HP 038906019CD 0281010218 352904.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI ARL 130HP 038906019KE 0281011201 366297.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI ATJ 115HP 038906019DM 0281010470 354455.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVB 100 HP 038906019EJ 0281010665 362053.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVB 100HP 038906019EB 0281010553 360009.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVB 100HP 038906019EK 0281010667 362051.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVB 100HP 038906019GK 0281010943 362893.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVB 100HP 038906019GL 0281010944 362894.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVB 115HP 038906019EA 0281010554 360477.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVF 130HP 038906019BN 0281010404 360707.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVF 130HP 038906019DS 0281010543 360449.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVF 130HP 038906019DS 0281010543 360705.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVF 130HP 038906019EN 0281010705 362633.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVF 130HP 038906019GQ 0281010941 363213.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AVF 130HP 038906019KD 0281011205 366501.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AWX 130HP 038906019EH 0281010558 360706.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AWX 130HP 038906019ER 0281010704 362704.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI AWX 130HP 038906019GS 0281010940 366946.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI BKC 105HP 03G906021DP 0281012724 1037377575.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 1.9TDI PD 130HP 038906019GS 0281010940 363212.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 2.0TD 140HP 03G906018 9722.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 2.0TDI 140HP 038906016K 0281011145 372127.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW passat 2.5 AVB 150HP 3B1907401B 0281010447 360452.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 2.5TDI 150HP 3B0907401H 0281010145 351026.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 2.5TDI 150HP 3B1907401B  0281010447 366617.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 2.5TDI 150HP 3B1907401B 0281010447 366617.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 2.5TDI AFB 150HP 3B0907401 0281001938 359796.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW passat 2.5TDI AFB 150HP 3B0907401G 0281010146 027-028.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.4TDI 75HP 045906019BF 0281011241 368175.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.4TDI AMF 75HP 045906019AB 0281010503 354620.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.4TDI AMF 75HP 045906019AP 0281010865 363954.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.9SDI 64HP 038906012AR 0281010109 350846.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.9SDI 74HP 038906012HL 0281011319 367056.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.9TDI ALH 90HP 038906018ED 0281001915 356955.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.9TDI ATD 110HP 038906019JK 0281011075 363985.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.9TDI AXR 100HP 038906019NC 0281011819 371274.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW polo 1.9TDI AXR 100HP 03890619JM 0281011029 363220.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 1.9TDI 1Z 90HP 028906021ES 0281001531 357820.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 1.9TDI AJM 115HP 038906019FC 0281010751 362766.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 1.9TDI AJM 115HP 038906019FC 0281010751 363162.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 1.9TDI AJM 130HP 038906019FC 0281010751 363953.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 1.9TDI ANU 90HP 038906019AB 0281001865 354276.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 1.9TDI ARL 150HP 038906019NQ 0281012287 372714.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 1.9TDI ASZ 130HP 0281011199 69546.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 1.9TDI AUY 115HP 038906019LQ 0281011144 366943.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW sharan 2.8V6 174HP021906256Q 0261203665 355640.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touareg 2.5TDI 174HP 070997016E 387080.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touareg 2.5TDI BAC 174HP 070906016BL 0281011859 371909.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touareg 3.0TDI 8E0907401AB 7L0907401 0281011960 374592.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touareg 5.0TDI 313HP 070906016D 0281010736 368400.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touran 1.9TDI 105HP 0281011945 03G906016CD 371097.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touran 1.9TDI 105HP 03G906021AN 383726.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touran 1.9TDI AVQ 105HP 0281011761 37600.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touran 2.0TDI 140HP 03G906016EH 0281011786 375893.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touran 2.0TDI 170HP PPD 03G906018EH 0498.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touran 2.0TDI BKD 140HP 03G906016BQ 0281011906 371266 SW6254.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW touran 2.0TDI BKD 140HP 03G906016BQ 0281011906 391561.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW transporter 1.9TDI 85HP 038906016 0281010734 368205.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI 102HP 074906018BG 0281010631 362439.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI 102HP 074906021A 0281001306 865.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI 130HP 070906016A 0281010733 368186.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI 130HP 070997016M 1037394151.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI 174HP 0281011271 372941.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI 174HP 070906016A 0281010733 368413.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI 174HP 070906016BF 0281011837 372367.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI AHY 150HP 074906018AN 0281010490 354499.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI AJT 87HP 074906018 0281010462 362446.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.5TDI AXE 174HP 070906016A 0281010733 370230.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW transporter 2.8i AES 021906256H 0261203971 355227.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW-Caddy-1_9TDI-03G906021PF-AB.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW-golf-AHU-90hp-028906021JB-1037358314-lll778.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW-golf-AHU-90hp-028906021JB-1037358315-hhh778.BIN` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VWTransporterT4-4592443.ORI` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Audi_115_Cv._0281010176_1037350953.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Bora_D1900_R4V2T_96kW_0281010702_038906019FG_1420_1037362471_crc69AA584A.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Bora_D1900_R4V2T_96kW_0281010702_038906019FG_1470_1037362796_crcBE32A56A.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Golf3_D1900_R4V2_47kW_0281001408_028906021CQ_D7X_2537355973_crc9938199D.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Golf3_D1900_R4V2_47kW_0281001408_028906021CQ_D7X_2537355974_crcD85057C8.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Golf4_D1900_R4V2T_74KW_0281010662_038906019FF_1355_1037362018_CRC1A832F65.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Golf4_D1900_R4V2T_74kW_0281010497_038906019DF_1237_1037360018_crc896A38D2.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Golf_GT_1,4TSI_170PS_0261201770_03C906032C_500422_.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Golf_MK3_2.0_ABA_115hp_0261203720_1037355532.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW_Golf_MK3_2.0_ABA_115hp_0261204634_1037358768.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW_Jetta_IV_1_9l_TDI_PD_Bosch_EDC_16U34.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW_Passat_(B5)_1_8l_Turbo_Bosch_ME_7_5.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW_Passat_1.9Tdi_66kW_0281001727_038906018N_1615_1037357703.ols` | `.OLS` | `558,160` bytes | ECU Parameter Definition Map (OLS) |
| `VW_Passat_130PSPD_0281010705_038906019EN_362701_1463.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Passat_D1900_R4V2T_66kW_0281001727_038906018N_1615_1037357703_crcF4227CA9.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Passat_D1900_R4V2T_81kW_0281010170_038906018GA_3102_1037354238_239_crcCD39720D.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Passat_D2500_V6V4T_132kW_0281011387_8E0907401J_0004_1037367775_crc81E4BFE5.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Passat_v6_2.5tdi_0281010147__HHH.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW_Passat_v6_2.5tdi_0281010147__LLL.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW_Sharan_D1900_R4V2T_85kW_0281010216_038906019J_1254_1037360085_crc6DEB4AE4.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Sharan_D1900_R4V2T_85kW_0281011144_038906019LQ_1594_1037366943_crc428A525A.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_T4_D2500_R5V2T_111kW_0281010078_074906018N_2529_1037352548_crc0741FC58.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_T4_D2500_R5V2T_111kW_0281010079_074906018D_2531_1037352222_crcCC55EE0E.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_T4_D2500_R5V2T_111kW_0281010461_074906018AJ_3323_1037360079_crc7E14F711.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_T4_D2500_R5V2T_111kW_0281010461_074906018AJ_3908_1037362445_crc6C2E0DDC.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VW_Touareg_3_0l_TDI_V6_Bosch_EDC_16CP_386372.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `VW_Touareg_D5000_V10V4T_230kW_0281010736_070906016D_4939_367325_crc698F0982.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `VWbo18t890stock.BIN` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Vw Caddy 19Tdi  105HP 03G906021_0281012469.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Vw Touareg V6 3.2L 4 Motion Aut 2004 022906032FT-0261208619-1037371624.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Vw passat 1.9TDI 105HP 03G906021AN_03G906021LR 382088.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Vw sharan 2.8LV6 174HP 021906256Q 0261203665 355640.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Vw touareg V6 3.2L 4Motion 022906032BF 0261207566 1037368623.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Vw_Polo_TDI_PD_19_100_0281011820_371260_6118_019ND.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `WV Passat B6 1.9 TDI PD 03G906021NG 394906.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `WinOLS (Audi Q7 (Original) as (All elements) - 396098).bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `a6-8057.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `a6-8058.ori` | `.ORI` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `audi Q7 dsimonek ECU1 orig.pak` | `.PAK` | `76,170` bytes | Raw OEM Factory Binary / Hardware Read (PAK) |
| `eeprom.bin` | `.BIN` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `eeprom_1.bin` | `.BIN` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `flash.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `flash_cmd.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `mcu.ori` | `.ORI` | `238,359` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `mpc.bin` | `.BIN` | `237,767` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `mpc555.bin` | `.BIN` | `462,848` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `orginal.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `orig585.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `orig586.BIN` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `orig696.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `orig697.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `original-hhh.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `original-lll.bin` | `.BIN` | `131,072` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `original.bin` | `.BIN` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `pastdi358702.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `pastdi358703.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `serial e2prom.bin` | `.BIN` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `sharan370538.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `sharan_90hp_019LP.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `t5_flash.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `vw golf 1.9tdi 150bhp 038906019HH 366661.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |

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
