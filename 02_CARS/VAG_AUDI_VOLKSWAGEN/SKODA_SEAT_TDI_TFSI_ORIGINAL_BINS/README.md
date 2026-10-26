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

* **Rentang Tahun / Model Year**: 2000–2012

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `0281001849_038906018BQ_.bin` | **2000–2012** | 256.0 KB | `debb95eb9a2cc486479e44c6fb322ee5` | Factory Binary Firmware Dump |
| `0281001967_312.ori` | **2000–2012** | 128.0 KB | `35fc6058ee7ed10b1c269fe018e27557` | Factory Binary Firmware Dump |
| `0281001967_313.ori` | **2000–2012** | 128.0 KB | `d2368fadc357d50a1bb228525b23a435` | Factory Binary Firmware Dump |
| `032FC.BIN` | **2000–2012** | 1.00 MB | `e87e2fafd75eafdcf0029335af5f3d8e` | Factory Binary Firmware Dump |
| `032QN.std` | **2000–2012** | 1.00 MB | `3d373965a0a4f5661c5e8b8c26c4b8d6` | Factory Binary Firmware Dump |
| `1Z0907115-0261S02114-orig.bin` | **2000–2012** | 2.00 MB | `cefd9bafac75341c43dfb27dbdede3a5` | Factory Binary Firmware Dump |
| `1Z0907115A-0261S02339-orig.BIN` | **2000–2012** | 2.00 MB | `6a530f78e82670ed9ad93f0cae23cacd` | Factory Binary Firmware Dump |
| `2806.ori` | **2000–2012** | 512.0 KB | `cf3b2d92b37bec4d8c6825add058273c` | Factory Binary Firmware Dump |
| `354563.ori` | **2000–2012** | 512.0 KB | `7f34ff404c4f17e4db3040b67915f24c` | Factory Binary Firmware Dump |
| `356587.ori` | **2000–2012** | 128.0 KB | `d0cd128d1e5bce611e9d8241264812b2` | Factory Binary Firmware Dump |
| `356588.ori` | **2000–2012** | 128.0 KB | `580a30d4c5a7d4f04256cfd14d7420c4` | Factory Binary Firmware Dump |
| `746.ori` | **2000–2012** | 128.0 KB | `4cca1740fd895eb9afb60e45dd668ff4` | Factory Binary Firmware Dump |
| `747.ori` | **2000–2012** | 128.0 KB | `5b4c657a98b5df6d3f569462395e7e66` | Factory Binary Firmware Dump |
| `FAbia 1.4 036906034CB .ori` | **2000–2012** | 512.0 KB | `2bc89820f498b04a27ee1c0b8e37281c` | Factory Binary Firmware Dump |
| `Fabia 1.4 75HP 047906033D 5WP4419.ori` | **2000–2012** | 512.0 KB | `32efd350d567251d8161a06e3490d6f8` | Factory Binary Firmware Dump |
| `Octavia 2.0TDI 140HP 03G906021AN  03G906021TC 393521.ori` | **2000–2012** | 2.00 MB | `a9c6f9aeaed072d06ccaf2147146572f` | Factory Binary Firmware Dump |
| `Seat Altea 1.9TDI 105HP 03G906016HB 0281012288 372776.ori` | **2000–2012** | 1.00 MB | `48adb76fa8104b64f5d97a33ecef2364` | Factory Binary Firmware Dump |
| `Seat Arosa 1.7 SDI 50hp 038906013L 0281001748 1834 HHH.bin` | **2000–2012** | 128.0 KB | `6305c8e1dcbfa8d33a31f5e6c223f249` | Factory Binary Firmware Dump |
| `Seat Arosa 1.7 SDI 50hp 038906013L 0281001748 1834 LLL.bin` | **2000–2012** | 128.0 KB | `b5323cd282f222340a50811551a90d6d` | Factory Binary Firmware Dump |
| `Seat Ibiza 1.9 TDI 110hp ASV 0281010006 038906018FB.ori` | **2000–2012** | 256.0 KB | `b6d989521e3741a666256267f90a757d` | Factory Binary Firmware Dump |
| `Seat Inca 1.4i 58HP 6K0906032AE 0261207230 1037360307.ori` | **2000–2012** | 512.0 KB | `6ba4432c17ff3e3c6bee6344b49ec999` | Factory Binary Firmware Dump |
| `Seat Leon 1.9TDI 105HP 03G906021JN 382685.ori` | **2000–2012** | 2.00 MB | `39a36d0de013487431372afe9dad47f1` | Factory Binary Firmware Dump |
| `Seat Leon 2 1.6 06A906033FF-5WP40217-01.ori` | **2000–2012** | 512.0 KB | `f8ec6ab874e0143341867a911a5cd8d5` | Factory Binary Firmware Dump |
| `Seat alhambra 1.8T AJH 150HP 06A906018BT 0261204683 358171.ori` | **2000–2012** | 256.0 KB | `d98e93513ca8fdcf0c35e6785b10f3eb` | Factory Binary Firmware Dump |
| `Seat alhambra 1.9TDI 115HP 038906019ET 0281010630 360459.ori` | **2000–2012** | 512.0 KB | `6473bb86d28c8bdcf6ac252a832144a2` | Factory Binary Firmware Dump |
| `Seat alhambra 1.9TDI 115HP 038906019PA 0281012932 380184.ori` | **2000–2012** | 512.0 KB | `c7ddbdabd8dcd4b23d294243d5e183c0` | Factory Binary Firmware Dump |
| `Seat alhambra 1.9TDI AJM 115HP 038906019J 0281010216 354462.ori` | **2000–2012** | 512.0 KB | `51b1c560b4bf01207fc3511e10b4a0a2` | Factory Binary Firmware Dump |
| `Seat alhambra 1.9TDI ASZ 130HP 038906019BH 0281011199 366689.ori` | **2000–2012** | 512.0 KB | `f50665ec34c2e48f38f122c6f8ae5208` | Factory Binary Firmware Dump |
| `Seat alhambra 2.0TDI 140HP 03G906016JN 381823.ori` | **2000–2012** | 2.00 MB | `63589d36cef81cb66db3960095c9191d` | Factory Binary Firmware Dump |
| `Seat altea 1.9TDI 105HP 0281011885  03G906016DG 370803.ori` | **2000–2012** | 1.00 MB | `e168b31bdbe837a2adeb54a9c1fca9e4` | Factory Binary Firmware Dump |
| `Seat altea 1.9TDI 105HP 03G906021AN 382082.ori` | **2000–2012** | 2.00 MB | `4a7ff45c5738debda5325e932b764e9d` | Factory Binary Firmware Dump |
| `Seat altea 2.0TDI 140HP 0281012278 1037372610.ori` | **2000–2012** | 1.00 MB | `758703940aa4d0618bb64a269a10f580` | Factory Binary Firmware Dump |
| `Seat althea 1.9TDI 105HP 03G906016DH 0281011864 370804.ori` | **2000–2012** | 1.00 MB | `7a133d4f63f9fad6505d4efcf9817e2c` | Factory Binary Firmware Dump |
| `Seat ibiza 0261204593 357494.ori` | **2000–2012** | 64.0 KB | `e3122eb78c27145b4acdeabd22ba52de` | Factory Binary Firmware Dump |
| `Seat ibiza 1.4TDI 75HP 045906019BQ 0281012708 377262.ori` | **2000–2012** | 512.0 KB | `30136e822176b80bcf615d5c30813859` | Factory Binary Firmware Dump |
| `Seat ibiza 1.4TDI AMF 75HP 045906019BG 0281011244 368177.ori` | **2000–2012** | 512.0 KB | `6a83d3be6038ed012cfd54bca81337c4` | Factory Binary Firmware Dump |
| `Seat ibiza 1.4TDI BNM 68HP 45906019BS 0281012319 375931.ori` | **2000–2012** | 512.0 KB | `5fb15b25428bb8b2735390fc86d6e4ec` | Factory Binary Firmware Dump |
| `Seat ibiza 1.8T 150HP 0261206023 352176.ori` | **2000–2012** | 512.0 KB | `3d23562e61e360a8212b7d8da748f731` | Factory Binary Firmware Dump |
| `Seat ibiza 1.8T 180HP 06A906032RP 0261208521 371739.ori` | **2000–2012** | 1.00 MB | `36f31c1f7035a09bd86da5e250ba9512` | Factory Binary Firmware Dump |
| `Seat ibiza 1.8T AYP 150HP 6K0906032AA 0261207071 354562.ori` | **2000–2012** | 512.0 KB | `91b8f34e154db7bb160b3b8681341218` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI AFN 110HP 028906021EK 0281001584.ori` | **2000–2012** | 256.0 KB | `d490c4bb70dff157e6ba99dc50d5f71c` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI ALH 90HP 038906018EE 0281001916.ori` | **2000–2012** | 256.0 KB | `a3420d3bfd81602f3e5a91b4c14f60b4` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI ASV 110HP 038906018FB 0281010006 352282.ori` | **2000–2012** | 256.0 KB | `c3d16a767846aa2a48ccf80b438df817` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI ASZ 130HP 038906019DQ 0281010891 363556.ori` | **2000–2012** | 512.0 KB | `c8e80fdc1692d2ebbc202a4ffeabddb2` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI ASZ 130HP 038906019NF 0281011825 369971.ori` | **2000–2012** | 512.0 KB | `84ce3f8c2f4dd77caf2d4ceea08e814e` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI ATD 100HP 038906019HQ 0281010957 363252.ori` | **2000–2012** | 512.0 KB | `76f7b515db524f010140ad5bca4a2396` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI ATD 100HP 038906019NE 0281011824 371258.ori` | **2000–2012** | 512.0 KB | `a2e3f981c3174b45f194cef245425756` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI BLT 130HP 038906019NJ 0281011823 375966.ori` | **2000–2012** | 512.0 KB | `4299f52d47e0dd5d1554543dd6e823c5` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TDI BLT 130HP 038906019NJ 0281011823 389851.ori` | **2000–2012** | 512.0 KB | `51335652d8db17c8a04c72dbf5cf5f73` | Factory Binary Firmware Dump |
| `Seat ibiza 1.9TID 100HP 038906019NL 0281012276 377186.ori` | **2000–2012** | 512.0 KB | `6e9559e0243b6904f5e27bf19f1ac30c` | Factory Binary Firmware Dump |
| `Seat ibiza 90HP 038906018EC 0281001914 356953.ori` | **2000–2012** | 256.0 KB | `f41650f12d95be957d3b80e96d60d9ae` | Factory Binary Firmware Dump |
| `Seat ibiza cupra 1.9TDI 160HP 0281011852 370651.ori` | **2000–2012** | 512.0 KB | `043532bab9a374e3f4e7308d3728a4bd` | Factory Binary Firmware Dump |
| `Seat ibiza cupra 1.9TDI 160HP 038906019NT 0281012668 378813.ori` | **2000–2012** | 512.0 KB | `0a109be7ff24de5f98558f0f71bd1af2` | Factory Binary Firmware Dump |
| `Seat lean 1.9TDI ASV 110HP 038906012HD 0281011312 367049.ori` | **2000–2012** | 512.0 KB | `2e915716c4602f8a4d48faff4fe6f147` | Factory Binary Firmware Dump |
| `Seat leon 1.8T 180HP 0261206866 0261206866 360165.ori` | **2000–2012** | 1.00 MB | `cc0b8944d6ed23fbd2568f28fb848fd5` | Factory Binary Firmware Dump |
| `Seat leon 1.8T 180HP 06A906032BE 0261206551 352772.ori` | **2000–2012** | 512.0 KB | `73b1f72a401fb00aa17cf4e16e0578e2` | Factory Binary Firmware Dump |
| `Seat leon 1.8T AUQ 180HP 06A906032MJ 0261208115 366379.ori` | **2000–2012** | 1.00 MB | `16c3452a01ae6ca6e8cccbbc806f1421` | Factory Binary Firmware Dump |
| `Seat leon 1.8T AUQ 180HP 06A906032SJ 0261208531 369040.ori` | **2000–2012** | 1.00 MB | `c396c68b972395055199832527fc94b4` | Factory Binary Firmware Dump |
| `Seat leon 1.8T BAM 225HP 1ML906032A 0261208221 367220.ori` | **2000–2012** | 1.00 MB | `04fc025fde790eedc0eabf5ac633b3ae` | Factory Binary Firmware Dump |
| `Seat leon 1.9SDI 68HP 038906012R 0281010058 354413.ori` | **2000–2012** | 512.0 KB | `a83f24971f60e3c00c5d79a89f10e28f` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI 03G906021LK 0281012262 377150ori.bin` | **2000–2012** | 2.00 MB | `465e023394f51a23e106855b6433bc59` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI 105HP 03G906021AN 382081.ori` | **2000–2012** | 2.00 MB | `92693294c976a4e3426c54f36b84e1f8` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI 110HP ASV 038906012AT 0281010062 1037350161.ori` | **2000–2012** | 512.0 KB | `7e546a346e23c58b59afa993b4082a3b` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI AFN 110HP 038906012BT 0281010229 352279.ori` | **2000–2012** | 512.0 KB | `b8e0e43b99c669354af4410988e2c878` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI ALH 90HP 038906012FN 0281010686 360533.ori` | **2000–2012** | 512.0 KB | `594d6ca37c2814ae667152f6737dce59` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI ARL 150HP 038906019FK 0281010687 362484.ori` | **2000–2012** | 512.0 KB | `b398a8ad4c30a2f684f2c5d325d84d40` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI ARL 150HP 038906019FK 0281010687 362707.ori` | **2000–2012** | 512.0 KB | `9e3206bb88ed135ffadb1d140497e1d6` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI ARL 150HP 038906019HK 0281010985 363170.ori` | **2000–2012** | 512.0 KB | `19984dd6ffd61e79edcd52a7d9f1a15b` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI ARL 150HP 038906019HK 0281010985 363170_1.ori` | **2000–2012** | 512.0 KB | `6826b2ee1aff936df0203f5f3d6a1ef7` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI ASV 110HP 0281011997 0281011997 371261.ori` | **2000–2012** | 512.0 KB | `ee256e966ac9d5fe59ecbc98e75ddd60` | Factory Binary Firmware Dump |
| `Seat leon 1.9TDI ASV 110HP 038906012FK 0281010683 360530.ori` | **2000–2012** | 512.0 KB | `575f25b1f421148436b4756092e77a3b` | Factory Binary Firmware Dump |
| `Seat leon 2.0TDI 140HP 03G906021LL 0281013280 381350.ori` | **2000–2012** | 2.00 MB | `7420d0185086ce7de82954eda5e0dd8e` | Factory Binary Firmware Dump |
| `Seat leon 2.0TDI 140HP 03G906021LL 1037381350.ori` | **2000–2012** | 2.00 MB | `3dd76bc304fd8eff69af6ef18872f475` | Factory Binary Firmware Dump |
| `Seat leon 2.0TDI 140HP 03G906021LL 381350.ori` | **2000–2012** | 512.0 KB | `efa22b06cc83ddc9738a7865c0e623f6` | Factory Binary Firmware Dump |
| `Seat leon 2.0TDI 140HP edc16u31 03G906021AN 390153.ori` | **2000–2012** | 2.00 MB | `994f5519741a02bf4165ae5a991b09ed` | Factory Binary Firmware Dump |
| `Seat leon 2.0TDI 170HP 03G906018D.ori` | **2000–2012** | 244.0 KB | `92a08d1ed29329a719642bf0e9db7191` | Factory Binary Firmware Dump |
| `Seat leon 2.0TFSI 185HP 1P0907115D 0261S02289 377624.ori` | **2000–2012** | 2.00 MB | `cf388f94e043f2e6d18163346337a16d` | Factory Binary Firmware Dump |
| `Seat leon 2.0TFSI 1P0907115 0261S02113 386675.ori` | **2000–2012** | 2.00 MB | `4f937103500a5bf1409e4fbdd263beed` | Factory Binary Firmware Dump |
| `Seat leon cupra 1.8T 180HP 06A906032T 0261206545 352761.ori` | **2000–2012** | 512.0 KB | `93d8c6bcd923e101ca8587e2f6ded782` | Factory Binary Firmware Dump |
| `Seat leon cupra 2.0TFSI 240HP 1P0907115C  0261S02337 386637.ori` | **2000–2012** | 2.00 MB | `7c2c4cf023c13df380df410df21414fd` | Factory Binary Firmware Dump |
| `Seat leon-2.0TDI-140hp-03G906016AJ-0281011730.ori` | **2000–2012** | 1.00 MB | `459846c7ad5822a2ba6bc36b3142b751` | Factory Binary Firmware Dump |
| `Seat toledo 1.9TDI AFN 110HP 028906021EF 0281001582 357749.ori` | **2000–2012** | 256.0 KB | `0c84f95cb727b83eb7ac6cd367763f36` | Factory Binary Firmware Dump |
| `Seat toledo 1.9TDI AFN 110HP 038906012BT 0281010229 352279.ori` | **2000–2012** | 512.0 KB | `51afc65a32e496c248d3d3e6a8f8463d` | Factory Binary Firmware Dump |
| `Seat toledo 1.9TDI AFN 110HP 038906012T 0281001060 352232.ori` | **2000–2012** | 512.0 KB | `823e467420caff0d426105423ba5f166` | Factory Binary Firmware Dump |
| `Seat toledo 1.9TDI AGR 90HP 038906012S 0281010059 359845.ori` | **2000–2012** | 512.0 KB | `e60cbbc4e4491b10bbe557e137f035df` | Factory Binary Firmware Dump |
| `Seat toledo 1.9TDI AGR 90HP 038906021BS 0281010228 352278.ori` | **2000–2012** | 512.0 KB | `4a6cf8f4a9555ad655455debff0520b1` | Factory Binary Firmware Dump |
| `Seat toledo 1.9TDI AHU 90HP 028906021FN 0281001604 746-747.ori` | **2000–2012** | 256.0 KB | `57f7e549e1cec43e0cba45a82e652867` | Factory Binary Firmware Dump |
| `Seat toledo 1.9TDI AHU 90HP 038906018BT 0281001926 926687.ori` | **2000–2012** | 256.0 KB | `461902fbc3d0d115f9d9cfca7a64aaf1` | Factory Binary Firmware Dump |
| `Seat_Alhambra_D1900_R4V2T_66kW_0281001252_028906021P_D3E_xx896_crc90FBE681.ori` | **2000–2012** | 64.0 KB | `fc967a1c604a10a360cf5f30f5c38abd` | Factory Binary Firmware Dump |
| `Seat_Alhambra_D1900_R4V2T_66kW_0281001252_028906021P_D3E_xx897_crcBFE76479.ori` | **2000–2012** | 64.0 KB | `3ad40daa05440d7c21949f88388e8645` | Factory Binary Firmware Dump |
| `Seat_Alhambra_D1900_R4V2T_81kW_0281001731_028906021GS_1904_1037357730_731_crcD3E232EF.ori` | **2000–2012** | 256.0 KB | `11dcb18362a7fd2d8f85a5f61c3a0cdf` | Factory Binary Firmware Dump |
| `Seat_Alhambra_D1900_R4V2T_81kW_0281001736_028906021HB_1907_1037356006.ori` | **2000–2012** | 256.0 KB | `5b5d39ec993fc92ca81096f3eae632e5` | Factory Binary Firmware Dump |
| `Seat_Alhambra_D1900_R4V2T_81kW_0281001968_028906021JK_2017_1037350315.ori` | **2017** | 256.0 KB | `62adf946145b6f435068ce7d771c2aa0` | Factory Binary Firmware Dump |
| `Seat_Alhambra_D1900_R4V2T_81kW_0281001968_028906021JK_2019_1037352608.ori` | **2019** | 256.0 KB | `1d960edc5b7df6dc3aa186dfd308f166` | Factory Binary Firmware Dump |
| `Seat_Arosa_D1400_R3V2T_55kW_0281001804_045906019T_1209_1037354619.ori` | **2000–2012** | 512.0 KB | `75a960d08a6a36bf02e4201a7b4d4b4a` | Factory Binary Firmware Dump |
| `Seat_Arosa_D1400_R3V2T_55kW_0281010211_045906019M_1043_1037352639_crcA6662AA0.ori` | **2000–2012** | 512.0 KB | `546e917bab03cdd322525d6a9d417080` | Factory Binary Firmware Dump |
| `Seat_Ibiza_1,8T_180PS_0261208370_06A906032QN_371181.ori` | **2000–2012** | 1.00 MB | `ad69b20950a0c64787e1bbcdde50b53d` | Factory Binary Firmware Dump |
| `Seat_Ibiza_D1900_R4V2T_110kW_0281010687_038906019FK_1469_1037362707_crc967A48EA.ori` | **2000–2012** | 512.0 KB | `e3c3d90eba87d5855a88bfc057c70a14` | Factory Binary Firmware Dump |
| `Seat_Ibiza_D1900_R4V2_47kW_0281001689_038906013E_1513_xxx234_235_crc0A82DEC6.ori` | **2000–2012** | 256.0 KB | `98fa48cc7a9dfc8decfa7d643315acd4` | Factory Binary Firmware Dump |
| `Seat_Ibiza_D1900_R4V2_47kW_0281001701_028906021HA_1439_1037357738_739_crcC2011619.ori` | **2000–2012** | 256.0 KB | `f73d1275b3a99e663e82d9c9544a496a` | Factory Binary Firmware Dump |
| `Seat_Leon_B1800_R4V5T_154kW_0261207952_1ML906032_0001_1037363579_crc01BDF485.ori` | **2000–2012** | 1.00 MB | `9c967e5d53bd4943d3d43ba6a5e210b2` | Factory Binary Firmware Dump |
| `Seat_Leon_B1800_R4V5_92kW_0261204969_06A906032CS_0005_1037354813_crcE01D8FC9.ori` | **2000–2012** | 512.0 KB | `87611a06c4a440841db2c3814a9ae565` | Factory Binary Firmware Dump |
| `Seat_Leon_B1800_R4V5_92kW_0261206587_06A906018GC_V01_1037352129_crc27C747C1.ori` | **2000–2012** | 256.0 KB | `9bf3994410499f883691cc81c12de9c5` | Factory Binary Firmware Dump |
| `Seat_Leon_B1800_R4V5_92kW_0261207648_06A906032JF_0002_1037362901_crcE40BCF28.ori` | **2000–2012** | 512.0 KB | `851fae205dbe07817c2137df6953c2a4` | Factory Binary Firmware Dump |
| `Seat_Toledo_B1800_R4V5_92kW_0261204970_06A906032CR_0005_1037354812_crc94607445.ori` | **2000–2012** | 512.0 KB | `b3c7857913c49bed7d3bfda5b9a2489c` | Factory Binary Firmware Dump |
| `Seat_Toledo_B1800_R4V5_92kW_0261206588_06A906018GD_V01_1037352130_crc6B3FD532.ori` | **2000–2012** | 256.0 KB | `0ffca7b192f77023b7a5cd50d0acd4fe` | Factory Binary Firmware Dump |
| `Seat_Toledo_D1900_R4V2T_66kW_0281001604_028906021FN_1417_1037357258_259_crc0B3C861E.ori` | **2000–2012** | 256.0 KB | `bb405b3de6e9a8befc9d68da4b342f68` | Factory Binary Firmware Dump |
| `Seat_Toledo_D1900_R4V2T_66kW_0281001864_038906018DQ_2146_1037356835_836_crcB3581B58.ori` | **2000–2012** | 256.0 KB | `8eb3b9e05616d7c6713f785a9c5fd9d2` | Factory Binary Firmware Dump |
| `Seat_Toledo_D1900_R4V2T_81kW_0281001582_038906021EF_1419_1037357262_263_crc5DB05C9A.ori` | **2000–2012** | 256.0 KB | `368230fffca177dd0ef81e96073891a2` | Factory Binary Firmware Dump |
| `Skoda 2.0TDI 140HP 03G906021AB 390602.ori` | **2000–2012** | 2.00 MB | `b1c7da617f99cae86161020db270f849` | Factory Binary Firmware Dump |
| `Skoda Fabia 1.2 40KW 03D906032A.ori` | **2000–2012** | 512.0 KB | `6b211b7ec425c20ad99eaa8a0ba37eec` | Factory Binary Firmware Dump |
| `Skoda Fabia 1.4 16V  03C906024B 03C906024F 0896 MARELLI 4HV.ori` | **2000–2012** | 896.0 KB | `5c6b17d5edbc5988601d2b356162a15b` | Factory Binary Firmware Dump |
| `Skoda Fabia 1.4 16V  03C906024R 03C906024F 2489 MARELLI 4HV.ori` | **2000–2012** | 896.0 KB | `46db41c0655574dc198e137beadc0da4` | Factory Binary Firmware Dump |
| `Skoda Fabia 1.4 16V 03C906024B 4115  MARELLI 4HV .ori` | **2000–2012** | 896.0 KB | `2260ba15a502b40df77b6429da27c9a3` | Factory Binary Firmware Dump |
| `Skoda Fabia 1.4 16V 03C906024R 4117 MARELLI 4HV.ori` | **2000–2012** | 896.0 KB | `203f6ea00a5d0a3d0b6baf9f19cc8e94` | Factory Binary Firmware Dump |
| `Skoda Faleicia 1.3i 40KW 5WP4248.ori` | **2000–2012** | 128.0 KB | `7f13adb2544be9f31318642f86efe9b2` | Factory Binary Firmware Dump |
| `Skoda Octavia 1.6MPi 75PS 032906014A.ori` | **2000–2012** | 64.0 KB | `93bf14898663e34ea35f5435d17360d6` | Factory Binary Firmware Dump |
| `Skoda Octavia 1.6MPi 75PS 032906014F.ori` | **2000–2012** | 64.0 KB | `a9b16e02eb64c7a3fbf5191f7ebbe8ec` | Factory Binary Firmware Dump |
| `Skoda Octavia 1.6i 100HP 5WP4428 01 06A906019BT.ori` | **2000–2012** | 256.0 KB | `9e3004bc1de200a0c4573131a64e317b` | Factory Binary Firmware Dump |
| `Skoda Octavia 1.9 TDI 105HP 03G906021RH 389825.ori` | **2000–2012** | 2.00 MB | `9641c7a080a58cc0357409009ae8b83d` | Factory Binary Firmware Dump |
| `Skoda Octavia 1.9TDI 100HP 0281010517 038906019R 360060.ori` | **2000–2012** | 512.0 KB | `a06730ddcb6db3ad5691be057cc3e536` | Factory Binary Firmware Dump |
| `Skoda Octavia 1.9TDI 105HP 03G906021RR 391862.ori` | **2000–2012** | 2.00 MB | `7a5f425ff79ddc4c16be339e6bc1f837` | Factory Binary Firmware Dump |
| `Skoda Octavia 2  1.4i 036906032BF.ori` | **2000–2012** | 1.00 MB | `0aa9ab4e806cbc230ddc584f72623297` | Factory Binary Firmware Dump |
| `Skoda Octavia 2  2.0FSI 150PS 0261S02259 378588.ori` | **2000–2012** | 2.00 MB | `10461d79a40468e643741740046a96bd` | Factory Binary Firmware Dump |
| `Skoda Octavia 2.0 170HP RS 03G906018EL  9953.ori` | **2000–2012** | 244.0 KB | `ffb74809b9871fbae32f5d6fcfc68918` | Factory Binary Firmware Dump |
| `Skoda Octavia 2.0FSI 0261S02018 06F906056R 372560.ori` | **2017–2023** | 2.00 MB | `d039aa6c3c5e01b3a8b6e28b1eaad92f` | Factory Binary Firmware Dump |
| `Skoda Octavia 2.0TDI 140HP 03G906021LD_0281013187_391532.ori` | **2000–2012** | 2.00 MB | `f2ef94dc287309791ea216e50713d7ab` | Factory Binary Firmware Dump |
| `Skoda Octavia 2.0TDI 140HP 03G906021LD_0281013187_Skoda Octavia 2.0TDI 140HP 03G906021LD_0281013187_381024.ori` | **2000–2012** | 2.00 MB | `07daee3d5d131f0091451e15c3c6ac82` | Factory Binary Firmware Dump |
| `Skoda Octavia Scount 2.0TDI 140HP 03G906021MC 390602.ori` | **2000–2012** | 2.00 MB | `76f8f5dbcecf7c9dd089c7416e0856dc` | Factory Binary Firmware Dump |
| `Skoda Octavia-1.8T-06A906032HJ-0261207436-1037362287.bin` | **2000–2012** | 1.00 MB | `2cf993a088cf18292cb639a0bba93cd7` | Factory Binary Firmware Dump |
| `Skoda Octavia-1.8T-06A906032HJ-0261207436-1037366426.bin` | **2000–2012** | 1.00 MB | `40fc0f5250227e51e5620bd89421cbdf` | Factory Binary Firmware Dump |
| `Skoda Superb 2.0TDI 140HP 03G906016GT 387090.ori` | **2000–2012** | 2.00 MB | `3b8b4ee89e3baad331562b6cdb2f5040` | Factory Binary Firmware Dump |
| `Skoda Superb 2.8 1 02612085471 3B0907551DD 369310.ori` | **2000–2012** | 1.00 MB | `9055c434fffeb5356634b8d871301e55` | Factory Binary Firmware Dump |
| `Skoda fabia 1.4 16V 100HP 036906034BK IAW 4LV.C.ori` | **2000–2012** | 512.0 KB | `82f9c5cc1587c2e746c8e8f482bfb1f3` | Factory Binary Firmware Dump |
| `Skoda fabia 1.4 68HP 5WP40179 047906033H.ori` | **2000–2012** | 512.0 KB | `1dad2a92de48752bb0559533e1e91260` | Factory Binary Firmware Dump |
| `Skoda fabia 1.4TDI 70HP 045906019BR 0281012318 377261.ori` | **2000–2012** | 512.0 KB | `cdf2e391b250eb2ee67ed494fb226d6d` | Factory Binary Firmware Dump |
| `Skoda fabia 1.9SDI 64HP 038906012AN 0281010107 354365.ori` | **2000–2012** | 512.0 KB | `e9f188ca665af23a73e5b28c0fd9a429` | Factory Binary Firmware Dump |
| `Skoda fabia 1.9SDI 64HP 038906012GD 0281010861 362792.ori` | **2000–2012** | 512.0 KB | `895b72ca6b673337cb4e93ee81295be0` | Factory Binary Firmware Dump |
| `Skoda fabia 1.9SDI 64HP 038906012HR 0281011321 1037367058.ori` | **2000–2012** | 512.0 KB | `0428b7d9e4f7650a160354a5f91ff679` | Factory Binary Firmware Dump |
| `Skoda fabia 1.9TDI 105HP 038906019NS 0281013082 386363.ori` | **2000–2012** | 512.0 KB | `3acef3dc558859865d88e24f230d7c03` | Factory Binary Firmware Dump |
| `Skoda fabia 1.9TDI 130HP 038906019 0281011217 366587.ori` | **2000–2012** | 512.0 KB | `934a2340c4d6dd46d588bf4206af948f` | Factory Binary Firmware Dump |
| `Skoda fabia 1.9TDI ASZ 130HP 038906019LA 0281011217 368406.ori` | **2000–2012** | 512.0 KB | `09ba3d0f4e713dc90c270b702517cf64` | Factory Binary Firmware Dump |
| `Skoda fabia 1.9TDI ASZ 130HP 038906019NF 0281011825 372304.ori` | **2000–2012** | 512.0 KB | `caf8cf99f05646f3ffe6e8b0dad70af2` | Factory Binary Firmware Dump |
| `Skoda fabia 1.9TDI ATD 100HP 038906019KT 0281011219 368184.ori` | **2000–2012** | 512.0 KB | `8af5ada5f1bf253bfd3ba411b44651f6` | Factory Binary Firmware Dump |
| `Skoda ocatavia 1.9TDI AHF 110HP 038906012G 0281010128 360549.ori` | **2000–2012** | 512.0 KB | `bcb271c9e234c4959580f0c36d4bb7d7` | Factory Binary Firmware Dump |
| `Skoda octavia 1.6 06A906019BH 5WP4860.ori` | **2000–2012** | 256.0 KB | `f265bbb54dbf0b949de81380f746a8f9` | Factory Binary Firmware Dump |
| `Skoda octavia 1.6 AEE 032906030AG.ori` | **2000–2012** | 64.0 KB | `0369fb33197ea51591e9c13e2ee9069f` | Factory Binary Firmware Dump |
| `Skoda octavia 1.6i 06A906033BG 5WP4015.ori` | **2000–2012** | 512.0 KB | `91b287c55a7a391214dca0a24f53e50f` | Factory Binary Firmware Dump |
| `Skoda octavia 1.8T AGU 150HP 06A906018CF 0261206141 5663756.ori` | **2000–2012** | 256.0 KB | `c1fe7ae8692044bfaabc205f6ecca97d` | Factory Binary Firmware Dump |
| `Skoda octavia 1.8T AGU 150HP 06A906018GA 261206519 352013.ori` | **2000–2012** | 256.0 KB | `e22638a4d55d4bc54269a95495a0a18a` | Factory Binary Firmware Dump |
| `Skoda octavia 1.8T AGU 150HP 06A906018GB 0261206520 350785.ori` | **2000–2012** | 256.0 KB | `53bd85d880c921abf56320de5fc972d7` | Factory Binary Firmware Dump |
| `Skoda octavia 1.8T ANB 150HP 4B0906018AC 0261206452 352160.ori` | **2000–2012** | 512.0 KB | `556b7de1774f33a9dc515e38b65efddc` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9SDI 68HP 038906012E 0281010105 360446.ori` | **2000–2012** | 512.0 KB | `053f957bb461cd3d203f08aae1c4547c` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI 105HP 03G906016K 0281012237 372601.ori` | **2000–2012** | 1.00 MB | `457367d087e1c2ee161f3232d9e7edf6` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI 105HP 03G906021LB 382414.ori` | **2000–2012** | 2.00 MB | `6f998ec4d21414f1f1ce3e6c2b1f53d9` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI 130HP 038906019EG 0281010928 351906.ori` | **2000–2012** | 512.0 KB | `145d60eeaf5113f11c0897fe5c3fa583` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI 90HP 038906012F 0281010127 350855.ori` | **2000–2012** | 512.0 KB | `057cdaf38af1141894d06aec4d81419c` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI 90HP 038906012F 0281010127 360546.ori` | **2000–2012** | 512.0 KB | `214221d773488a4954a238b97d94649e` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AGR 90HP 038906012F 0281010127 1037350855.ori` | **2000–2012** | 512.0 KB | `cea5ec579593b2e2573e4f868b2949f4` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AGR 90HP 038906012H 0281010129 350857.ori` | **2000–2012** | 512.0 KB | `b63dc5227bb31539c1e86e8adf3ed1fd` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AGR 90HP 038906018AG 0281001695 357789.ori` | **2000–2012** | 256.0 KB | `38995855cb177e29d77a8ade87bfe3c6` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AGR 90HP 038906018BC 0281001755 357868.ori` | **2000–2012** | 256.0 KB | `790f48a7b924248a68f99709d6a9fcfd` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AGR 90HP 038906018GM 0281010181 350932.ori` | **2000–2012** | 256.0 KB | `729ca45b1399ef3668f787d0e10049e4` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AHF 110HP 038906012G 0281010128 350856.ori` | **2000–2012** | 512.0 KB | `fa9444465c1cba36608a7ef86ef8fac4` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AHF 110HP 038906018AM 0281001707 242.ori` | **2000–2012** | 256.0 KB | `b724cba197e37e11a6bbff4a3de5af7e` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AHF 110HP 038906018GN 0281010182 110934.ori` | **2000–2012** | 256.0 KB | `6ec9789b019f1392f08e8ef183fbf65a` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI AHU 90HP 038906018B 0281001602 355556.ori` | **2000–2012** | 256.0 KB | `eea06611ba26b9b7cf7619973f633fa2` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI ASV 110HP 038906012BA 0281010130 352668.ori` | **2000–2012** | 512.0 KB | `529eee583ee7fb8972e4089fa341430f` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI ASV 110HP 038906012CL 0281010380 354322.ori` | **2000–2012** | 512.0 KB | `63c1829b915b54146a8a70fedf95accd` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI ASV 110HP 038906012CL 0281010380 362160.ori` | **2000–2012** | 512.0 KB | `70a65e1580d48059d302f83c2ec4c8a3` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI ASV 110HP 038906012HC 0281011311 367048.ori` | **2000–2012** | 512.0 KB | `7e4cfd8177dc4b1068c5027f32fd7f5d` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI ASZ 130HP 038906019HJ 0281010977 366272.ori` | **2000–2012** | 512.0 KB | `1cf5cd4b43a107f7471d0e9c5ab34679` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI ATD 100HP 038906019DL 0281011077 363696.ori` | **2000–2012** | 512.0 KB | `29409fa8337d415205bb79d8f018b574` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI ATD 100HP 038906019FJ 0281010789 362146.ori` | **2000–2012** | 512.0 KB | `735e634feef4d469f92b1b5c4697ab63` | Factory Binary Firmware Dump |
| `Skoda octavia 1.9TDI BJB 105HP 03G906016AG 0281011658 370256.ori` | **2000–2012** | 1.00 MB | `3609d77756435a307fd0a6e097b4a05a` | Factory Binary Firmware Dump |
| `Skoda octavia 110HP AHF 038906018BR 0281001850 597-598.ori` | **2000–2012** | 256.0 KB | `a65d69492f387857a183067aa694f317` | Factory Binary Firmware Dump |
| `Skoda octavia 2.0TDI 140HP 03G906021LD 379738.ori` | **2000–2012** | 2.00 MB | `b56fa2fc761d24432252559f1418b5e9` | Factory Binary Firmware Dump |
| `Skoda octavia 2.0TDI BKD 140HP 03G906016DS 0281011953 372775.ori` | **2000–2012** | 1.00 MB | `a0f5a463ba66b88492958a196e45aa1c` | Factory Binary Firmware Dump |
| `Skoda octavia 2.0TDI BMM 140HP 03G906021JC 382441.ori` | **2000–2012** | 2.00 MB | `9135ca1744e4b9b8d5797398aa9e27f9` | Factory Binary Firmware Dump |
| `Skoda octavia 2.0TDI-03G906021JC-AB-7GG-BMM-1037392969.bin` | **2000–2012** | 2.00 MB | `fe33e66a28b8d24002e07067336d9ef3` | Factory Binary Firmware Dump |
| `Skoda octavia II 2.0TDI 140HP 03G906016F 0281011391 370892.ori` | **2000–2012** | 1.00 MB | `45ffa79b8b707e80c0bb803d907ca7fe` | Factory Binary Firmware Dump |
| `Skoda octavia RS 03G906018HB.ori` | **2000–2012** | 2.00 MB | `aa9c9ae488e3bb261ec644bef20763ee` | Factory Binary Firmware Dump |
| `Skoda octavia RS 1.8T 180HP 06a906032bj 0261206892 360288.ori` | **2000–2012** | 1.00 MB | `e33b58b881b31bd92b202d965fb09436` | Factory Binary Firmware Dump |
| `Skoda octavia RS 1.8T AUQ 06A906032SG 0261208532 369039.ori` | **2000–2012** | 1.00 MB | `e9dc14f2c08cca2236f77548141ad362` | Factory Binary Firmware Dump |
| `Skoda octavia RS 2.0TFSI 200HP 1Z0907115A 0261S02339 386859.ori` | **2000–2012** | 2.00 MB | `5b9a80e91bc924ba34766c30d617e4f4` | Factory Binary Firmware Dump |
| `Skoda oktavia 1.9TDI 90HP 038906012HA 0281011309 367046.ori` | **2000–2012** | 512.0 KB | `0a12cf20838c09950204468e1699a4a8` | Factory Binary Firmware Dump |
| `Skoda oktavia 1.9TDI AGR 90HP 038906012H 02810101291037360547.ori` | **2000–2012** | 512.0 KB | `7f8dc787ecb2cf8cf533e5ae5f45a42f` | Factory Binary Firmware Dump |
| `Skoda roomster 1.4TDI - 69HP 045906019CJ 0281013180 382690.ori` | **2000–2012** | 512.0 KB | `1943bcf5650af9f8a67f245593ff7842` | Factory Binary Firmware Dump |
| `Skoda roomster 1.9TDI 105HP 038906019NR 0281013081 381002.ori` | **2000–2012** | 512.0 KB | `853f6d1c1053df9cf2ac6dbd83404b00` | Factory Binary Firmware Dump |
| `Skoda superb 1.8T 180HP 8E0909018A 0261207929 1037366458.ori` | **2000–2012** | 1.00 MB | `f6ef24aefd67cba046db07fe42e06b5a` | Factory Binary Firmware Dump |
| `Skoda superb 1.9TDI 105HP 3G906021QN 1037395404.ori` | **2000–2012** | 2.00 MB | `bbdba47daebe82f91a5adcacb37d855d` | Factory Binary Firmware Dump |
| `Skoda superb 1.9TDI 130HP 038906019EG 0281010928 363744.ori` | **2000–2012** | 512.0 KB | `5c9c635b3f23ce630740b6c0599d5524` | Factory Binary Firmware Dump |
| `Skoda_Fabia_D1900_R4V2T_74kW_0281010289_038906019AF_1056_1037352972_crc146360EC.ori` | **2000–2012** | 512.0 KB | `d6d886d60fc5d6dc7bdab98f3fb500a1` | Factory Binary Firmware Dump |
| `Skoda_Fabia_D1900_R4V2T_74kW_0281010289_038906019AF_1110_1037354466_crcCBCBF822.ori` | **2014–2020** | 512.0 KB | `62b053d7647975641f50a77d00d3b369` | Factory Binary Firmware Dump |
| `Skoda_Octavia_1,9_TDI_105PS_0281011883_03G906016DJ_6250_1037371259.ori` | **2000–2012** | 1.00 MB | `15d0dcad65d2ad217b12c40776da2d9a` | Factory Binary Firmware Dump |
| `Skoda_Octavia_2,0TFSI_200PS_0261S02114_1Z0907115_377701.ori` | **2000–2012** | 2.00 MB | `7646a895db889f6549a8aeb5e94c11fb` | Factory Binary Firmware Dump |
| `Skoda_Octavia_B1800_R4V5_92kW_0261204373_06A906018H_V05_1037358798_crc2ABE377E.ori` | **2000–2012** | 128.0 KB | `a4689061b702f291dcbf7d36a8b88279` | Factory Binary Firmware Dump |
| `Skoda_Octavia_B1800_R4V5_92kW_0261204681_6A906018AM_V02_1037358186_crcAAFD2CBF.ori` | **2000–2012** | 256.0 KB | `0e3cdadf61f64dbed984dfee823b6c7c` | Factory Binary Firmware Dump |
| `Skoda_Octavia_D1900_R4V2T_74kW_0281011077_038906019DL_1548_1037363696_crc87D4BD87.ori` | **2000–2012** | 512.0 KB | `f4915f962bbc64e5f38bd835b2d2d8ae` | Factory Binary Firmware Dump |
| `Skoda_Octavia_D1900_R4V2T_84kW_0281010517_038906019R_1275_1037360480_CRC1934580e.ori` | **2000–2012** | 512.0 KB | `ed13a6af57afa84d7b9e24a8d016679c` | Factory Binary Firmware Dump |
| `Skoda_Superb_B1800_R4V5T_110kW_0261207928_8E0909018A_P0000_1037363930_crc97A78B5B.ori` | **2000–2012** | 1.00 MB | `5386a9381f19b6be5d46b9a52b0cb0a4` | Factory Binary Firmware Dump |
| `Skoda_Superb_D2500_V6V4T_114kW_0281010905_3U0907401_D09_1037366618_crc08B732A0.ori` | **2000–2012** | 512.0 KB | `a5fc98ed0a89edbc24aa61f29ae3a880` | Factory Binary Firmware Dump |
| `Sokda Fabia 1.4 68HP  047906033 5WP4419.ori` | **2000–2012** | 512.0 KB | `706f155ea214ff7f2bbbae02f5242324` | Factory Binary Firmware Dump |
| `WinOLS (Seat Leon Cupra (Original) as (All elements) - 386637).bin` | **2000–2012** | 2.00 MB | `b48203d781a2c893a37133e020ae891d` | Factory Binary Firmware Dump |
| `WinOLS (Skoda New Octavia (Original) as Eprom - 379738).bin` | **2000–2012** | 2.00 MB | `0f9ad1327d51f33a058807f0587f5b80` | Factory Binary Firmware Dump |
| `ibiza_org_038_906_019_LA.bin` | **2000–2012** | 512.0 KB | `8d5545108145786ddf8592f5436fafae` | Factory Binary Firmware Dump |

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
