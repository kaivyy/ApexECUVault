# NISSAN_HISTORIC_FACTORY_BIN_SUITE - ECU Calibration Suite

**Repository Path**: `02_CARS/NISSAN_INFINITI/NISSAN_HISTORIC_FACTORY_BIN_SUITE`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `453 files` (453 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `NISSAN_HISTORIC_FACTORY_BIN_SUITE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2000–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `92Pathfinder.bin` | **1992** | 32.0 KB | `0b72b05c287d35e82527aa96c9c18eab` | Factory Binary Firmware Dump |
| `A31_RB20DET_5L210_MEC-R330_AT.BIN` | **2000–2024** | 32.0 KB | `3486bd45af12c2dbd1db0958592f4b50` | Factory Binary Firmware Dump |
| `A31_RB20DET_73L00_R102D_MT.bin` | **2000–2024** | 16.0 KB | `2d39cda43a573a65e79dd7ae96a2790d` | Factory Binary Firmware Dump |
| `A31_RB20DET_73L10_MEC-R103D_AT.bin` | **2000–2024** | 16.0 KB | `cb3ddc5e63be7a3f86addc04a65cbd3c` | Factory Binary Firmware Dump |
| `A31_RB20DET_94L10_MEC113_AT.bin` | **2000–2024** | 16.0 KB | `bb64b4de6aaedd16157df278c2b9dae9` | Factory Binary Firmware Dump |
| `A31_RB20DE_72L00_MEC-R100d_MT.bin` | **2000–2024** | 16.0 KB | `949d296bdf91291b455c6d6799c9427f` | Factory Binary Firmware Dump |
| `A31_RB20DE_72L10_MEC-R101D_MT.BIN` | **2000–2024** | 16.0 KB | `744351143e6ae3b9c8af4d584f180327` | Factory Binary Firmware Dump |
| `A32_VQ30DE_0L701_MT_1997.bin` | **1997** | 64.0 KB | `5712495841b4c0deb304ff90e8ba69f0` | Factory Binary Firmware Dump |
| `A32_VQ30DE_40U01_1995_MT.bin` | **1995** | 64.0 KB | `246ec3d0820b098bcd63a5e16b7ab808` | Factory Binary Firmware Dump |
| `A32_VQ30DE_40U03_1995_MT.bin` | **1995** | 64.0 KB | `37b1821a217aa161859cb760c2d0c83b` | Factory Binary Firmware Dump |
| `A32_VQ30DE_40U11_1995_AT.bin` | **1995** | 64.0 KB | `986417d21b81d967db4078cd1cfbe037` | Factory Binary Firmware Dump |
| `A32_VQ30DE_40U11_1995_AT_maps.bin` | **1995** | 64.0 KB | `a357f8b2134e737c49c7531599c20616` | Factory Binary Firmware Dump |
| `A32_VQ30DE_40U13_1995_AT.bin` | **1995** | 64.0 KB | `294fd92873901f98b00de3a27b654ef3` | Factory Binary Firmware Dump |
| `A32_VQ30DE_40U13_1995_AT_maps.bin` | **1995** | 64.0 KB | `251132793b5c0b1b0023c90378562355` | Factory Binary Firmware Dump |
| `A32_VQ30DE_49U10_1995_AT_consult.bin` | **1995** | 64.0 KB | `7133319931149ba5de29a3dbaf26b0a6` | Factory Binary Firmware Dump |
| `A32_VQ30DE_54U00_1996_MT.bin` | **1996** | 64.0 KB | `5e5c8f1417327b2ee09a16b50b8d35f1` | Factory Binary Firmware Dump |
| `A32_VQ30DE_54U01_1996_MT.bin` | **1996** | 64.0 KB | `a10bf2773178ea83a428fb831058f84d` | Factory Binary Firmware Dump |
| `A32_VQ30DE_54U03_1996_MT.bin` | **1996** | 64.0 KB | `d8792620bdad41a2a1a8cfa75a68da2f` | Factory Binary Firmware Dump |
| `A32_VQ30DE_54U11_1996_AT.bin` | **1996** | 64.0 KB | `e37298a901cde1afe518709fa2308814` | Factory Binary Firmware Dump |
| `A32_VQ30DE_54U13_1996_AT.bin` | **1996** | 64.0 KB | `d6a0b0bbe7b7b9adb945ffba77b68c1d` | Factory Binary Firmware Dump |
| `B13_E16E_79Y05_MT.bin` | **2000–2024** | 32.0 KB | `225f9903053a2e4fb01c28cfa3507255` | Factory Binary Firmware Dump |
| `B13_GA16DE_73Y05_MT.bin` | **2000–2024** | 32.0 KB | `2ecb4f4f515e04e9230ae35e55b6d9fb` | Factory Binary Firmware Dump |
| `B13_GA16DE_81R00_MT.bin` | **2000–2024** | 32.0 KB | `87b6da5cfd8c0081eecc8fe600b9ca94` | Factory Binary Firmware Dump |
| `B13_GA16DE_81R05_MT.bin` | **2000–2024** | 32.0 KB | `d9317f100fb64e15d1faf2025cf2b089` | Factory Binary Firmware Dump |
| `B13_SR20DE_64Y00_MT.bin` | **2000–2024** | 32.0 KB | `7f559766ef9b20742c25cf0bed5e30fd` | Factory Binary Firmware Dump |
| `B13_SR20DE_64Y01_MT.bin` | **2000–2024** | 32.0 KB | `5421011c33869e574461f146b376c6df` | Factory Binary Firmware Dump |
| `B13_SR20DE_64Y02.bin` | **2000–2024** | 32.0 KB | `9a26edbaabc757e8aac00f5d4092ef34` | Factory Binary Firmware Dump |
| `B13_SR20DE_64Y15_AT.bin` | **2000–2024** | 32.0 KB | `0059e6b627c4aba9aa7fd022e051f0a0` | Factory Binary Firmware Dump |
| `B13_SR20DE_67Y00_MT.bin` | **2000–2024** | 32.0 KB | `223c138913268e371bd9693420d6d834` | Factory Binary Firmware Dump |
| `B13_SR20DE_70Y05_MT.bin` | **2000–2024** | 32.0 KB | `3af269b100aa261acb037047ae0bfe21` | Factory Binary Firmware Dump |
| `B13_SR20DE_71Y00_MT.bin` | **2000–2024** | 32.0 KB | `85810c08e9e0b89034971697c2dec485` | Factory Binary Firmware Dump |
| `B13_SR20DE_71Y05_MT.bin` | **2000–2024** | 32.0 KB | `2d161f1aaf27dfbdacc9bfc9dd881a3d` | Factory Binary Firmware Dump |
| `B13_SR20DE_78C20.bin` | **2000–2024** | 32.0 KB | `58a9560a773a2bf7132e8adedc6b24dd` | Factory Binary Firmware Dump |
| `B13_SR20DE_94Y00.bin` | **2000–2024** | 64.0 KB | `a09c6e98bbd91d66058763c89e341194` | Factory Binary Firmware Dump |
| `B14_GA16DE_0M201_MT.bin` | **2000–2024** | 64.0 KB | `9df60cfebb030054674a20877e0288f5` | Factory Binary Firmware Dump |
| `B14_GA16DE_0M272_AT.bin` | **2000–2024** | 64.0 KB | `82d349c341d27391b5c0317d4178ffcb` | Factory Binary Firmware Dump |
| `B14_GA16DE_2M000_MT.bin` | **2000–2024** | 32.0 KB | `4851079e74e8a76353ffd35a429b98e7` | Factory Binary Firmware Dump |
| `B14_SR20DE_0M761_MT.bin` | **2000–2024** | 64.0 KB | `38b673e71dca244e44996d137b34891b` | Factory Binary Firmware Dump |
| `B14_SR20DE_0M765_AT.bin` | **2000–2024** | 64.0 KB | `259489e8b56a868819f87969d6be576e` | Factory Binary Firmware Dump |
| `B14_SR20DE_1M860_MT.bin` | **2000–2024** | 64.0 KB | `e9ca796e2ece6d6c90abf62c6ec4ed4e` | Factory Binary Firmware Dump |
| `B14_SR20DE_1M861_MT.bin` | **2000–2024** | 64.0 KB | `025e3ddf7aca828baef99b1215405897` | Factory Binary Firmware Dump |
| `B14_SR20DE_1M871_MT.bin` | **2000–2024** | 64.0 KB | `22476c859d6cd020de89423b8dc9c851` | Factory Binary Firmware Dump |
| `B14_SR20DE_1M876_AT.bin` | **2000–2024** | 64.0 KB | `139c61f9614c8238f563c8421e992797` | Factory Binary Firmware Dump |
| `B14_SR20DE_2M080.bin` | **2000–2024** | 64.0 KB | `c77ac9a0b7be9cd2e4d92da05413357f` | Factory Binary Firmware Dump |
| `B14_SR20DE_4M201.bin` | **2000–2024** | 64.0 KB | `652d02034baf7817ff66978e6ea59903` | Factory Binary Firmware Dump |
| `B14_SR20DE_xxxxx.BIN` | **2000–2024** | 64.0 KB | `2191d49df4efa81cdaad2b97d5a5d793` | Factory Binary Firmware Dump |
| `BNCR33_RB26DETT_24U00.bin` | **2000–2024** | 32.0 KB | `76eab1f407eccc121e1829a4be5e6af7` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U02_MT_MECR128.bin` | **2000–2024** | 32.0 KB | `7ec4c92bc09498595fbc61d1e883299e` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U03_MT_MEC-R138.BIN` | **2000–2024** | 32.0 KB | `6687444c0f098e91f418cfab02a1a67f` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U60_MT_MECR280.bin` | **2000–2024** | 32.0 KB | `c4173c0ff5051ee9b90766ee869475ef` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U61_MT_MECR281.bin` | **2000–2024** | 32.0 KB | `bbe7a861efd6813e88a8d4e7805cafe7` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U62_MT_MECR282A.BIN` | **2000–2024** | 32.0 KB | `3269f74f11578842638c456048c8b517` | Factory Binary Firmware Dump |
| `C23_SR20DE_2C000_MT.bin` | **2000–2024** | 32.0 KB | `0ff43d7dc059f2a2a36822a09ecde58d` | Factory Binary Firmware Dump |
| `C33_RB20DE_71L60_ MT_DEB7.BIN` | **2000–2024** | 32.0 KB | `a24d21902f9a57d25be0a4d15128422e` | Factory Binary Firmware Dump |
| `C33_RB20DE_72L70_AT_MEC-R201B.BIN` | **2000–2024** | 32.0 KB | `d6560466b5b62e5fc5a50fa20ef08cf7` | Factory Binary Firmware Dump |
| `C35_RB25DET_8L302.bin` | **2000–2024** | 64.0 KB | `bf7a6bdd0f326dd9e48b60c47640cb06` | Factory Binary Firmware Dump |
| `CR31_RB30E_J7100_MT.bin` | **2000–2024** | 16.0 KB | `e4fe5d11c8ea71549913b8f067f61ce0` | Factory Binary Firmware Dump |
| `CR31_RB30E_J7110_AT.bin` | **2000–2024** | 16.0 KB | `721747bcc9d7a9c5810b72e5a0b3ecfd` | Factory Binary Firmware Dump |
| `D21_KA24DE_1993_MT_FED.bin` | **1993** | 32.0 KB | `75b560996f6ac316014e886ea33622e8` | Factory Binary Firmware Dump |
| `D21_KA24E_76P00_MECMT113.bin` | **2000–2024** | 32.0 KB | `3229bb9b8e194bf89450ab08daa374c9` | Factory Binary Firmware Dump |
| `D21_KA24E_86G01_MECMT110.bin` | **2000–2024** | 32.0 KB | `a2346293593dc58d89b2111619229ca0` | Factory Binary Firmware Dump |
| `D21_KA24E_MECMT122.bin` | **2000–2024** | 32.0 KB | `7f3739aa9b743907523e060f3d4711f9` | Factory Binary Firmware Dump |
| `D21_VG30E_MECM-V131.BIN` | **2000–2024** | 32.0 KB | `d6a39b908700136499efa9e3875baeac` | Factory Binary Firmware Dump |
| `ECR32_FOR_RB25_08U01_MT.bin` | **2000–2024** | 32.0 KB | `5d3de6a8abaa2b6b3a69f83474ce99f1` | Factory Binary Firmware Dump |
| `ECR32_RB25DE_08U01_MT_MEC-R232.Bin` | **2000–2024** | 32.0 KB | `d05f31ee66fa90601c2dd9c4b79d0320` | Factory Binary Firmware Dump |
| `ECR32_RB25DE_08U02_MT.Bin` | **2000–2024** | 32.0 KB | `6d3af9d53fdbf53ac8f07256eda67dd6` | Factory Binary Firmware Dump |
| `ECR32_RB25DE_08U11_AT.Bin` | **2000–2024** | 32.0 KB | `01b76ca0a562b4e18c791c5bf48085a4` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_13U00_MT_MEC-R720.bin` | **2000–2024** | 32.0 KB | `c8950859d771360e4b69defbcd3cf3c1` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_13U01_MT_MEC-R260.bin` | **2000–2024** | 32.0 KB | `ecc2ae76a8b877cd8d2641e81c9aed2f` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U00_MT_MECR520.bin` | **2000–2024** | 32.0 KB | `8ff34d3cd1ff166a7f6e0432c8753d65` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U01_MT_MECR521_daughterboard.BIN` | **2000–2024** | 32.0 KB | `a3913ab115b4f37c3e37698d298dd866` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U02_MT.bin` | **2000–2024** | 32.0 KB | `59ee88ecb993d90c60055da4e511ca6f` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U03.bin` | **2000–2024** | 32.0 KB | `dc037cb006ff718da05571acae9b4388` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U11_AT_MECR531.bin` | **2000–2024** | 32.0 KB | `dcaa3f2695a6dc82d933a9a8db55a09f` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U60_MT_MECR530.bin` | **2000–2024** | 32.0 KB | `5ab53e3c832ef44721e6aabeb28d8fea` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U70.bin` | **2000–2024** | 32.0 KB | `f1af734b5fac1f69e148154569835c1a` | Factory Binary Firmware Dump |
| `ECR33_RB25DE_17U14_AT_MECR514.bin` | **2000–2024** | 32.0 KB | `88e7f19bf52d52c6d4b84f9a0c766a34` | Factory Binary Firmware Dump |
| `ECR33_RB25DE_28U00_MT_MEC-R700.bin` | **2000–2024** | 32.0 KB | `d87200d55fd5d75bca9ed099459047c8` | Factory Binary Firmware Dump |
| `EFK10_MA09ET_37B10.BIN` | **2000–2024** | 16.0 KB | `dd73329bf36080bf77fc240fdff2b33f` | Factory Binary Firmware Dump |
| `EK10_MA09ERT_21B00_MT_T104ADM6.bin` | **2000–2024** | 16.0 KB | `667b5e66929bab8458e1534693314ebd` | Factory Binary Firmware Dump |
| `EK10_MA09ERT_Nismo.BIN` | **2000–2024** | 16.0 KB | `797a2c85a8bdc377d625c4bd09be22f5` | Factory Binary Firmware Dump |
| `EK10_MA09ERT_STOCK_EK10009518.bin` | **2000–2024** | 16.0 KB | `dde8d2017f5f66e0b242862f09e29aa6` | Factory Binary Firmware Dump |
| `ENR33_RB20E_29U10_MECR750_1997.bin` | **1997** | 32.0 KB | `9f15928b4a226a4ae681ed5325a745da` | Factory Binary Firmware Dump |
| `ENY34_VQ30DE_AG500.bin` | **2000–2024** | 64.0 KB | `a41663d846e0bc5ac3a5f74f7d98b66e` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA500_MT.bin` | **2000–2024** | 64.0 KB | `c3015b3be3081fb76a2883e3f8727a44` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA501_MT.bin` | **2000–2024** | 64.0 KB | `71b5ed4eeead5b9a3851df20f825dd5c` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA502_MT.bin` | **2000–2024** | 64.0 KB | `fc6bfe12b220501a02808dbe9d8a3644` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA510_AT.bin` | **2000–2024** | 64.0 KB | `a70a1f93f0be45c6ead3b29de32aced8` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA511_AT.bin` | **2000–2024** | 64.0 KB | `f7f7065d16877bfb510355b0558d6f84` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA512_AT.bin` | **2000–2024** | 64.0 KB | `f8d8dade7aa82442721ae35034991474` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA513_AT.bin` | **2000–2024** | 64.0 KB | `9030d7c636fdbe6480295790dd4537a6` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA560_MT.bin` | **2000–2024** | 64.0 KB | `3cd1425872f768da8110c241f9630126` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA570_AT.bin` | **2000–2024** | 64.0 KB | `b47cf11ed3ffe14643cd6b3b314857a5` | Factory Binary Firmware Dump |
| `F31_VG20DET_F6371_MECE55.bin` | **2000–2024** | 16.0 KB | `a3f773a441012e1550fdc6e66ac24522` | Factory Binary Firmware Dump |
| `G20_P10_SR20DE_0J200_MT_1994.bin` | **1994** | 64.0 KB | `aba8bd7ba2039c0b7d79396c180cfe79` | Factory Binary Firmware Dump |
| `G20_P10_SR20DE_0J202_MT_1995.bin` | **1995** | 64.0 KB | `23370230711141a51025fdf5be243090` | Factory Binary Firmware Dump |
| `G20_P10_SR20DE_0J203_MT_1995.bin` | **1995** | 64.0 KB | `413d42578fba08f85060f28ee01a34d8` | Factory Binary Firmware Dump |
| `G20_P10_SR20DE_0J212_AT_1995.bin` | **1995** | 64.0 KB | `2462d362b039d0151c035a60e7f07edf` | Factory Binary Firmware Dump |
| `G20_P10_SR20DE_0J600_MT_1995.bin` | **1995** | 64.0 KB | `f3138d3b7a1d92148a638ed217020cae` | Factory Binary Firmware Dump |
| `G20_P10_SR20DE_0J610_AT_1995.bin` | **1995** | 64.0 KB | `137b2a81de1dab5ea862f422bcc52c8c` | Factory Binary Firmware Dump |
| `HB14_SR18DE_0M801.bin` | **2000–2024** | 32.0 KB | `f37f64562c341e2be300f17325585a21` | Factory Binary Firmware Dump |
| `HB14_SR18DE_0M811.bin` | **2000–2024** | 32.0 KB | `c4213cdd9eadfd12b274cd60016d27cb` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_01U01_MEC-R124.BIN` | **2000–2024** | 32.0 KB | `5040ac9797dc65418ab04622e0f43a3a` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U00_MT_MEC-R106.bin` | **2000–2024** | 32.0 KB | `2b632fe336fa6c9e8ff3cecfdc6e3be0` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U01_MT_MEC-R126.BIN` | **2000–2024** | 32.0 KB | `d20a3b7357a20012ecfee57a27a29d90` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U02_MT_MEC-R132.bin` | **2000–2024** | 32.0 KB | `094566ad0d41b49e0cfa686246339381` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U11_AT_MECR109.bin` | **2000–2024** | 32.0 KB | `e4e87f33d5d8f472e110e5798c473978` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U12_AT_MECR127.bin` | **2000–2024** | 32.0 KB | `7412119766c3c2f68281ce322ff5e0b9` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U60_MT_GTS4.bin` | **2000–2024** | 32.0 KB | `ddb6089de1946f59a08c1fc266d8752d` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U70_AT_GTS4_MEC-R117.bin` | **2000–2024** | 32.0 KB | `dd0556b46d65c12992f4a04ddb8499c2` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_10U01_MEC-R210B.bin` | **2000–2024** | 32.0 KB | `8c0c6774d7eeda447331152f3d816b8a` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_10U11_MEC-217.bin` | **2000–2024** | 32.0 KB | `abfca442ef5dc9986f56b3d00d96d2bc` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U00_MT_MEC-212B.bin` | **2000–2024** | 32.0 KB | `1ff8dc2c3c1ca8a80030e0749fb98c49` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U01.bin` | **2000–2024** | 32.0 KB | `15477dcf386553002608db42f8bebe46` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U10_AT.bin` | **2000–2024** | 32.0 KB | `0ddb29f034a914b9479cd0b5601ded75` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U60_MT_MEC-214B.bin` | **2000–2024** | 32.0 KB | `e8332d3363735e60a71444699d480769` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U70_MT_MEC-215B.bin` | **2000–2024** | 32.0 KB | `1e4b87674034f30ec5ae806c14517129` | Factory Binary Firmware Dump |
| `HR31_RB20DET_45L70_AT_MEC-R50C.bin` | **2000–2024** | 16.0 KB | `b181e3cc8eccf6b06d896a8d7a9ffa71` | Factory Binary Firmware Dump |
| `HR31_RB20DET_56S13_AT_J171ADA3.bin` | **2000–2024** | 16.0 KB | `7323ddb89b74765d4af0035f49d7514f` | Factory Binary Firmware Dump |
| `HR31_RB20DET_58S12_AT_MECR12.BIN` | **2000–2024** | 16.0 KB | `98bd049507e17fa8d1d0b80724a0fe02` | Factory Binary Firmware Dump |
| `HR31_RB20DET_59S03_MT_MEC-R16.BIN` | **2000–2024** | 16.0 KB | `997169b6ea946ec91bb8b45ef0102958` | Factory Binary Firmware Dump |
| `HR31_RB20DET_59S13_AT_MEC-R17.BIN` | **2000–2024** | 16.0 KB | `411f282edad03950162f43cd01866d18` | Factory Binary Firmware Dump |
| `HR31_RB20DET_70S00_MEC-R45.bin` | **2000–2024** | 16.0 KB | `79d8f7c7e866ed2d1c04c71fc8904473` | Factory Binary Firmware Dump |
| `HR31_RB20DET_79S01_MEC-R40.bin` | **2000–2024** | 16.0 KB | `dda0b49830dacf3e753cce55b4e447b2` | Factory Binary Firmware Dump |
| `HR31_RB20DET_80503_MT_MEC-R72R_bottom.BIN` | **2000–2024** | 16.0 KB | `2e3e9d6d977b2faa42067b36f6ef545f` | Factory Binary Firmware Dump |
| `HR31_RB20DET_80S01_MEC-R42.bin` | **2000–2024** | 16.0 KB | `c6fe5218ee1dd3d1c68b4db0c0bfd426` | Factory Binary Firmware Dump |
| `HR31_RB20DET_80S11_AT_MEC-R43.BIN` | **2000–2024** | 16.0 KB | `897d26ad84be90422573b94b3a9e2609` | Factory Binary Firmware Dump |
| `HR31_RB20DET_80S12_MECR48.BIN` | **2000–2024** | 16.0 KB | `ca77b85c5cdd1d547414279e4751ac5d` | Factory Binary Firmware Dump |
| `HR31_RB20DET_MEC-R37.BIN` | **2000–2024** | 16.0 KB | `b75cb186b9be5438449cb7ca880016bc` | Factory Binary Firmware Dump |
| `HR31_RB20DET_MEC-R49_Autech.bin` | **2000–2024** | 16.0 KB | `e7a00635254c5d29736d2abf7e2c0130` | Factory Binary Firmware Dump |
| `HR31_RB20ET_76S10.bin` | **2000–2024** | 16.0 KB | `a3f8e5ce871dbc2f6f7f68c50f13ba15` | Factory Binary Firmware Dump |
| `HR33_RB20E_26U00.bin` | **2000–2024** | 32.0 KB | `acfda384e304f06476f27d5ad352b109` | Factory Binary Firmware Dump |
| `J30_VE30DE_97E10_AT.bin` | **2000–2024** | 32.0 KB | `02d7eff09e1dc6c23a56415de28230c3` | Factory Binary Firmware Dump |
| `J30_VE30DE_97E60_MT.bin` | **2000–2024** | 32.0 KB | `6df949c640d97b79d85d37fee0756ba5` | Factory Binary Firmware Dump |
| `J30_VG30DE_17Y11.bin` | **2000–2024** | 64.0 KB | `20ae91e4a4122383fa5e33a09a4bb8ef` | Factory Binary Firmware Dump |
| `J30_VG30E_87E00_MT.bin` | **2000–2024** | 32.0 KB | `ec785d75ce3ecb6f8d169c64437d2afa` | Factory Binary Firmware Dump |
| `J30_VG30E_98E00_MT_E255FFM2.bin` | **2000–2024** | 32.0 KB | `553205cc3ecbf7bc6ed972fd2638de64` | Factory Binary Firmware Dump |
| `J30_VG30_87E05_MT.BIN` | **2000–2024** | 32.0 KB | `7ec7b2a5b94cbccc13423c0e7385b842` | Factory Binary Firmware Dump |
| `J30_VG30_E255efm7.bin` | **2000–2024** | 32.0 KB | `8345a3a674eaf8610753157f48bbb668` | Factory Binary Firmware Dump |
| `K11_CG10DE_0U000k.bin` | **2000–2024** | 32.0 KB | `6bb9d6c420b28a65d176d12a5eebfcf2` | Factory Binary Firmware Dump |
| `K11_CG10DE_0U400_MT_late_64KB.bin` | **2000–2024** | 64.0 KB | `07da198d4f260adccdcfe5716da0ac6f` | Factory Binary Firmware Dump |
| `K11_CG10DE_1U210_64KB.bin` | **2000–2024** | 64.0 KB | `3d1b0fe2f593f89192f03a97a0d39950` | Factory Binary Firmware Dump |
| `K11_CG10DE_41B10_AT.bin` | **2000–2024** | 32.0 KB | `ab112bfb0d9420be076a6c179f76937f` | Factory Binary Firmware Dump |
| `K11_CG10DE_72B01_MT.bin` | **2000–2024** | 32.0 KB | `15726b911a34f5074c7b9157df9a27de` | Factory Binary Firmware Dump |
| `K11_CG13DE_1U203_64KB.bin` | **2000–2024** | 64.0 KB | `feabb92dbfc9ec8a8c31fb16b99a9159` | Factory Binary Firmware Dump |
| `K11_CG13DE_44B00_MT.bin` | **2000–2024** | 32.0 KB | `0c8776e0eaf2398b3d2aa3f907edd8f5` | Factory Binary Firmware Dump |
| `K11_CG13DE_71B00_MT.bin` | **2000–2024** | 32.0 KB | `1d1d6f37e2ea82f5bced09947c57dd66` | Factory Binary Firmware Dump |
| `K11_CG13DE_74B01_late_64KB.bin` | **2000–2024** | 64.0 KB | `5a050f229733cebcff33de16b96abf85` | Factory Binary Firmware Dump |
| `K11_CG13DE_74B61_late_64KB.bin` | **2000–2024** | 64.0 KB | `172186a8d2b1e183aacabb1d5432494c` | Factory Binary Firmware Dump |
| `K11_CG13DE_99B00_MT.bin` | **2000–2024** | 32.0 KB | `fdcb91c496a3a435eb4eb83896bd025d` | Factory Binary Firmware Dump |
| `K11_CG13DE_99B05_MT.bin` | **2000–2024** | 32.0 KB | `e9ce93b0ca29f0218a8d99feff06e8fa` | Factory Binary Firmware Dump |
| `K11_CG13DE_99B16_AT.bin` | **2000–2024** | 32.0 KB | `062d297fd0bdfe4c8097f025e0adce35` | Factory Binary Firmware Dump |
| `K11_CG13DE_99B60_AT.bin` | **2000–2024** | 32.0 KB | `40df7cbf4f8428a810eebe37b0cf5010` | Factory Binary Firmware Dump |
| `K11_CG13DE_99B65_AT.bin` | **2000–2024** | 32.0 KB | `12eb146c3098260c06befdd03b3632da` | Factory Binary Firmware Dump |
| `KN13_CA18DE_02Y01_MT_USDM_1989_Fed.BIN` | **1989** | 16.0 KB | `9ac79b458b1884824d065a14abec245a` | Factory Binary Firmware Dump |
| `KN13_CA18DE_02Y03_MT_USDM_1988_Fed.BIN` | **1988** | 16.0 KB | `2acee03af1e9980afc900b952f09ef97` | Factory Binary Firmware Dump |
| `M30_VG30_F6610_K255AFA6.bin` | **2000–2024** | 32.0 KB | `8c514144cc154405a515a3f15d0f7b88` | Factory Binary Firmware Dump |
| `M30_VG30_F6610_TB45MAPS.bin` | **2000–2024** | 32.0 KB | `4cf08a8764c61f9d3e8654eec639ec8f` | Factory Binary Firmware Dump |
| `M30_VG30_F6615_AT_1990.bin` | **1990** | 32.0 KB | `6bae5f47ca7cb114377b94df24afe270` | Factory Binary Firmware Dump |
| `M30_VG30_F6670_AT_1991.bin` | **1991** | 32.0 KB | `cdd68cb4ddfb7cd919f592b27a9a752e` | Factory Binary Firmware Dump |
| `M30_VG30_F6675_AT_1991.bin` | **1991** | 32.0 KB | `d1cc20d7dc9279a9a27e4ecc754203eb` | Factory Binary Firmware Dump |
| `N12_E15ET_28M04_MT_N306P5T1.bin` | **2000–2024** | 16.0 KB | `d1be06cdb2add1a025e2c53d17c0afa8` | Factory Binary Firmware Dump |
| `N12_E15ET_28M04_MT_V2.bin` | **2000–2024** | 16.0 KB | `67b1f5c0590afe3de2eb31ed1327d062` | Factory Binary Firmware Dump |
| `N13_CA16DE_64M00_MT.bin` | **2000–2024** | 16.0 KB | `96f205eb6f805f43b9723b4ec10e360f` | Factory Binary Firmware Dump |
| `N13_CA16DE_65M00_CA18DE.BIN` | **2000–2024** | 16.0 KB | `f2c8e6bcd33ca4740a9c2169a1fd6548` | Factory Binary Firmware Dump |
| `N13_CA16DE_82M00_MT_MEC-410_1987.bin` | **1987** | 16.0 KB | `6855e24f85164f42dcf1d60dad3a1e92` | Factory Binary Firmware Dump |
| `N14_GA16DE_65C05.bin` | **2000–2024** | 32.0 KB | `e2265bdce336a312b76832ef5f37347e` | Factory Binary Firmware Dump |
| `N14_SR18DE_58Y01_MT.bin` | **2000–2024** | 32.0 KB | `694e2f455abbe00fcd6159b2182f689c` | Factory Binary Firmware Dump |
| `N14_SR20DE_68C00_MT.bin` | **2000–2024** | 32.0 KB | `a52526d269d4b476469f673bc7896c6b` | Factory Binary Firmware Dump |
| `N14_SR20DE_68C10_MT.bin` | **2000–2024** | 32.0 KB | `1084b0cab4b7246a83072ede3748b2d7` | Factory Binary Firmware Dump |
| `N15A_GA16DE_1N900_MT.bin` | **2000–2024** | 64.0 KB | `5add29f4126df28b829e7e051c67d56c` | Factory Binary Firmware Dump |
| `N15A_GA16DE_1N910_AT.bin` | **2000–2024** | 64.0 KB | `7a1d136bcfbd0229b1ef592a4141d750` | Factory Binary Firmware Dump |
| `N15_SR20DE_0A540_autech.bin` | **2000–2024** | 32.0 KB | `71052fd41e5de21a3de1b844c92d0f4d` | Factory Binary Firmware Dump |
| `N15_SR20DE_1N401_MT.bin` | **2000–2024** | 64.0 KB | `4f775ebfc94697672805407e5f217596` | Factory Binary Firmware Dump |
| `N15_SR20DE_1N410_AT.bin` | **2000–2024** | 64.0 KB | `7bf39570856177090a6d17a08a3d6705` | Factory Binary Firmware Dump |
| `N15_SR20DE_1N411_AT.bin` | **2000–2024** | 64.0 KB | `e323c4a069199505732af00e86a6a8a4` | Factory Binary Firmware Dump |
| `N15_SR20DE_1N960_MT.bin` | **2000–2024** | 32.0 KB | `1fc4156a0b75342539e9ace75ee1739b` | Factory Binary Firmware Dump |
| `P10_SR18DE_0J312_AT.Bin` | **2000–2024** | 32.0 KB | `e6d6bab348b93302adb2869bd7c0f18f` | Factory Binary Firmware Dump |
| `P10_SR20DE_0J261_MT.bin` | **2000–2024** | 32.0 KB | `280e4df75a97191f467a6447ebf1ac8c` | Factory Binary Firmware Dump |
| `P10_SR20DE_5J000_MT_1993.bin` | **1993** | 32.0 KB | `ec8871ee15254a9de3597047add0a02e` | Factory Binary Firmware Dump |
| `P10_SR20DE_62J00_MT_1991.bin` | **1991** | 32.0 KB | `2728545230b72b72c6f3fb69db9ff100` | Factory Binary Firmware Dump |
| `P10_SR20DE_63J11_AT_1991.bin` | **1991** | 32.0 KB | `6c898664e609eee69e1eda915a5aa34e` | Factory Binary Firmware Dump |
| `P10_SR20DE_70J00_MT.bin` | **2000–2024** | 32.0 KB | `3161a9b16365c6177a041950d9e46c05` | Factory Binary Firmware Dump |
| `P10_SR20DE_70J10_AT_1993.bin` | **1993** | 32.0 KB | `a45ce8b6d2b26f96dd5580e50af24733` | Factory Binary Firmware Dump |
| `P10_SR20DE_70J15_AT_1993.bin` | **1993** | 32.0 KB | `c3a49283e6f39e068855172016727475` | Factory Binary Firmware Dump |
| `P10_SR20DE_71C00_MT.bin` | **2000–2024** | 32.0 KB | `930e8eaab5c7d46b3d6a8f54d4c4a137` | Factory Binary Firmware Dump |
| `P10_SR20DE_77J00_MT_1992.bin` | **1992** | 32.0 KB | `4f413e0813b9ed6de986deda9b2972e4` | Factory Binary Firmware Dump |
| `P10_SR20DE_83J00_MT_1994.bin` | **1994** | 64.0 KB | `95b399eea4cd1a34daf07e0c939d2d73` | Factory Binary Firmware Dump |
| `P10_SR20DE_83J10.bin` | **2000–2024** | 64.0 KB | `81a4b5e7377004598391d424c9f9c163` | Factory Binary Firmware Dump |
| `P10_SR20DE_83J14.bin` | **2000–2024** | 64.0 KB | `cb9b3e9fd2d0ef83904eb8e41a7dd500` | Factory Binary Firmware Dump |
| `P10_SR20DI_70J81_1992.bin` | **1992** | 32.0 KB | `af1210a2e29ff5b1f402db07d7a57667` | Factory Binary Firmware Dump |
| `P11_SR18DE_79J71.bin` | **2000–2024** | 32.0 KB | `761d482cdeb83757188d901258b5619a` | Factory Binary Firmware Dump |
| `P11_SR20DE_2J200_MT.bin` | **2000–2024** | 64.0 KB | `7ace6e56db10e83305cba1fa0a1ec57f` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J400.bin` | **2000–2024** | 64.0 KB | `f2a731552e2e3938cf35b80d0b444eb2` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J403_MT.bin` | **2000–2024** | 64.0 KB | `16f0401dc3b14036556b88b91337bf26` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J404.bin` | **2000–2024** | 64.0 KB | `36c75f7a09b46ed0ee7c24771bda8009` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J461_MT.bin` | **2000–2024** | 64.0 KB | `201bad7e968fabac81040954c9d283c3` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J501_MT.bin` | **2000–2024** | 64.0 KB | `777a4c986c016daee5cf9ead59334dc7` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J503_MT.bin` | **2000–2024** | 64.0 KB | `2b625fecd347af90269a42ff37d277fd` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J504_MT.bin` | **2000–2024** | 64.0 KB | `150197b66eccc0fd354c6bdb40d893ce` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J800_MT.bin` | **2000–2024** | 64.0 KB | `f016449234ed09cae079ca8df748959a` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J801_MT.bin` | **2000–2024** | 64.0 KB | `7da7a92ad387f69742f8b768474de845` | Factory Binary Firmware Dump |
| `P11_SR20DE_3J905_MT.bin` | **2000–2024** | 64.0 KB | `412fff0bae31d313e564a63ea1eefed1` | Factory Binary Firmware Dump |
| `P11_SR20DE_7J100_1999_MT.bin` | **1999** | 64.0 KB | `c95abfbaba8169b4f9150ca9b3a0353b` | Factory Binary Firmware Dump |
| `PW10_SR20DE_78N05.bin` | **2000–2024** | 32.0 KB | `6fe9d8d7bf21e0ed7fbf4a134b573b47` | Factory Binary Firmware Dump |
| `Q45_VH45DE_60U00_MT.bin` | **2000–2024** | 32.0 KB | `7d8d300bbdb76330e9a264a5f7485ad0` | Factory Binary Firmware Dump |
| `Q45_VH45DE_61U00_MT.bin` | **2000–2024** | 32.0 KB | `5fce6e1e96ddd4a6187ad0fd41c98606` | Factory Binary Firmware Dump |
| `Q45_VH45DE_62U00_MT.bin` | **2000–2024** | 32.0 KB | `73f300c6ee2498e8aec3e063356ab21a` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U00_MT.bin` | **2000–2024** | 32.0 KB | `797c7f5d7c92806e155765c8e034c867` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U01_MT.bin` | **2000–2024** | 32.0 KB | `63b6638e33fdf466186af59587627ae7` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U04_MT.bin` | **2000–2024** | 32.0 KB | `b161f9f54098add363c18a106d690d04` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U05_MT.bin` | **2000–2024** | 32.0 KB | `80d86e7b07cb08cfb776f536554632aa` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U06_MT.bin` | **2000–2024** | 32.0 KB | `a69c14d03d11a049057a9c0a506d0cae` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U07_MT.bin` | **2000–2024** | 32.0 KB | `85b6935643d9fa7b3771125cbe759056` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U08_MT.bin` | **2000–2024** | 32.0 KB | `5e97139ac0698692d5d71217e4075e71` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U09_MT.bin` | **2000–2024** | 32.0 KB | `f2643940a20584ac231e53f2031b5d29` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U10_AT.bin` | **2000–2024** | 32.0 KB | `031ad156953341a69aff46b3a8be2024` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U12_AT.bin` | **2000–2024** | 32.0 KB | `4dc6487d62a886892f96b238696ea599` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U21.bin` | **2000–2024** | 32.0 KB | `76c362453bc71fe33333577b4778f647` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U61_MT.bin` | **2000–2024** | 32.0 KB | `b2fe1da37fbbaa78f507d12f0883afbb` | Factory Binary Firmware Dump |
| `Q45_VH45DE_64U65_MT.bin` | **2000–2024** | 32.0 KB | `58e2c4e775ddee7f4534c117cedd547f` | Factory Binary Firmware Dump |
| `Q45_VH45DE_66U15_AT.bin` | **2000–2024** | 32.0 KB | `41b33dab6c4c03233f7f761152a23176` | Factory Binary Firmware Dump |
| `Q45_VH45DE_71U04_MT.bin` | **2000–2024** | 32.0 KB | `ee59e1af86c6f722323d7df38e59a371` | Factory Binary Firmware Dump |
| `Q45_VH45DE_71U12_MT.bin` | **2000–2024** | 32.0 KB | `e5061b2a8546c1d81c257b2365f07a6b` | Factory Binary Firmware Dump |
| `R30_FJ20DET_R2201_MT.bin` | **2000–2024** | 16.0 KB | `ed2c401c0ab9b895420fbc35228f238c` | Factory Binary Firmware Dump |
| `RNN14_SR20DET_54C00_MT_JDM.bin` | **2000–2024** | 32.0 KB | `277f24660b86ae3b98bff0c6c0f84503` | Factory Binary Firmware Dump |
| `RNN14_SR20DET_54C60_MT_JDM.bin` | **2000–2024** | 32.0 KB | `ac105a25cd4fc99857c790ae9b42761f` | Factory Binary Firmware Dump |
| `RNN14_SR20DET_69C05_MT_EDM.bin` | **2000–2024** | 32.0 KB | `dabddc8ee52bdbfc4fba70f959e7cf50` | Factory Binary Firmware Dump |
| `RNU12_CA18DET_MT.BIN` | **2000–2024** | 16.0 KB | `b805876e212d48354c6f76c9c8f41ae0` | Factory Binary Firmware Dump |
| `RS13_CA18DET_36F05_MT_MEC-D016B_JDM.BIN` | **2000–2024** | 16.0 KB | `0f5ad2f35c42be75762286e35e7165f9` | Factory Binary Firmware Dump |
| `RS13_CA18DET_36F11_MT_MEC-D015A_JDM.bin` | **2000–2024** | 16.0 KB | `af77544fbae4cab817b07968a1035e4f` | Factory Binary Firmware Dump |
| `RS13_CA18DET_36F15_MT_MEC-D017B_JDM.bin` | **2000–2024** | 16.0 KB | `bebe8049b8a032a3eb75e3b045af95de` | Factory Binary Firmware Dump |
| `S12_CA18ET_21F13_c321aem4.BIN` | **2000–2024** | 16.0 KB | `600ebaae8e372060d0ee8c10ff280858` | Factory Binary Firmware Dump |
| `S12_CA18ET_30F00_MT_MEC-450.bin` | **2000–2024** | 16.0 KB | `33145502e166e644258d4d024f56033b` | Factory Binary Firmware Dump |
| `S12_CA18ET_30F10_AT_MEC-550.bin` | **2000–2024** | 16.0 KB | `171e84dfc3ab7bd30a1588cacd25c489` | Factory Binary Firmware Dump |
| `S12_CA18ET_33F01.bin` | **2000–2024** | 16.0 KB | `d081680597cf5de4b59d0987b329f1b0` | Factory Binary Firmware Dump |
| `S13_CA18DET_36F00_MEC-D003E2_JDM_MT.BIN` | **2000–2024** | 16.0 KB | `8d093ce78e9fefb1cf0afbd56589575a` | Factory Binary Firmware Dump |
| `S13_CA18DET_39F00_MEC-D007D_EDM_MT.bin` | **2000–2024** | 16.0 KB | `06f9690cc16ba3cff5a2c646e719a4c2` | Factory Binary Firmware Dump |
| `S13_CA18DET_44F02_MT_MEC-D005B.bin` | **2000–2024** | 16.0 KB | `d542e97f3f16daa16138dfd83f0cc993` | Factory Binary Firmware Dump |
| `S13_CA18DET_44F06_MT_MEC-D022A.bin` | **2000–2024** | 16.0 KB | `d33715f9123c2db041b63e030d446cae` | Factory Binary Firmware Dump |
| `S13_CA18DET_44F07_MT_MEC-D009D.bin` | **2000–2024** | 16.0 KB | `32c47cdb71f78cbeff9c87e7cee6c806` | Factory Binary Firmware Dump |
| `S13_CA18DET_MEC-D010C.bin` | **2000–2024** | 16.0 KB | `dde23d1544d95292a1ab8c3d14651763` | Factory Binary Firmware Dump |
| `S13_CA18DE_35F00_MEC-D001_JDM_MT.bin` | **2000–2024** | 16.0 KB | `8ed4aa67ca2536ea4fcf863fc87cf630` | Factory Binary Firmware Dump |
| `S13_CA18DE_35F11_MEC-D014.bin` | **2000–2024** | 16.0 KB | `7c12747ce5742ed8077ceefb48d83a6b` | Factory Binary Firmware Dump |
| `S13_CA18DE_35F11_MEC-R015_JDM_AT.bin` | **2000–2024** | 16.0 KB | `a024ce34b38663645e82f1eeae730739` | Factory Binary Firmware Dump |
| `S13_CA18ET_D4600_MT.bin` | **2000–2024** | 16.0 KB | `1575e79f029e5d7d23255a136465db2f` | Factory Binary Firmware Dump |
| `S13_KA24DE_51F11.bin` | **2000–2024** | 32.0 KB | `6ba818fe246b5d5a5cd7c472c4179c1c` | Factory Binary Firmware Dump |
| `S13_KA24DE_53F00_MT_1991_FED.bin` | **1991** | 32.0 KB | `6db8e508e0ffb835ca45bc7f9fda5d09` | Factory Binary Firmware Dump |
| `S13_KA24DE_53F01_MT_1993_FED.bin` | **1993** | 32.0 KB | `66f844d53df7ed1ab12e5b03c867b558` | Factory Binary Firmware Dump |
| `S13_KA24DE_53F10_AT_1991.bin` | **1991** | 32.0 KB | `4a71309a0c974e8d4d8417690d7e8610` | Factory Binary Firmware Dump |
| `S13_KA24DE_53F11_MT_1991_FED.bin` | **1991** | 32.0 KB | `aa8e8f18468fa6f3b68162bc3088ea1f` | Factory Binary Firmware Dump |
| `S13_KA24DE_54F00_MT.bin` | **2000–2024** | 32.0 KB | `5f193a7d8e83286a594dd7844ecd1286` | Factory Binary Firmware Dump |
| `S13_KA24DE_54F02_MT.BIN` | **2000–2024** | 32.0 KB | `d02d34e7fc328aec66c38a23452d56ac` | Factory Binary Firmware Dump |
| `S13_KA24DE_54F10_AT_CAL.bin` | **2000–2024** | 32.0 KB | `2629af5e6db0081fcd560fb61756f1eb` | Factory Binary Firmware Dump |
| `S13_KA24DE_54F12_AT.bin` | **2000–2024** | 32.0 KB | `e896d7d43df53d7be5446b44b45ca1a0` | Factory Binary Firmware Dump |
| `S13_KA24DE_59F10_AT.bin` | **2000–2024** | 32.0 KB | `d9f477ca20c4cf7b0ea52403f4356631` | Factory Binary Firmware Dump |
| `S13_KA24DE_59F12_AT_1994_FED.bin` | **1994** | 32.0 KB | `dc07b7afc1d50250d23769b6b093dc80` | Factory Binary Firmware Dump |
| `S13_KA24DE_59F16_AT_CAL.bin` | **2000–2024** | 32.0 KB | `d049787b32795a19f19db817d7eeca98` | Factory Binary Firmware Dump |
| `S13_KA24E_40F0X_1990_MT_FED.bin` | **1990** | 32.0 KB | `9c0bca9b033e319feef8cebc2950a79a` | Factory Binary Firmware Dump |
| `S13_KA24E_42F61_89_AT_CALI.bin` | **2000–2024** | 32.0 KB | `a6a6e289e7be101fed44781bd7be5ba8` | Factory Binary Firmware Dump |
| `S13_KA24E_42F62_89_AT_CALI.BIN` | **2000–2024** | 32.0 KB | `4f3a093811ff0450ff56845c1bef8da9` | Factory Binary Firmware Dump |
| `S13_KA24E_42F65_89_AT_CALI.bin` | **2000–2024** | 32.0 KB | `76281edc30ab19f097505787125bb1f3` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F00_MT_red_top.bin` | **2000–2024** | 32.0 KB | `331c675160d4b3a2f8e6c2fc7643c70b` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F01_MT.bin` | **2000–2024** | 32.0 KB | `ed637f93635ab118fba7a530af15b468` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F05_MT_black_top.bin` | **2000–2024** | 32.0 KB | `dd65894d26d7b081ce2138ae7f4e52b6` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F10_AT.bin` | **2000–2024** | 32.0 KB | `c5c53a6a5724e98b36b37a4fa2eb0df4` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F11_AT.bin` | **2000–2024** | 32.0 KB | `c6de968d6c92d05fa8f29d3d864a535a` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F15_AT.bin` | **2000–2024** | 32.0 KB | `4890359a20d053b80d122a3ebc4b8ece` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F06_MT_TypeX.bin` | **2000–2024** | 32.0 KB | `5ff40c110fa7bc294942198a79bc1067` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F07_TypeX.bin` | **2000–2024** | 32.0 KB | `fa1ffcb7f80b833c34df801ec5033a7d` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F16_TypeX.bin` | **2000–2024** | 32.0 KB | `e0218e51b46b0957f3403bdbecb4efb1` | Factory Binary Firmware Dump |
| `S13_SR20DE_52F00_MT.bin` | **2000–2024** | 32.0 KB | `6d019045a4a262e860eede2629746d9c` | Factory Binary Firmware Dump |
| `S13_SR20DE_52F10_AT.bin` | **2000–2024** | 32.0 KB | `acd33e19c2212ad06df648e77edd6316` | Factory Binary Firmware Dump |
| `S13_SR20DE_60F00_TypeS.bin` | **2000–2024** | 32.0 KB | `c8d7a684399b7048f6c67e3561a3cbdf` | Factory Binary Firmware Dump |
| `S13_SR20DE_60F10_TypeS.bin` | **2000–2024** | 32.0 KB | `faa388aad4e53acb0c190d451b8ec066` | Factory Binary Firmware Dump |
| `S14_KA24DE_70F00_MT_1995.bin` | **1995** | 64.0 KB | `9faec6ca61efaca6ef3f2d2fa64ca4e6` | Factory Binary Firmware Dump |
| `S14_KA24DE_70F01_MT.bin` | **2000–2024** | 64.0 KB | `b0cf99a0baf72bff7afa1344185b2195` | Factory Binary Firmware Dump |
| `S14_KA24DE_70F02.bin` | **2000–2024** | 64.0 KB | `5659ead04d997791016bafacb7bbf467` | Factory Binary Firmware Dump |
| `S14_KA24DE_70F03_MT.bin` | **2000–2024** | 64.0 KB | `efb569cb69d74005eaa52264a81d59f6` | Factory Binary Firmware Dump |
| `S14_KA24DE_70F05_AT.bin` | **2000–2024** | 64.0 KB | `eb61fe845acd10e0ed93e4c4797601f8` | Factory Binary Firmware Dump |
| `S14_KA24DE_70F06.bin` | **2000–2024** | 64.0 KB | `553f9419a28a8b460a3644e1b0cb77fd` | Factory Binary Firmware Dump |
| `S14_KA24DE_70F08_AT.bin` | **2000–2024** | 64.0 KB | `1e5416388a671a518e827d58a6194fdf` | Factory Binary Firmware Dump |
| `S14_KA24DE_70F10_AT_1995.bin` | **1995** | 64.0 KB | `93c76c9fc894eccf65a83290fab4d47c` | Factory Binary Firmware Dump |
| `S14_KA24DE_72F01_MT.bin` | **2000–2024** | 64.0 KB | `1818528bc248fde1f0462b0d84633d24` | Factory Binary Firmware Dump |
| `S14_KA24DE_72F13_AT.bin` | **2000–2024** | 64.0 KB | `717052f81e8c6e8fc0923c3803106ade` | Factory Binary Firmware Dump |
| `S14_SR20DET_69F00_MT.bin` | **2000–2024** | 64.0 KB | `cbb54f9c2c9cd146b34b6ff458ca5ddf` | Factory Binary Firmware Dump |
| `S14_SR20DET_69F01_MT.bin` | **2000–2024** | 64.0 KB | `586a0842d7bf4fbb1085b653589819bd` | Factory Binary Firmware Dump |
| `S14_SR20DET_69F10.bin` | **2000–2024** | 64.0 KB | `c5ce1f7c5f353e07391628975a54e468` | Factory Binary Firmware Dump |
| `S14_SR20DET_74F00_MT.bin` | **2000–2024** | 64.0 KB | `d0cf290091084af398c9788fd6cc6247` | Factory Binary Firmware Dump |
| `S14_SR20DET_74F01_MT.BIN` | **2000–2024** | 64.0 KB | `d99270c5f466738849eb5270aaf07284` | Factory Binary Firmware Dump |
| `S14_SR20DET_74F05_MT.BIN` | **2000–2024** | 64.0 KB | `7ca2454dfe3768a175d848660cead1b2` | Factory Binary Firmware Dump |
| `S14_SR20DET_74F05_s14a-wiring.bin` | **2000–2024** | 64.0 KB | `3fb047c9957ddec63770231ac107ba97` | Factory Binary Firmware Dump |
| `S14_SR20DET_74F10_AT.bin` | **2000–2024** | 64.0 KB | `fea774e02733d102a74918f88f92cd79` | Factory Binary Firmware Dump |
| `S14_SR20DET_74F11_AT.bin` | **2000–2024** | 64.0 KB | `e73665ce855043933eadb784d4c2948f` | Factory Binary Firmware Dump |
| `S14_SR20DET_74F15_s14a-wiring.bin` | **2000–2024** | 64.0 KB | `95f0a8db6f4f0b13d3dccb268f947853` | Factory Binary Firmware Dump |
| `S14_SR20DET_75F00_MT_NATS_EDM.bin` | **2000–2024** | 64.0 KB | `9f19ebc7c2407380c3dcc0da061e65c2` | Factory Binary Firmware Dump |
| `S14_SR20DET_75F01_MT_NATS_EDM.bin` | **2000–2024** | 64.0 KB | `1d4fe375da301136a38c02c448dd51c2` | Factory Binary Firmware Dump |
| `S14_SR20DET_75F10_AT_NATS_EDM.bin` | **2000–2024** | 64.0 KB | `dafc6b5b0348adb1f1e5da363abad92d` | Factory Binary Firmware Dump |
| `S14_SR20DET_80F00_MT_JDM.bin` | **2000–2024** | 64.0 KB | `8f2ba0660c957b44069b3247343adcff` | Factory Binary Firmware Dump |
| `S14_SR20DET_80F10_MT_JDM.bin` | **2000–2024** | 64.0 KB | `df9356da91f3b6430ef5dce42e356f15` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F00_MT_EDM.bin` | **2000–2024** | 64.0 KB | `12e2e790352715b7bb2aa288bb32c61d` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F01_MT_EDM.bin` | **2000–2024** | 64.0 KB | `5a5289c1aa104281f001835d0f9bd1ea` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F04_MT_EDM.bin` | **2000–2024** | 64.0 KB | `64228cbe4c138278fb5d65ae431e07b9` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F05_MT_EDM.bin` | **2000–2024** | 64.0 KB | `f12c8db6b5f9b47ff899f858a8c33218` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F06_MT_EDM.bin` | **2000–2024** | 64.0 KB | `e318593b2ad2e862f48c9695bd5f4d4a` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F08_MT_EDM.BIN` | **2000–2024** | 64.0 KB | `1a8f4cf398d937c031104d9820b1868b` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F14_AT_EDM.bin` | **2000–2024** | 64.0 KB | `a9eb4fc1e2ffc7d4b7dcc6255f3cc646` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F15_AT_EDM.bin` | **2000–2024** | 64.0 KB | `42913248be7c49950c41db52330dd5b6` | Factory Binary Firmware Dump |
| `S14_SR20DET_82F18_MT_EDM.BIN` | **2000–2024** | 64.0 KB | `c4ee2a9e17e773bc51bbfef21329ed71` | Factory Binary Firmware Dump |
| `S14_SR20DET_83F00_MT_ADM.bin` | **2000–2024** | 64.0 KB | `7e00754a2a85fc9cf0ce3254e8a16e57` | Factory Binary Firmware Dump |
| `S14_SR20DET_83F05.bin` | **2000–2024** | 64.0 KB | `b8fe134d3b130caedc3d58647a162c9c` | Factory Binary Firmware Dump |
| `S14_SR20DET_83F10_AT_ADM.bin` | **2000–2024** | 64.0 KB | `3e452f620783d002bd32dbe0f219b485` | Factory Binary Firmware Dump |
| `S14_SR20DE_65F00_MT.bin` | **2000–2024** | 32.0 KB | `7f6dc89aa87d22bdc829a7a82f432772` | Factory Binary Firmware Dump |
| `S14_SR20DE_65F00_MT_knockadj.bin` | **2000–2024** | 32.0 KB | `068565b1fd1373cbf2218959dff77aa1` | Factory Binary Firmware Dump |
| `S14_SR20DE_65F10_AT.bin` | **2000–2024** | 32.0 KB | `78c3fc9a2aa33f1e2f46bd73c596866a` | Factory Binary Firmware Dump |
| `S15_SR20DET_91F00_MT_JDM.bin` | **2000–2024** | 64.0 KB | `8947e5ed75a8e1ebf45ac2fec21d4a3f` | Factory Binary Firmware Dump |
| `S15_SR20DET_91F01_MT_JDM.bin` | **2000–2024** | 64.0 KB | `543c40cf57ff0e64f6abf37ab319f58d` | Factory Binary Firmware Dump |
| `S15_SR20DET_91F05_MT_JDM.bin` | **2000–2024** | 64.0 KB | `dcdbd7a4974146b7cdc4890909694e19` | Factory Binary Firmware Dump |
| `S15_SR20DET_91F06_MT_JDM.bin` | **2000–2024** | 64.0 KB | `c638b1129d7d62b2bdf8ea33311a4bf4` | Factory Binary Firmware Dump |
| `S15_SR20DET_91F07_MT_JDM.bin` | **2000–2024** | 64.0 KB | `f6b92f48d0f8a44d32f25bc282b87c10` | Factory Binary Firmware Dump |
| `S15_SR20DET_91F08_MT_JDM.bin` | **2000–2024** | 64.0 KB | `2fca7584f32baed063b2ffa911cf23a0` | Factory Binary Firmware Dump |
| `S15_SR20DET_91F10_AT_JDM.bin` | **2000–2024** | 64.0 KB | `1e31ba00f22e7d0a89409e39ae302d5e` | Factory Binary Firmware Dump |
| `S15_SR20DET_91F15_AT_JDM.bin` | **2000–2024** | 64.0 KB | `d79bc0880183197fad5f2435fcd0134c` | Factory Binary Firmware Dump |
| `S15_SR20DET_93F00_MT_ADM.bin` | **2000–2024** | 64.0 KB | `93ec12a4a928afcf0320588985182126` | Factory Binary Firmware Dump |
| `S15_SR20DET_93F10_AT_ADM.bin` | **2000–2024** | 64.0 KB | `4da935e81fa573c3c12190a25a54b817` | Factory Binary Firmware Dump |
| `U11_VG30E_56U62.bin` | **2000–2024** | 64.0 KB | `3e0412fcbb77116d06013b4bce3eee79` | Factory Binary Firmware Dump |
| `U12_CA18DET_56E62_MEC-C006C.bin` | **2000–2024** | 16.0 KB | `cc3a730aa751a1c34b0197c1f46f0195` | Factory Binary Firmware Dump |
| `U12_CA18DET_56E70_MEC-C006.bin` | **2000–2024** | 16.0 KB | `c8dfecd7c7a6ba8d97290db6075b1373` | Factory Binary Firmware Dump |
| `U12_KA24E_65E01.bin` | **2000–2024** | 32.0 KB | `c5eba27c63bce8c528537c4972d29f12` | Factory Binary Firmware Dump |
| `U12_KA24E_65E14.bin` | **2000–2024** | 32.0 KB | `c4c5473cdea9d23ceb499a0a48d473d1` | Factory Binary Firmware Dump |
| `U12_KA24E_95E03_E480AAM6.bin` | **2000–2024** | 32.0 KB | `4fac71b7c2db9fb70db76ddc457abc1a` | Factory Binary Firmware Dump |
| `U12_KA24E_95E11.bin` | **2000–2024** | 32.0 KB | `de1753e5b02a6c6cc11e916a8a6b56e0` | Factory Binary Firmware Dump |
| `U12_SR20DET_5E200_MT.bin` | **2000–2024** | 32.0 KB | `0a6fb27b9b4b13a3b510f5341225f13b` | Factory Binary Firmware Dump |
| `U12_SR20DET_79E01_MT.bin` | **2000–2024** | 32.0 KB | `84d5fa21d55ab933603912b827825846` | Factory Binary Firmware Dump |
| `U12_SR20DET_79E10_AT.bin` | **2000–2024** | 32.0 KB | `43abf7890d97f4405149fba32ffa7e90` | Factory Binary Firmware Dump |
| `U12_SR20DET_79E11_AT.bin` | **2000–2024** | 32.0 KB | `e1d18599f66ce685876f5671a0ba84b0` | Factory Binary Firmware Dump |
| `U13_KA24DE_1E460_1993_MT_Altima.bin` | **1993** | 64.0 KB | `3a5ad2141fef2c15432ca2422a808819` | Factory Binary Firmware Dump |
| `U13_KA24DE_1E470_1993_AT_Altima.bin` | **1993** | 64.0 KB | `cfa530e3c53ac68b05a4a23d79ea3d03` | Factory Binary Firmware Dump |
| `U13_KA24DE_3E600_1994_JDM_MT.bin` | **1994** | 64.0 KB | `2d88ddc17f03ffcd6134e190761858bf` | Factory Binary Firmware Dump |
| `U13_KA24DE_4E800_1995_FED_MT.bin` | **1995** | 64.0 KB | `082a3da4a270d4d9948fd322dbd1721c` | Factory Binary Firmware Dump |
| `U13_SR20DET_1E000_MT.bin` | **2000–2024** | 32.0 KB | `bba6ac8ca32cce54720d42e8801991c7` | Factory Binary Firmware Dump |
| `U13_SR20DET_1E010.bin` | **2000–2024** | 32.0 KB | `b48033ecb5af7eebb2ee5494949f6f0a` | Factory Binary Firmware Dump |
| `U13_SR20DET_4E610_AT.bin` | **2000–2024** | 32.0 KB | `9e8099af8711e6ab8c189db8fde940c2` | Factory Binary Firmware Dump |
| `UC32-VG30E.bin` | **2000–2024** | 16.0 KB | `65efcd9bd6f83b50eadd154e7372abda` | Factory Binary Firmware Dump |
| `VL_RB30ET_B4903_MT.bin` | **2000–2024** | 16.0 KB | `7b2dfea275f0cad3c536cd06920c32d6` | Factory Binary Firmware Dump |
| `VL_RB30ET_B4913_AT.bin` | **2000–2024** | 16.0 KB | `fe8210907b8d1ae9281f63ee7c300062` | Factory Binary Firmware Dump |
| `VL_RB30E_AT.bin` | **2000–2024** | 16.0 KB | `3980cf401b6b94cd285cc08d8830c4c7` | Factory Binary Firmware Dump |
| `VL_RB30E_MT.bin` | **2000–2024** | 16.0 KB | `afa9f0be8fb25018df81cab61b662317` | Factory Binary Firmware Dump |
| `W10_SR20DET_95N11.bin` | **2000–2024** | 32.0 KB | `9c31296760b82bcf5a7bac76e1b60fca` | Factory Binary Firmware Dump |
| `W10_SR20DET_95N15.bin` | **2000–2024** | 32.0 KB | `65213f015c63e759af6d1128e57f021e` | Factory Binary Firmware Dump |
| `WC34_RB25DET_0V810_4WD_AT.bin` | **2000–2024** | 64.0 KB | `0969a0e00cf33f85e33c024cbe272395` | Factory Binary Firmware Dump |
| `WC34_RB25DET_0V811_4WD_AT.bin` | **2000–2024** | 64.0 KB | `09020ebf815d3966000a87dce9c3bbb1` | Factory Binary Firmware Dump |
| `WC34_RB25DET_0V812_4WD_AT.bin` | **2000–2024** | 64.0 KB | `4bf4a865eb9e35b2474b3b83c63769b2` | Factory Binary Firmware Dump |
| `WC34_RB25DET_0V813_4WD_AT.bin` | **2000–2024** | 64.0 KB | `495f965c068e4bd350ec392712d3cdf8` | Factory Binary Firmware Dump |
| `WC34_RB25DET_23710_0V800_4WD_MT.bin` | **2000–2024** | 64.0 KB | `334068e2d5316327d151c0c10569c324` | Factory Binary Firmware Dump |
| `WC34_RB25DET_23710_0V801_4WD_MT.bin` | **2000–2024** | 64.0 KB | `1af14d59b414f071b27cbff2c7e97579` | Factory Binary Firmware Dump |
| `WC34_RB25DET_23740_0V800_2WD_AT.BIN` | **2000–2024** | 64.0 KB | `a42b092d732272f53094e1b384781963` | Factory Binary Firmware Dump |
| `WC34_RB25DET_23740_0V802_2WD_AT.bin` | **2000–2024** | 64.0 KB | `96b596d73bccc587150e98bb3fa1c7d5` | Factory Binary Firmware Dump |
| `WC34_RB25DET_23740_0V810_4WD_AT.bin` | **2000–2024** | 64.0 KB | `fd79b160007103c4bf735f79831fd980` | Factory Binary Firmware Dump |
| `Y30_VG30ET_MECV16.bin` | **2000–2024** | 16.0 KB | `6fa8a172b49f3c4d08951e209a18a0bb` | Factory Binary Firmware Dump |
| `Y31_VG20DET_71V10_AT_MECE101.BIN` | **2000–2024** | 32.0 KB | `215ee2784796c1add52bba24c4185993` | Factory Binary Firmware Dump |
| `Y31_VG30DET_71V70_AT.bin` | **2000–2024** | 32.0 KB | `76d13474d81e52d0c99b27c99f6e70fa` | Factory Binary Firmware Dump |
| `Y32_VG30DET_0P501_MT.bin` | **2000–2024** | 32.0 KB | `c398c6d4f8267167aa70a0bf6a9a1083` | Factory Binary Firmware Dump |
| `Y32_VG30DET_0P602_MT_1992_Gloria.BIN` | **1992** | 32.0 KB | `0adf8903f6165f6f36946642851cfb9b` | Factory Binary Firmware Dump |
| `Y32_VG30DET_OP660.BIN` | **2000–2024** | 32.0 KB | `152c4715e0778d674ba94514f36101ca` | Factory Binary Firmware Dump |
| `Y32_VH41DE_1P121-Tuned.bin` | **2000–2024** | 32.0 KB | `ab0434a154e36d16d71dc9fb89f1e394` | Factory Binary Firmware Dump |
| `Y33_VQ30DET_4P200_MT.bin` | **2000–2024** | 64.0 KB | `08d9dabd221ea1877954bdec2d74623b` | Factory Binary Firmware Dump |
| `Y33_VQ30DET_4P201_MT.bin` | **2000–2024** | 64.0 KB | `6afc200699f004339e2cb32c6e7bc74b` | Factory Binary Firmware Dump |
| `Y33_VQ30DET_4P202_MT.bin` | **2000–2024** | 64.0 KB | `3b35c446d25419e63d4892568bca1525` | Factory Binary Firmware Dump |
| `Y33_VQ30DET_4P203_MT.bin` | **2000–2024** | 64.0 KB | `8e08165f7f1a357d21b1bcd946656f83` | Factory Binary Firmware Dump |
| `Y33_VQ30DET_5P710_AT.bin` | **2000–2024** | 64.0 KB | `9c25b10ac01b13ee5a3cb2c374dc02d9` | Factory Binary Firmware Dump |
| `Y33_VQ30DET_5P711_AT.bin` | **2000–2024** | 64.0 KB | `7e1c22f67f00840ab9a0fd9d20597d2e` | Factory Binary Firmware Dump |
| `Y33_VQ30DET_6P500_MT.bin` | **2000–2024** | 64.0 KB | `592bdfb03b1b4b07aa196393d6ae27d2` | Factory Binary Firmware Dump |
| `Y33_VQ30DET_6P501_MT.bin` | **2000–2024** | 64.0 KB | `d987d2167a98e998705fc3b9c99c4fb1` | Factory Binary Firmware Dump |
| `Y60_TB42E_35J00_MT.bin` | **2000–2024** | 32.0 KB | `1771e948326a32f02c06c52ec33c2e14` | Factory Binary Firmware Dump |
| `Y60_TB42E_35J01_MT.bin` | **2000–2024** | 32.0 KB | `7d0717dbdbf0ae72e89e908b884a56e2` | Factory Binary Firmware Dump |
| `Y60_TB42E_35J10_AT.bin` | **2000–2024** | 32.0 KB | `66139f5301ffc3c195cda64670719c7a` | Factory Binary Firmware Dump |
| `Y62_TB45E_VB716.BIN` | **2000–2024** | 63.6 KB | `0bfaac53a806e8ed1e4d97b94afaaa1e` | Factory Binary Firmware Dump |
| `Z31_RB20DET_20P61_MEC_R62_MT.BIN` | **2000–2024** | 16.0 KB | `7cdd762711ab4a818c3038a0bbd0bdb9` | Factory Binary Firmware Dump |
| `Z31_RB20DET_20P70_MEC_R61_AT.bin` | **2000–2024** | 16.0 KB | `99238042870ad683c03059f9e82e8f9a` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1984_02P02_MT.BIN` | **1984** | 16.0 KB | `2cbac6dd21820be2aa55d4b1a16e09e5` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1984_02P03_MT.bin` | **1984** | 16.0 KB | `28728a3352e6a25bd1acf54507189007` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1984_02P07_MT.bin` | **1984** | 16.0 KB | `7c52f306ce28883c19cf05f953d07ef2` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1984_07P00_MT.BIN` | **1984** | 16.0 KB | `ee1cbd469989a725c070c63ce001cee9` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1984_10P00_MT.BIN` | **1984** | 16.0 KB | `1a9d312275e33d42ac5dcc3bb9b575c3` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1986_19P12_AT.bin` | **1986** | 16.0 KB | `db51811002f79a13c803c16ae7ec9975` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1987_21P01_MT.BIN` | **1987** | 16.0 KB | `5d5ded86c0f600aaad07fe9c77ede950` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1987_21P11_AT.bin` | **1987** | 16.0 KB | `002a28a25881d6b7e2858e36184c1895` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1988_26P00_MT_SS.bin` | **1988** | 16.0 KB | `07a443497578501746bf93b5881ef794` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1988_26P01_MT.bin` | **1988** | 16.0 KB | `ac449b4ab5212ff757564f246e298e32` | Factory Binary Firmware Dump |
| `Z31_VG30ET_1988_26P10.BIN` | **1988** | 16.0 KB | `e8e184ece6f365dd75538f5a0b36ad3c` | Factory Binary Firmware Dump |
| `Z31_VG30E_1984_01P00_MT.bin` | **1984** | 16.0 KB | `eb3caa9035a354ed0955eb93bc81827e` | Factory Binary Firmware Dump |
| `Z31_VG30E_1984_06P01_MT.BIN` | **1984** | 32.0 KB | `7b210dff307cc90251ccccf09efddeff` | Factory Binary Firmware Dump |
| `Z31_VG30E_1984_06P11_AT.BIN` | **1984** | 16.0 KB | `3919d26ecef7510581da9cac3d4a9690` | Factory Binary Firmware Dump |
| `Z31_VG30E_1984_06P15_AT.bin` | **1984** | 16.0 KB | `894159d219a452b1801ca4b428dec70c` | Factory Binary Firmware Dump |
| `Z31_VG30E_1984_10P00_MT.bin` | **1984** | 16.0 KB | `31ffc12c2c6421701b0b23574eab533b` | Factory Binary Firmware Dump |
| `Z31_VG30E_1986_18P03_MT.bin` | **1986** | 16.0 KB | `b6d0ade8d77b9ebcf7126cf732640593` | Factory Binary Firmware Dump |
| `Z31_VG30E_1986_18P07_MT.bin` | **1986** | 16.0 KB | `718fec8b361f8660f1b2e27bca1778dd` | Factory Binary Firmware Dump |
| `Z31_VG30E_1986_18P18_MT.bin` | **1986** | 16.0 KB | `c8d54983abd3cb262a6aa36ed0869a88` | Factory Binary Firmware Dump |
| `Z31_VG30E_1986_21P66_MT.bin` | **1986** | 16.0 KB | `ee11a981029306cadc86d4852e09f380` | Factory Binary Firmware Dump |
| `Z31_VG30E_1988_25P00_MT.bin` | **1988** | 16.0 KB | `50046ca7293227474da4434ac8ae6f14` | Factory Binary Firmware Dump |
| `Z31_VG30E_1988_25P10_AT.bin` | **1988** | 16.0 KB | `8eba4009dce8a0cb0e75eb5fde0d15d2` | Factory Binary Firmware Dump |
| `Z31_VG30E_1988_NA_CA.BIN` | **1988** | 16.0 KB | `b1f31b6d8722704fffa335f1cdbfaf0a` | Factory Binary Firmware Dump |
| `Z32_FOR_RB25DET_41P03_MT_v3.bin` | **2000–2024** | 32.0 KB | `609348c7da7c673223692a0f45b8a37c` | Factory Binary Firmware Dump |
| `Z32_FOR_RB25DE_41P03_MT_S2_v3.bin` | **2000–2024** | 32.0 KB | `5d3ff856415d0c01a8c076446483bcb5` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_1989_NA_AT_M257ACA8.bin` | **1989** | 32.0 KB | `634969617a539295be2a95bac8f13cf3` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_30P10.bin` | **2000–2024** | 32.0 KB | `c675735fade59ef7e66faeadd2e00e24` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P02_1990_MT_FED.BIN` | **1990** | 32.0 KB | `bc726e7565cd9ae3b6c7ba651364e784` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P03_1990_MT_FED.BIN` | **1990** | 32.0 KB | `97c50fa61263428c981e600dec6ce313` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P08_1990_MT_CALI.BIN` | **1990** | 32.0 KB | `bb9668c388d54882c605eddcd38d03fe` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P11.bin` | **2000–2024** | 32.0 KB | `6a4885cf061d8f7452ff441f5eea6acd` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P12.bin` | **2000–2024** | 32.0 KB | `c7e984bdc4864426799ec4e9695f09aa` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P01_1991_1993_MT_EDM.bin` | **1991–1993** | 32.0 KB | `7fca8db92cbbc9f811923a370def1d83` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P06_MT.bin` | **2000–2024** | 32.0 KB | `a6a655c1e5587c05d8b510a99831de58` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P11_AT_1992_EDM.bin` | **1992** | 32.0 KB | `9c8edf0efb04ddfa4645048e94d04526` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P01_AT_1990_JDM_M4.BIN` | **1990** | 32.0 KB | `123fd911b8e8d6d6308da239401a17a9` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P02_MT_JDM.bin` | **2000–2024** | 32.0 KB | `2917c557091a9df4d97428ffe38f5a09` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P03_MT_JDM.BIN` | **2000–2024** | 32.0 KB | `76f4afd37d040a861963b9db48425d35` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P04_MT_1991_JDM.BIN` | **1991** | 32.0 KB | `4fb4d51f776d68259de427305eca1a7a` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P11_AT_TXC_661.bin` | **2000–2024** | 32.0 KB | `bfee693253557eef52f53b33d6ff81ac` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P12_AT.bin` | **2000–2024** | 32.0 KB | `80b92e376e3da858b42b9288c8212599` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P13_AT.bin` | **2000–2024** | 32.0 KB | `8277b6aeb51ce560e4a949cace0979f7` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P14_JDM.bin` | **2000–2024** | 32.0 KB | `7d15b18850f72c9a3d401cad2ebcb0dd` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P60_MT_1992.BIN` | **1992** | 32.0 KB | `4409df9b429e02f268e7d654c4f15529` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P70_MT.BIN` | **2000–2024** | 32.0 KB | `a0d4f6a1884d5d0b465573e37b0fa905` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_47P10_MT.bin` | **2000–2024** | 32.0 KB | `d698dd4a383c96dc5cdcd890b53cfc08` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_48P01_MT_1991.BIN` | **1991** | 32.0 KB | `af4656fd08c4c8c9f0451d56c7ebb126` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_48P76.BIN` | **2000–2024** | 32.0 KB | `2de0ea0c9ce88fc649eb238df57d9c70` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_49P71.bin` | **2000–2024** | 64.0 KB | `cc3dec24bfc0ac77d2a227df915a4120` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_51P00_MT_1995.bin` | **1995** | 64.0 KB | `889bd9c30e24f0dd7c18c793367ca810` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_51P05_MT_1995.bin` | **1995** | 64.0 KB | `3f15582c9b01ad1943996814a62e4508` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_51P60_MT.bin` | **2000–2024** | 64.0 KB | `15a26f7adf7354b1abc3bfdcad110863` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_51P65_MT.bin` | **2000–2024** | 64.0 KB | `5c4a73de625b1021afcc6af32315a12a` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_51P70.bin` | **2000–2024** | 64.0 KB | `edbb9b467896f48db29f6c879ef3b176` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_54P00_1996_MT.bin` | **1996** | 64.0 KB | `57f3232366c077f98d3ee6978acbb173` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P00_1990_NA_MT_FED.BIN` | **1990** | 32.0 KB | `decdee3ae2db76af59e9f12576e774a8` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P60_1990_NA_MT_FED.BIN` | **1990** | 32.0 KB | `4edc4bbcf0bbcfe5f83842393a5ec6c3` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P75_1991_NA_AT.BIN` | **1991** | 32.0 KB | `b6e807523ca68acbaf215223e430b8ce` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P00_1990_NA_AT.bin` | **1990** | 32.0 KB | `3287d5ece0ee82c4626c91dcc74fc90c` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P12_1990_NA_AT.bin` | **1990** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P12_AT.bin` | **2000–2024** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `Z32_VG30DE_40P01_1991_NA_MT_JDM.bin` | **1991** | 32.0 KB | `9ccebd22f09f29afe03615984cbf2add` | Factory Binary Firmware Dump |
| `Z32_VG30DE_40P13_AT.bin` | **2000–2024** | 32.0 KB | `c8b592bf26ed5128eb8b8b8c19fc4fa6` | Factory Binary Firmware Dump |
| `Z32_VG30DE_45P05_1993_NA_MT.bin` | **1993** | 64.0 KB | `336081a37acb46044edca577f46173f3` | Factory Binary Firmware Dump |
| `Z32_VG30DE_45P15_1993_NA_AT.bin` | **1993** | 64.0 KB | `bfc61c3daa5c90f0137cd7a915dea5fc` | Factory Binary Firmware Dump |
| `Z32_VG30DE_46P10_1992_AT_ADM.bin` | **1992** | 32.0 KB | `83f20f9d6b2f4e827cf80a5bfdbbf644` | Factory Binary Firmware Dump |
| `Z32_VG30DE_46P80_1992_AT.bin` | **1992** | 32.0 KB | `c65c5518813167583ccf898840eab84e` | Factory Binary Firmware Dump |
| `Z32_VG30DE_50P06.bin` | **2000–2024** | 64.0 KB | `2ee468bc13fb2880545c9aa4a80b42c4` | Factory Binary Firmware Dump |
| `Z32_VG30DE_50P76_1994_NA_AT.bin` | **1994** | 64.0 KB | `3cd661cd1e09462f6f7f883171082722` | Factory Binary Firmware Dump |
| `Z32_VG30DE_52P05.bin` | **2000–2024** | 64.0 KB | `fa34981622d6af63407fd79efe21dd5b` | Factory Binary Firmware Dump |
| `Z32_VG30DE_53P00_NA_MT.bin` | **2000–2024** | 64.0 KB | `c4dc43612271209045cc018029e38621` | Factory Binary Firmware Dump |
| `Z32_VG30DE_53P05_NA_MT.bin` | **2000–2024** | 64.0 KB | `6217271bfc0ae65302bfe728564900a1` | Factory Binary Firmware Dump |
| `Z32_VG30DE_AT_49P66.bin` | **2000–2024** | 64.0 KB | `1aa07634df9c49f82f2c68b5e19e8c93` | Factory Binary Firmware Dump |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi yang tersedia, struktur kalibrasi mencakup parameter esensial:
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
