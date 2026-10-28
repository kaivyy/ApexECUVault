# VAG_TDI_EDC15_EDC16_ORIGINAL_BINS - ECU Calibration Suite

**Repository Path**: `02_CARS/VAG_AUDI_VOLKSWAGEN/VAG_TDI_EDC15_EDC16_ORIGINAL_BINS`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `879 files` (864 binary dumps, 15 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `VAG_TDI_EDC15_EDC16_ORIGINAL_BINS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1998–2009

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| ` VW Golf V 2.0 TFSI 1K0907115T 387445.ori` | **1998–2009** | 2.00 MB | `56b3535a308605b52eea2e0d99f235e8` | Factory Binary Firmware Dump |
| `0-281-011-666_all_BDM_EEprom.bin` | **1998–2009** | 4.0 KB | `86af2be99f512e5e7ea61f428aec7ac5` | Factory Binary Firmware Dump |
| `0-281-011-666_all_BDM_Flash.bin` | **1998–2009** | 1.00 MB | `973a51c687a6fdcb3953c7bb60c1ccf3` | Factory Binary Firmware Dump |
| `0-281-011-666_all_BDM_Mic.bin` | **1998–2009** | 448.2 KB | `01394300d53ef43224e95dc21871ae1a` | Factory Binary Firmware Dump |
| `001566h.ori` | **1998–2009** | 128.0 KB | `598b872a1fcf51c33490b2883c7802dd` | Factory Binary Firmware Dump |
| `001566l.ori` | **1998–2009** | 128.0 KB | `17b857dd4b7e0d282a19e9ff0747fd39` | Factory Binary Firmware Dump |
| `016FEorg.127.bin` | **1998–2009** | 256.0 KB | `668a663abd474deaf7066b79e768df4d` | Factory Binary Firmware Dump |
| `018AT_0003.ORI` | **1998–2009** | 512.0 KB | `252cf2f73ad8dfba8f09b07ff73df420` | Factory Binary Firmware Dump |
| `019CJ.ori` | **1998–2009** | 512.0 KB | `c696c81178172f0f21e047554bd9aafb` | Factory Binary Firmware Dump |
| `019EP.ori` | **1998–2009** | 512.0 KB | `d826f907a5962f84ed4ca50789c82708` | Factory Binary Firmware Dump |
| `021906258B.bin` | **1998–2009** | 64.0 KB | `b948278205ab5e8ae7b8573f26e0590c` | Factory Binary Firmware Dump |
| `021906258BK.ori` | **1998–2009** | 64.0 KB | `60542b159fae38a22d365e0d4360bc94` | Factory Binary Firmware Dump |
| `021906258BS_0261203215_v358227_OEM.bin` | **1998–2009** | 64.0 KB | `e4365f6f3668f6d8335925971054aacd` | Factory Binary Firmware Dump |
| `021906258CK.ori` | **1998–2009** | 64.0 KB | `1a5285580c1f86eedc1ab8cf7f163b4e` | Factory Binary Firmware Dump |
| `021906258CP.ori` | **1998–2009** | 64.0 KB | `9e9eca50c669766df240a50a0e58a62e` | Factory Binary Firmware Dump |
| `021906258DJ_0261203045_v358341_OEM.bin` | **1998–2009** | 64.0 KB | `c81a3b390e9d486dcbbc01d38d7d9625` | Factory Binary Firmware Dump |
| `021CG_high.ori` | **1998–2009** | 128.0 KB | `1eb90148fb5811c8f8a9076ee9b38060` | Factory Binary Firmware Dump |
| `021CG_low.ori` | **1998–2009** | 128.0 KB | `a56ce6b420eec652a34afb6d11083786` | Factory Binary Firmware Dump |
| `021DL_H.bin` | **1998–2009** | 128.0 KB | `2776a2d2e16723932320ca7ccea9c08c` | Factory Binary Firmware Dump |
| `021DL_L.bin` | **1998–2009** | 128.0 KB | `935fa9b3002ee7b2079ba4e5b94730a3` | Factory Binary Firmware Dump |
| `022906032CS_0261207881_v368604_ME_7.1.1_OEM.bin` | **1998–2009** | 1.00 MB | `15852becfbb0f46e0dc0bf4180ad685c` | Factory Binary Firmware Dump |
| `0261204022 355640.ori` | **1998–2009** | 8.0 KB | `6f63925a66c242443982bdb64d5b8e8a` | Factory Binary Firmware Dump |
| `0261208268 8N0906018CG 369579.ori` | **1998–2009** | 1.00 MB | `033d34d9dbeca9a3b88f8a961e829c90` | Factory Binary Firmware Dump |
| `0261S02291_386852.ori` | **1998–2009** | 2.00 MB | `842e578200330acb945944d0bea5a559` | Factory Binary Firmware Dump |
| `0281001242_698.ori` | **1998–2009** | 64.0 KB | `f4112fd9476a544db34d75060ae48917` | Factory Binary Firmware Dump |
| `0281001242_699.ori` | **1998–2009** | 64.0 KB | `a191def26eab79a81ed59a5d2e629f2d` | Factory Binary Firmware Dump |
| `0281001324_551.ori` | **1998–2009** | 64.0 KB | `fe1be5f6a1b4f075fa132e69bf86d0ac` | Factory Binary Firmware Dump |
| `0281001324_552.ori` | **1998–2009** | 64.0 KB | `b85eab07ca0ab9f22590165d8e972f99` | Factory Binary Firmware Dump |
| `0281001652-821.ori` | **1998–2009** | 128.0 KB | `5c976b3d4d19b9fe3f9025e9509e9db9` | Factory Binary Firmware Dump |
| `0281001652-822.ori` | **1998–2009** | 128.0 KB | `4b8096149a29b605c71a61838a53c031` | Factory Binary Firmware Dump |
| `0281010159_401Q_D66_351132_LL.ori` | **1998–2009** | 128.0 KB | `51920545baccb73ab695ced83409e7ed` | Factory Binary Firmware Dump |
| `0281010159_401Q_D66_351133_HH.ori` | **1998–2009** | 128.0 KB | `8e4a68032083a5637bdd57efa304dc73` | Factory Binary Firmware Dump |
| `0281011672 - 1037370516 - 03G906016AP - Meu Golf 2.0 TDI DSG 140hp.ori` | **1998–2009** | 1.00 MB | `470ceb1071aa49098146297e0cec4b0d` | Factory Binary Firmware Dump |
| `028906021AF 0281001309 867.ori` | **1998–2009** | 64.0 KB | `1da936d507404c749ba76eaf55638111` | Factory Binary Firmware Dump |
| `028906021AF 0281001309 868.ori` | **1998–2009** | 64.0 KB | `8e59d629244a2eb6516f3e5d572ae481` | Factory Binary Firmware Dump |
| `028906021CK-0281001423424-1037355221.ori` | **1998–2009** | 128.0 KB | `39b3a117c4a6876106662a0055d96e37` | Factory Binary Firmware Dump |
| `028906021CK-0281001423424-1037355222.ori` | **1998–2009** | 128.0 KB | `ad42cbd206e786097e59a153da16ba21` | Factory Binary Firmware Dump |
| `028906021CS_0281001664.bin` | **1998–2009** | 256.0 KB | `3682457f44fc5a10ccef464c91917f21` | Factory Binary Firmware Dump |
| `028906021GQ_0281001682_MSA15_OEM.bin` | **1998–2009** | 256.0 KB | `4f33dedb6cc4d220ef43d7f041326f9a` | Factory Binary Firmware Dump |
| `028906021GQ_0281001682_v357271_HHH683_MSA15_OEM.bin` | **1998–2009** | 128.0 KB | `73ad84f0784a24d3962edf8f996d2e82` | Factory Binary Firmware Dump |
| `034BH_M_4MV.ori` | **1998–2009** | 512.0 KB | `3259d212544afa1ac14c35def3c7a8e2` | Factory Binary Firmware Dump |
| `038906016H_0281011146_v371297_EDC16U31_OEM.bin` | **1998–2009** | 512.0 KB | `412fbf9e4b0c5621cc7d23200eeed50e` | Factory Binary Firmware Dump |
| `038906016L_0281011433_v370476_EDC16U31_2004AT_OEM.bin` | **2004** | 512.0 KB | `ab4250effbfd2c0092cac1efdc2f7b33` | Factory Binary Firmware Dump |
| `038906016Q_0281011812_v371296_EDC16U31_OEM.bin` | **1998–2009** | 512.0 KB | `85f727027fdc920751eada8b70e4c922` | Factory Binary Firmware Dump |
| `038906018EB_HHH_A_0.BIN` | **1998–2009** | 128.0 KB | `5a8b83343bf02489584abf997b22414c` | Factory Binary Firmware Dump |
| `038906018EB_LLL_A_0.BIN` | **1998–2009** | 128.0 KB | `00c7a4245fa22f8469199627f2a41a2d` | Factory Binary Firmware Dump |
| `038906019GC_0281010892_1037362795_A3_ATD.Bin` | **1998–2009** | 512.0 KB | `1bedc8069117029ec5c14472eaf5b47d` | Factory Binary Firmware Dump |
| `03G906016AB_0281012238_v376708_EDC16U34_MT_OEM.bin` | **1998–2009** | 512.0 KB | `7593baba1f938b5c2fad12567f05ea49` | Factory Binary Firmware Dump |
| `03G906016AC_0281012239_v376707_EDC16U34_DSG_OEM.bin` | **1998–2009** | 512.0 KB | `8390ffa698fe176ffe5d75e59b647e0b` | Factory Binary Firmware Dump |
| `03G906016GD 9577-orig.BIN` | **1998–2009** | 2.00 MB | `7e26b2022c867a0ea01de7de9e11ac10` | Factory Binary Firmware Dump |
| `03L906022NH-1037399332-Q5-2,0 edc17.bin` | **1998–2009** | 2.00 MB | `fe10f3475907b2fa6db578eda68c9223` | Factory Binary Firmware Dump |
| `057x.ori` | **1998–2009** | 256.0 KB | `80d070ea6b23fb72aa442d7bb86e6fc2` | Factory Binary Firmware Dump |
| `05Golf101_195_292.bin` | **2005** | 512.0 KB | `9d255a8888d0cc72aa3116c0be13f31d` | Factory Binary Firmware Dump |
| `06A90601AK.bin` | **1998–2009** | 256.0 KB | `0d18ec73a4e6f1f5fdf063012ac68eae` | Factory Binary Firmware Dump |
| `06A906032DS_0261207080_v360930_ME7.5_MT_OEM.bin` | **1998–2009** | 1.00 MB | `6143f1770874d5d372e73aa5e6d4a1de` | Factory Binary Firmware Dump |
| `06A906032LP_0261207955_v367518_ME7.5-1M_Jetta-1.8T-MT_OEM.bin` | **1998–2009** | 1.00 MB | `9b5c750a1edecd74b4449bfdf9470841` | Factory Binary Firmware Dump |
| `070906016AN_368585 ori.bin` | **1998–2009** | 1.00 MB | `670dbd551e2e219479a2b6d740513d5c` | Factory Binary Firmware Dump |
| `1.9TDI AVF 130HP 038906019GF 0281010812 362603.ori` | **1998–2009** | 512.0 KB | `875bdd42154e34452f74b7269d784d85` | Factory Binary Firmware Dump |
| `1037355659_orig.BIN` | **1998–2009** | 64.0 KB | `a5f64f26fc009bc91993167cd9534881` | Factory Binary Firmware Dump |
| `1037355660_orig.BIN` | **1998–2009** | 64.0 KB | `b3c5268bf328b4d77b3ac51b52307bcc` | Factory Binary Firmware Dump |
| `1037393968org.ori` | **1998–2009** | 643.9 KB | `46e134af684bcf1290d1a453a3990208` | Factory Binary Firmware Dump |
| `1K0907115A.ori` | **1998–2009** | 2.00 MB | `5f73e53acdd73ce55a33a443edf52e97` | Factory Binary Firmware Dump |
| `206580.ORG.bin` | **1998–2009** | 512.0 KB | `17c7a648c41155bff09d20a34453cc18` | Factory Binary Firmware Dump |
| `206619.ori` | **1998–2009** | 1.00 MB | `a734acbdd2c39f114c71ba04dd2cf980` | Factory Binary Firmware Dump |
| `2706.ori` | **1998–2009** | 512.0 KB | `41fd7559d1cde485bb9413471628a74f` | Factory Binary Firmware Dump |
| `27c010.bin` | **1998–2009** | 128.0 KB | `58c2dc2e54ea398159853b9f3cda1958` | Factory Binary Firmware Dump |
| `27æ010.bin` | **1998–2009** | 128.0 KB | `f336c2c16e99148a31a51166b98ae8aa` | Factory Binary Firmware Dump |
| `29BL1MB.bin` | **1998–2009** | 1.00 MB | `585abd0b1934a4c92f05a79706929447` | Factory Binary Firmware Dump |
| `29BL802.ori` | **1998–2009** | 1.00 MB | `5cf88ec92234156a528ac7339cd06e8f` | Factory Binary Firmware Dump |
| `29bl802.bin` | **1998–2009** | 1.00 MB | `019030a832c31f142a89e4255a9932e4` | Factory Binary Firmware Dump |
| `350751.ori` | **1998–2009** | 512.0 KB | `75db018112fc83ebf302f63bc932a3ac` | Factory Binary Firmware Dump |
| `352633.ori` | **1998–2009** | 128.0 KB | `2e3daba21b18c270f154f5369115a7a2` | Factory Binary Firmware Dump |
| `352634.ori` | **1998–2009** | 128.0 KB | `4754194c3ab36cba55cc320420bde442` | Factory Binary Firmware Dump |
| `354008.ori` | **1998–2009** | 1.00 MB | `3dc3c20da3be6458cd72ea99299f1bef` | Factory Binary Firmware Dump |
| `355.827.ori` | **1998–2009** | 128.0 KB | `b601ae8daafbf529fe70ab54d84023b4` | Factory Binary Firmware Dump |
| `355.828.ori` | **1998–2009** | 128.0 KB | `5cb0aba8846194ed245118cc3ecf616e` | Factory Binary Firmware Dump |
| `355054.ori` | **1998–2009** | 64.0 KB | `a9a2c26d3199cf38e8e403f67415fe2a` | Factory Binary Firmware Dump |
| `355055.ori` | **1998–2009** | 64.0 KB | `d92db562bc69d7fc85563f52b0468701` | Factory Binary Firmware Dump |
| `356791.ori` | **1998–2009** | 128.0 KB | `7c0681fa1d93e4c0ed71061f8582d7a7` | Factory Binary Firmware Dump |
| `356792.ori` | **1998–2009** | 128.0 KB | `0a35259c5047480edd0739f45b8effdb` | Factory Binary Firmware Dump |
| `357791.ori.BIN` | **1998–2009** | 128.0 KB | `35d403c08df77e2c113da8ef11e3ece0` | Factory Binary Firmware Dump |
| `357792.ori.BIN` | **1998–2009** | 128.0 KB | `29c6f8ad0046e6514ba3bcaa923cfb1d` | Factory Binary Firmware Dump |
| `357_871.ori` | **1998–2009** | 64.0 KB | `b06c19bc99500cff789755ee253928f2` | Factory Binary Firmware Dump |
| `357_872.ori` | **1998–2009** | 64.0 KB | `e021064f5144324d97763b2eb8e34106` | Factory Binary Firmware Dump |
| `358022.ori` | **1998–2009** | 64.0 KB | `434fe8247601597e92178ac5f2bf12f2` | Factory Binary Firmware Dump |
| `358389.ori` | **1998–2009** | 256.0 KB | `b53800d4db7d168a06d860fe4d4f59ac` | Factory Binary Firmware Dump |
| `358390.ori` | **1998–2009** | 256.0 KB | `f4d721534847c8d0a0bda4fc62fed506` | Factory Binary Firmware Dump |
| `359_834.ori` | **1998–2009** | 128.0 KB | `d8fe1021dba2aee96d08eb4ed7aa4b1e` | Factory Binary Firmware Dump |
| `359_835.ori` | **1998–2009** | 128.0 KB | `e96e12c3d069a99e5d17aaa16c744108` | Factory Binary Firmware Dump |
| `360647.ori` | **1998–2009** | 1.00 MB | `38462ff188118bfb184ab4240b9d1346` | Factory Binary Firmware Dump |
| `371-ECU1.ori` | **1998–2009** | 2.00 MB | `12cfbcce2be6d1371a416c886c34695e` | Factory Binary Firmware Dump |
| `386826.ori` | **1998–2009** | 2.00 MB | `6b933bca2ed78daf78b97f71e0835d61` | Factory Binary Firmware Dump |
| `3C0907115S_0261S02510_v391093_MED9.1_2007AT_OEM.bin` | **2007** | 2.00 MB | `c700e3f5dc8f5764dd53d36119cf2c36` | Factory Binary Firmware Dump |
| `496_hhh.bin` | **1998–2009** | 128.0 KB | `8bb07a67a4e110803decf2d907b385c4` | Factory Binary Firmware Dump |
| `496_lll.bin` | **1998–2009** | 128.0 KB | `f6f98688a3ab37d2e52946dd59978bd8` | Factory Binary Firmware Dump |
| `4B0906018CH_0261207216_v360101_ME7.5_1M_Audi_A4_MT_OEM.bin` | **1998–2009** | 1.00 MB | `85412cd972e93d4c44b4d02383150a3c` | Factory Binary Firmware Dump |
| `4B0907401T-0281010153-1037352631.ori` | **1998–2009** | 128.0 KB | `1a8fec09d1de772aac4efc531b8bb28c` | Factory Binary Firmware Dump |
| `4B0907401T-0281010153-1037352632.ori` | **1998–2009** | 128.0 KB | `58fea107f32bfdde63a4c1c79d21d00f` | Factory Binary Firmware Dump |
| `4F9910401B.ori` | **1998–2009** | 2.00 MB | `423ef92d3d7eb05151a61458d8577795` | Factory Binary Firmware Dump |
| `4L0907401 379749.ori` | **1998–2009** | 2.00 MB | `31a1fc5181ebfa836a7e41d728dbd841` | Factory Binary Firmware Dump |
| `887.BIN` | **1998–2009** | 64.0 KB | `b507819094d5012744f89af599910b18` | Factory Binary Firmware Dump |
| `888.BIN` | **1998–2009** | 64.0 KB | `ce01dab2855cef6dd789d55a5a569984` | Factory Binary Firmware Dump |
| `8E0909518AF_0261207939_7366883_0003_1_8L_R4_5VT__audi_170_5s.std` | **1998–2009** | 1.00 MB | `77a429d6fad8f0865ec26b3f4a16e655` | Factory Binary Firmware Dump |
| `8E0910115M_0261S02223_v387401_MED9.1_2006MT_OEM.bin` | **2006** | 2.00 MB | `b680d1b44d96fa2bbe508d099e5a26cb` | Factory Binary Firmware Dump |
| `8E0910115N_0261S02211_1037376490_0020.bin` | **1998–2009** | 2.00 MB | `6923befb9937b489eacf355e3f34807a` | Factory Binary Firmware Dump |
| `93C56.BIN` | **1998–2009** | 256 B | `b7cb62e55e8621524963711aa76fe70c` | Factory Binary Firmware Dump |
| `A4_2.0tdi_170ps_03G906018AQ_ppd1.3_orig.bin` | **1998–2009** | 2.00 MB | `1c36d7e4aaa6306055a29c012a1a1811` | Factory Binary Firmware Dump |
| `A6 EEPROM.ori` | **1998–2009** | 4.0 KB | `90cd51668a36d167db40aae43bb6bf4f` | Factory Binary Firmware Dump |
| `A6 flash.ori` | **1998–2009** | 2.00 MB | `04b5511d64b61874ddb5fa40c8fac9e5` | Factory Binary Firmware Dump |
| `A6 mcu.ori` | **1998–2009** | 253.5 KB | `6b0405a9fcbcbf7b2d11d1a639506dad` | Factory Binary Firmware Dump |
| `A6TD7549.ORI` | **1998–2009** | 128.0 KB | `638fd7a7451a5eee43576e6303b4e8c9` | Factory Binary Firmware Dump |
| `A6TD7550.ORI` | **1998–2009** | 128.0 KB | `808de13beba30b8cd7237d0011a6e52d` | Factory Binary Firmware Dump |
| `A6_2.0L_98y_024D.bin` | **1998–2009** | 32.0 KB | `4853c212a09588311733937bfb954797` | Factory Binary Firmware Dump |
| `A8 4_0 V8 275Ks org.binS.bin` | **1998–2009** | 1.00 MB | `8f042a81055c3b0ee5cc0979237a1cad` | Factory Binary Firmware Dump |
| `AM29F800B_1c.BIN` | **1998–2009** | 1.00 MB | `8f575fda9e64a924d23bacad55e02d6d` | Factory Binary Firmware Dump |
| `AM29F800B_2.BIN` | **1998–2009** | 1.00 MB | `e100243c1b6cef0f6ede4b10134e9ddc` | Factory Binary Firmware Dump |
| `AT156ES.ori` | **1998–2009** | 512.0 KB | `73039bbabc34a86c06abf8f5c6ede8ea` | Factory Binary Firmware Dump |
| `AUDI A4 2.5TDI 150HP 0281001945 8D0907401F 766-767.ori` | **1998–2009** | 256.0 KB | `263fa09d0882ab575d5e17b4bb4c5b0a` | Factory Binary Firmware Dump |
| `AUDI S4 2.7 V6  0261206376  8D0907551E 350221.ori` | **1998–2009** | 512.0 KB | `534588a2f5ad0b4b876212f477b15b98` | Factory Binary Firmware Dump |
| `AUDI TT RS 340 CV 0261S02601_1037503608.ORI` | **1998–2009** | 2.00 MB | `f83af942039ed2efc38af832c9266a1a` | Factory Binary Firmware Dump |
| `AUDI_A2_D1200_R3V2T_44kw_0281011239_045906019BL_1037366716_crcC0956A22.ori` | **1998–2009** | 512.0 KB | `7b5215e4a81eba2a4d497fbb03b315a9` | Factory Binary Firmware Dump |
| `AVPD6AF.ori` | **1998–2009** | 128.0 KB | `088fb878a6570c0205209277e35b9cc4` | Factory Binary Firmware Dump |
| `Audi  A3 1.8T 180PS 0261206269  06A906032AF 350034.ori` | **1998–2009** | 512.0 KB | `39610a14c4726e02477edb9021eef090` | Factory Binary Firmware Dump |
| `Audi  A6 3.0TDI 225HP 0281012269  4f0907401b_375256.ori` | **1998–2009** | 2.00 MB | `37f5969e2233f636828f316ed2584859` | Factory Binary Firmware Dump |
| `Audi 100 4.2 V8 280HP 4A0907557A 0261203143 357764.ori` | **1998–2009** | 64.0 KB | `2a29babddf70b072367a1d7e8d524caf` | Factory Binary Firmware Dump |
| `Audi 80 1.9TDI 0281001317_875.ori` | **1998–2009** | 64.0 KB | `c74639e7b887a2c0c37f71cafdfd859c` | Factory Binary Firmware Dump |
| `Audi 80 1.9TDI 0281001317_876.ori` | **1998–2009** | 64.0 KB | `4e190762e51f0c86cb6af1abd5c15860` | Factory Binary Firmware Dump |
| `Audi 80 1.9TDI 1Z 90HP 028906021GC 0281001668 357787.ori` | **1998–2009** | 256.0 KB | `4ccdaee08f7ad564ae70783423bc3b93` | Factory Binary Firmware Dump |
| `Audi 80 1.9TDI 90HP 028906021D 0281001198.ori` | **1998–2009** | 64.0 KB | `2822fb3a1b20a9be905e4ec7d2ab7493` | Factory Binary Firmware Dump |
| `Audi 80 TDI 1.9L 0281001133-2287357911-4A0907401A(Diesel).std` | **1998–2009** | 32.0 KB | `066626344d9188c0149bc103dd0a0c98` | Factory Binary Firmware Dump |
| `Audi 80 TDI 1.9L 0281001133-2287357912-4A907401A(Turbo).std` | **1998–2009** | 32.0 KB | `b1964dd2d89e7fc22924f945c0b289e0` | Factory Binary Firmware Dump |
| `Audi 80 TDI 1.9L 0281001317-2537355581-021906028AP(Diesel).std` | **1998–2009** | 64.0 KB | `c7060a9d6dd3670b193db5bc656be501` | Factory Binary Firmware Dump |
| `Audi 80 TDI 1.9L 0281001317-2537355582-021906028AP(Turbo).std` | **1998–2009** | 64.0 KB | `f0552785ae9f1ec6daa3827dba696d53` | Factory Binary Firmware Dump |
| `Audi 80 TDI 1.9L 0281001319-2287357877-021906028AQ(Diesel).std` | **1998–2009** | 64.0 KB | `693be9c23683881352613745fbdd4ac7` | Factory Binary Firmware Dump |
| `Audi 80 TDI 1.9L 0281001319-2287357878-021906028AQ(Turbo).std` | **1998–2009** | 64.0 KB | `0d816c7ed1a487ab04c24e9c81998d28` | Factory Binary Firmware Dump |
| `Audi 80 TDI 1.9L 0281001441-2537355890-028906021DQ(Diesel).std` | **1998–2009** | 64.0 KB | `2a1c5bfb3716da77a9a5c5561877cd21` | Factory Binary Firmware Dump |
| `Audi 80 TDI 1.9L 0281001441-2537355891-028906021DQ(Turbo).std` | **1998–2009** | 64.0 KB | `4270c7d64ac93b84a069ef2f25d8ff11` | Factory Binary Firmware Dump |
| `Audi A2 1.4TDI 75HP 045906019BP 0281012194 376317.ori` | **1998–2009** | 512.0 KB | `beb66aa9e82b9fb0a57081a9dda0e519` | Factory Binary Firmware Dump |
| `Audi A2 1.4TDI 75HP 045906019G 0281010220 360497.ori` | **1998–2009** | 512.0 KB | `2492338ea8db907f29054a8911d74c4c` | Factory Binary Firmware Dump |
| `Audi A2 1.4TDI AMF 75HP 045906019AT 0281011100 366249.ori` | **1998–2009** | 512.0 KB | `4318c496040400c61179d5d37dfb03e6` | Factory Binary Firmware Dump |
| `Audi A2 1.4TDI AMF 75HP 045906019BA 0281011404 367361.ori` | **1998–2009** | 512.0 KB | `69e38fabf6944316d231203fc69ca5ba` | Factory Binary Firmware Dump |
| `Audi A2 1.4TDI AMF 75HP 045906019F 0281011607 368969.ori` | **1998–2009** | 512.0 KB | `8f528ea776c1df1af684bbee3149e316` | Factory Binary Firmware Dump |
| `Audi A2 1.4TDI AMF 75HP 045906019G 0281010220 363201.ori` | **1998–2009** | 512.0 KB | `0523a5443ff15e8f3721d585afa03cfb` | Factory Binary Firmware Dump |
| `Audi A3 1.6FSI 115HP 03C906056CP 0261S02187 381976.ori` | **1998–2009** | 2.00 MB | `29c12f10abbc91cffbc41e23e7fe9d02` | Factory Binary Firmware Dump |
| `Audi A3 1.8T 06A906032BB 0261206268 350033.ori` | **1998–2009** | 512.0 KB | `1c618a872096186ec51cc0ad6cbf2d2a` | Factory Binary Firmware Dump |
| `Audi A3 1.8T 06A906032HN 0261207440 363908.ori` | **1998–2009** | 1.00 MB | `0f041121f2f68c74be6ec6acc9ab0053` | Factory Binary Firmware Dump |
| `Audi A3 1.8T 150HP 06A906018AQ 0261204678 358108.ori` | **1998–2009** | 256.0 KB | `378bfe2bce9bf2fbcc3918809b74fa85` | Factory Binary Firmware Dump |
| `Audi A3 1.8T 150HP 06A906032AS 0261206435 352354.ori` | **1998–2009** | 512.0 KB | `c76752a786988e5f6bb1ca15dd7471e1` | Factory Binary Firmware Dump |
| `Audi A3 1.8T 150HP 06A906032CL 0261206552 1037354003.ori` | **1998–2009** | 512.0 KB | `4fce90e13ef25360043c87f76574bdc9` | Factory Binary Firmware Dump |
| `Audi A3 1.8T 150HP 06A906032S 0261206197 359598.ori` | **1998–2009** | 512.0 KB | `916266153346ce36d32d15f1a61dbd94` | Factory Binary Firmware Dump |
| `Audi A3 1.8T AGN 125HP 06A906018C 0261204127 355961.ori` | **1998–2009** | 128.0 KB | `50f202d27ee11845d15bbfe41ff069f3` | Factory Binary Firmware Dump |
| `Audi A3 1.8T AGU 150HP 06A906018AQ 0261204678 350010.ori` | **1998–2009** | 256.0 KB | `c88c89b349ad014687499f1db4c266af` | Factory Binary Firmware Dump |
| `Audi A3 1.8T AGU 150HP 06A906018AQ 0261204678 359525.ori` | **1998–2009** | 256.0 KB | `2e871d2a304d1fb3546de1e8305ee7da` | Factory Binary Firmware Dump |
| `Audi A3 1.8T AGU 150HP 06A906018AR 0261204679 359522.ori` | **1998–2009** | 256.0 KB | `079d605392652947effd8b50773891b7` | Factory Binary Firmware Dump |
| `Audi A3 1.8T AGU 150HP 06A906018CG 0261206518 352127.ori` | **1998–2009** | 256.0 KB | `aabef5afb1e93f854afffc0b56c09eb0` | Factory Binary Firmware Dump |
| `Audi A3 1.8T AGU 150HP 06A906018D 0261204254 357459.ori` | **1998–2009** | 128.0 KB | `a9a901e6c68f9bbed5cb1983909e5e20` | Factory Binary Firmware Dump |
| `Audi A3 1.8T ARZ 150HP 0261206435 352757.ori` | **1998–2009** | 512.0 KB | `d449f8efbaeea23a60a01b9620f34825` | Factory Binary Firmware Dump |
| `Audi A3 1.8T AUQ 180HP 06A906032BJ 0261206892 360288.ori` | **1998–2009** | 1.00 MB | `fcb781c79e78eea16a3a619a969ef991` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI 038906016H.ori` | **1998–2009** | 1.00 MB | `2e396827fe7fa10e18a8bbeb51b1048d` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI 105HP 03G906016J 0281011383 368596.ori` | **1998–2009** | 1.00 MB | `a2f5955cbfc0629a626bd2492b45fbae` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI 105HP 03G906021AB 389826.ori` | **1998–2009** | 2.00 MB | `eb2b51b237b1761e63036b50c6eb55f8` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI 110HP 038906012BB 0281010123 350851.ori` | **1998–2009** | 512.0 KB | `e487b4ee414459aaa4fc3a56621696fd` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI 90HP 038906012B 0281010121 350849 2802.ori` | **1998–2009** | 512.0 KB | `0d0eef07056d6b5f1c3c0d3b7f7c834e` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI 90HP 038906012C 0281010122 1037350850.ori` | **1998–2009** | 512.0 KB | `eafc3f4565ba6eea7d663c48566a2cac` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI 90HP 038906018AK 0281001728 357704.ori` | **1998–2009** | 256.0 KB | `415baa29f88d616bd022627cf425e2ae` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI AGR 90HP 038906018BB 0281001757 358253.ori` | **1998–2009** | 256.0 KB | `18b893f37bf2bf793958182752ff0b7d` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI AHF 110HP 038906012A 0281010120 1037350848.ori` | **1998–2009** | 512.0 KB | `a754573701f1df6cdbaa6da44d0d1410` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI AHF 110HP 038906018BP 0281001848.ori` | **1998–2009** | 256.0 KB | `7b29d265d023c8d7c01dfc76113382b6` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI AHU 90HP 038906018A 0281001410 355828.ori` | **1998–2009** | 256.0 KB | `db7444d1d50618ea9cc1ddda84c02a0d` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI ASZ 130HP 038906019CK 0281010308 360763.ori` | **1998–2009** | 512.0 KB | `e00dce348ae48e5ed2d60b62a0b76e99` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI ASZ 130HP 038906019CK 0281010308 362845.ori` | **1998–2009** | 512.0 KB | `d5f42b54d3624a768dfcf51d91e5296f` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI ASZ 130HP 038906019FT 0281010981 363228.ori` | **1998–2009** | 512.0 KB | `e7647ec359bdbc61c022f803bd844b08` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI ASZ 130HP 038906019FT 0281010981 366273.ori` | **1998–2009** | 512.0 KB | `889e5effb6d6c3786f97672052924b2d` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI BKC 105HP 03G906016CC 0281011832 371093.ori` | **1998–2009** | 1.00 MB | `a981da25e8da6de2391bd25bb4281579` | Factory Binary Firmware Dump |
| `Audi A3 1.9TDI BKD 105HP 03G906016J 0281011383 369261.ori` | **1998–2009** | 1.00 MB | `bd5525be47bc659130d7679590dfdc30` | Factory Binary Firmware Dump |
| `Audi A3 2.0T 8P0907115K 0261S02220 386817.ori` | **1998–2009** | 2.00 MB | `8936c29200e2aed44c1cf93c8b4356ba` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI 140HP 03G906016G 0281011364 367950.ori` | **1998–2009** | 1.00 MB | `e1142feaf6b728d70e66aefda8edb67a` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI 140HP 03G906016G 0281011364 368156.ori` | **1998–2009** | 1.00 MB | `152acf6f10bf28d429188934c11ae911` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI 140HP 03G906016G 0281011364 368508.ori` | **1998–2009** | 1.00 MB | `578485fa86456628a62b861bb1e1079c` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI 140HP 03G906021AN.ori` | **1998–2009** | 2.00 MB | `c1464d84bfd87557cb503ee1b6221429` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI BKD 03G906016FF 0281011905 371366.ori` | **1998–2009** | 1.00 MB | `2ba9f5ece94525bddde89a71366db5fb` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI BKD 140HP 0281011905 371366.ori` | **1998–2009** | 1.00 MB | `b36f5bd15d1c8f3006e0bb0a6f07b83f` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI BKD 140HP 03G906016AT 0281011453 369901.ori` | **1998–2009** | 1.00 MB | `0f41bdb85677ee0dec884bef5ff0d558` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI BKD 140HP 03G906016FF 0281011905 370634.ori` | **1998–2009** | 1.00 MB | `fc9107271577fc41ab383e407ded3ee0` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI BKD 140HP 03G906016FF 0281011905 375970.ori` | **1998–2009** | 1.00 MB | `0223d5d75f5546c1eac4cc83ee3483d2` | Factory Binary Firmware Dump |
| `Audi A3 2.0TDI BKD 140HP 03G906016G 0281011364 369819.ori` | **1998–2009** | 1.00 MB | `c07bf6e4d0a81b66ec1e85928df0a3db` | Factory Binary Firmware Dump |
| `Audi A3 BLS 03G906021HP 382669.ori` | **1998–2009** | 2.00 MB | `38e4063d4eeaa12c9d773d0415222ffa` | Factory Binary Firmware Dump |
| `Audi A3_1.8TQ_206434_0261206434.ori` | **1998–2009** | 194.4 KB | `2cb0cb9f021fd354159be3ca631aa261` | Factory Binary Firmware Dump |
| `Audi A4 1.8 0261204774 8D0907558B 357973.ori` | **1998–2009** | 128.0 KB | `d12577ff1b097b5e126e1cd9b2ec0a44` | Factory Binary Firmware Dump |
| `Audi A4 1.8 0261204957 8D0907558T 356670.ori` | **1998–2009** | 128.0 KB | `701f2d6767a3e8b4137377fed6e9bf0b` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 150HP 4B0906018P 0261206537 352750.ori` | **1998–2009** | 512.0 KB | `260af00583c9f63da5cf7f55f439aa58` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 150HP 8D0907557 0261203550 355966.ori` | **1998–2009** | 128.0 KB | `ddaecfc3a60d36fe117f83252ffe2434` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 150HP 8D0907557P 0261204258 350269.ori` | **1998–2009** | 256.0 KB | `0b5ddb6527cdf3156221a73196f10ff2` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 150HP 8D0907557T 0261204185 1037358703.ori` | **1998–2009** | 128.0 KB | `639eed0af98d58bc5e7366d5de41e6da` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 150HP 8D0907557T 0261204185 358761.ori` | **1998–2009** | 128.0 KB | `3af631af88d89f61a052ce94cad9afa4` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 150HP 8D0907559 0261204963 359127.ori` | **1998–2009** | 256.0 KB | `1737179052f6bb5d24f310633caa8fed` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 150HP 8D0907559C 0261206315 350004.ori` | **1998–2009** | 256.0 KB | `8501cef30bfab0093bbc49d4df268c67` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 150HP 8E0909518M 0261207778 363466.ori` | **1998–2009** | 1.00 MB | `5834c031d73e69dee325e8f324d15dfa` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 163HP 8E0909518AA 0261207934 366381.ori` | **1998–2009** | 1.00 MB | `f07899dba003dcdecd5f0e7cb13240de` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 180HP 8E0906018B 0261206868 360990.ori` | **1998–2009** | 1.00 MB | `f62ffe49ad2c6fc714610c04ddc770a8` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 190HP 8E0909518AN 0261208285 368075.ori` | **1998–2009** | 1.00 MB | `3885748589223a3765a9e7974114dbc4` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 4B0906018R 0261206539 354735.ori` | **1998–2009** | 1.00 MB | `82fd47beb9ebf2e117e96d8711acd0d6` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 4B0906018R 0261206539 354801.ori` | **1998–2009** | 1.00 MB | `6703115fae3e1591f8bed3b6557cff19` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 8D0907558DA 0261206429 350714.ori` | **1998–2009** | 128.0 KB | `f6fdafb9fb72db1e26f588c9c82869b0` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 8E0909018 0261207435 362521.ori` | **1998–2009** | 1.00 MB | `c4f07aab7ec8a26310f1214f04af7c2c` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 8E0909518AK 0261208230 368072.ori` | **1998–2009** | 1.00 MB | `de0521f258855661f27284d17dbc8907` | Factory Binary Firmware Dump |
| `Audi A4 1.8T 8E0909518AS 0261208500 369011.ori` | **1998–2009** | 1.00 MB | `5c4fe991098d6258ef2b2fb293f4b53f` | Factory Binary Firmware Dump |
| `Audi A4 1.8T AEB 150HP 8D0907557 0261203551 355800.ori` | **1998–2009** | 128.0 KB | `f76da67f6c29f25141bfeaea0848ab3d` | Factory Binary Firmware Dump |
| `Audi A4 1.8T AJL 8D0907558D 0261204778 358150.ori` | **1998–2009** | 128.0 KB | `86a3976e5115c74b4c0be3613a7ed2b5` | Factory Binary Firmware Dump |
| `Audi A4 1.8T APU 150HP 4B0906018AR 0261206524 352053.ori` | **1998–2009** | 512.0 KB | `6e1b504b5c2bd8e86539719597c17ce1` | Factory Binary Firmware Dump |
| `Audi A4 1.8T AWT 4B0906018CG 0261207215 360306.ori` | **1998–2009** | 1.00 MB | `6346428aded07e53dca869ecddb27a20` | Factory Binary Firmware Dump |
| `Audi A4 1.8T BEX 192HP 8E0909518AH 0261207941 366871.ori` | **1998–2009** | 1.00 MB | `59c64e69946defe36b975f6497352583` | Factory Binary Firmware Dump |
| `Audi A4 1.8T BFB 163HP 8E0909518AA 0261207934 366494.ori` | **1998–2009** | 1.00 MB | `24d3e2cc0c637531820692532fd94e53` | Factory Binary Firmware Dump |
| `Audi A4 1.8T BFB 163HP 8E0909518AL 0281208228 369311.ori` | **1998–2009** | 1.00 MB | `a4e56774f72e82142e87eb95d1d325ac` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 100HP 038906019LF 0281011210 366506.ori` | **1998–2009** | 512.0 KB | `96aa082d5af0a2dd0cbf1b2293c8eb07` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 105HP 03G906016HA 390133.ori` | **1998–2009** | 2.00 MB | `e02b9ccb0e22fa8529ef7249d0ab9b11` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 110HP 038906012AH 0281010200 1037352636.ori` | **1998–2009** | 512.0 KB | `797747d519d1e1d77e14980b3a06122e` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 110HP 038906012AH 0281010200 352255.ori` | **1998–2009** | 512.0 KB | `9fd5429e0651da39456991353ad4d849` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 110HP 038906012BL 0281010199 352254.ori` | **1998–2009** | 512.0 KB | `a4823cde808a2aeb5b267e2550f9110c` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 115HP 0281011887 03G906016CJ 1037371805.ori` | **1998–2009** | 2.00 MB | `92aa50818cba94ffccc7fbde2ca7be9c` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 115HP 03G906016FE 0281012127 390131.ori` | **1998–2009** | 2.00 MB | `da283c8b3b84eaf117943c65cd716947` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 130HP 038906019F 0281012187 372301.ori` | **1998–2009** | 512.0 KB | `5d06c012297e9a4f97b03d8ef18bba61` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 130HP 038906019FP 0281010729 362614.ori` | **1998–2009** | 512.0 KB | `1892fd3cb9f5200c975532f21462df9b` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 130HP 038906019FP 0281010729 363740.ori` | **1998–2009** | 512.0 KB | `bfd300431e6eed944cd87d64b3b414f5` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 1Z 90HP 028906021F 0281001367 355586.ori` | **1998–2009** | 128.0 KB | `ac1d475cbad57986755f0dd1b9d3cf20` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI 90HP 0281010197 038906012AF 352621.ori` | **1998–2009** | 512.0 KB | `5bbe71d28bede643f88dcab6d60d865d` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AFN 110HP 028906021CE 0281001426 355217.ori` | **1998–2009** | 256.0 KB | `88024153b22cdae16f197844c5b72140` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AFN 110HP 028906021CE 0281001426 355304.ori` | **1998–2009** | 256.0 KB | `d8e7ddba5c1bc4705ec6f41b00b81608` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AFN 110HP 028906021GN 0281001660 357272.ori` | **1998–2009** | 256.0 KB | `15a3044f245630e525f68bc9d663f90e` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AFN 110HP 028906021GN 0281001660 357833.ori` | **1998–2009** | 256.0 KB | `e0d6234322adf3ef3b364ef55deea554` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AFN 110HP 038906018S 0281001721 356817.ori` | **1998–2009** | 256.0 KB | `480dd6f5819631793f521bd094ab1322` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AFN 110HP 038906018S 0281001721 358381.ori` | **1998–2009** | 256.0 KB | `d8dbaafa738c79edcc1329f4b83141d2` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AHH 90HP 038906012AJ 0281010202 352257.ori` | **1998–2009** | 512.0 KB | `6a30923235fe02477a28cbb0bffe6438` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AHH 90HP 038906012AJ 0281010202 352625.ori` | **1998–2009** | 512.0 KB | `85c4f96235603c6cdf7aa7a11d722156` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AHU 90HP 028906021BD 0281001439 438-439.ori` | **1998–2009** | 256.0 KB | `67ed1383484747e6e1419d23480cf107` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AHU 90HP 028906021GM 0281001658 355274.ori` | **1998–2009** | 256.0 KB | `4256e195c5a6df510bb5807170afc437` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AHU 90HP 028906021GM 0281001658 357835.ori` | **1998–2009** | 256.0 KB | `ecc37997447366f018b85d0019a3718a` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AHU 90HP 038906018R 0281001726 727820.ori` | **1998–2009** | 256.0 KB | `0108c7c7cc4ce57323762bc375f12eda` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AJM 115HP 038906019AN 0281010094 354607.ori` | **1998–2009** | 512.0 KB | `5394b06445f45b1c7fdeee7f89c25910` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AJM 115HP 038906019BR 0281010226 354265.ori` | **1998–2009** | 512.0 KB | `f8388f53609e9ee0af01321c7cd69d49` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AVB 100HP 038906019JP 0281011141 366049 1569.ori` | **1998–2009** | 512.0 KB | `b3c124de074908a77b5ebef1e134920d` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AVF 130HP 038906019JL 0281011036 363230.ori` | **1998–2009** | 512.0 KB | `41520bd83a73618930cf70bc54bbfe89` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AVF 130HP 038906019JT 0281011138 366048.ori` | **1998–2009** | 512.0 KB | `ae1fde9413f03d4b7d4e17d19ce331f6` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AVF 130HP 038906019KA 0281011140 367021.ori` | **1998–2009** | 512.0 KB | `e41dd9587af4a73e6a8d64e473e29bc2` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AVF 130HP 038906019LJ 0281011222 366508.ori` | **1998–2009** | 512.0 KB | `c6a345fe753e0c200af57d3f6512eb7f` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AVF 130HP 038906019LJ 0281011222 370445.ori` | **1998–2009** | 512.0 KB | `50bfca7e4f8410968164758b9c18e2dc` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AWX 130HP 038906019CG 0281010406 362036.ori` | **1998–2009** | 512.0 KB | `fe0eec31b3a9a4046d1f516c25a1a244` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AWX 130HP 038906019FP 0281010729 362705.ori` | **1998–2009** | 512.0 KB | `4cae32ec897e1b03cd7a7a5abe3b3414` | Factory Binary Firmware Dump |
| `Audi A4 1.9TDI AWX 130HP 038906019GD 0281010844 362628.ori` | **1998–2009** | 512.0 KB | `55c39c7a996a0e4c65b7b08d7a007b6e` | Factory Binary Firmware Dump |
| `Audi A4 19TDI AFN 110 038906018S 0281001721 357593.ori` | **1998–2009** | 256.0 KB | `c6c2fb949e7b6872f5fa1f18f554ab8a` | Factory Binary Firmware Dump |
| `Audi A4 2.0TDI 140HP 03G906016JD 0281012654 378340.ori` | **1998–2009** | 2.00 MB | `8c958cff847c07bf8829e588943f2739` | Factory Binary Firmware Dump |
| `Audi A4 2.0TDI 140HP 03G906016LR 0281012726 386343.ori` | **1998–2009** | 2.00 MB | `6e8eecaaf664c9497740e308659f073a` | Factory Binary Firmware Dump |
| `Audi A4 2.0TDI BPW 140 03G906016KN 391503.ori` | **1998–2009** | 2.00 MB | `349adaa287817d2e02528f42387e3c3e` | Factory Binary Firmware Dump |
| `Audi A4 2.0TDI BPW 140HP 03G906016KN 382430.ori` | **1998–2009** | 2.00 MB | `b8f80b64ceaceec7946e96353390e746` | Factory Binary Firmware Dump |
| `Audi A4 2.0TDI BRD 170HP 03G906018AQ 5WP4554.ori` | **1998–2009** | 2.00 MB | `3040e5aceba2fc55bdaeb10f61a5d1bb` | Factory Binary Firmware Dump |
| `Audi A4 2.0TFSI 8E0907115D 0261S02211 386863.ori` | **1998–2009** | 2.00 MB | `d8634039264b1f85081ddb603d422e08` | Factory Binary Firmware Dump |
| `Audi A4 2.5 TDI 180HP O8E0907401 0281011386 1037367176.ori` | **1998–2009** | 1.00 MB | `36a89e4ba1e2c21c100285ec820c3f06` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 150HP 0281010152 4B0907401R 1037351651.ori` | **1998–2009** | 256.0 KB | `1d46d9ab3fba253797fcb1a60145a731` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 150HP 8D0907401H 0281001834 356764.ori` | **1998–2009** | 256.0 KB | `b5639a6e20b754631e30ffa0bcb1eff7` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 150HP 8D0907401P 0281010158.ori` | **1998–2009** | 256.0 KB | `57aa1343fc9e220552d301aa950d2744` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 150HP 8D0907401Q 0281010159 351133.ori` | **1998–2009** | 256.0 KB | `adaaf16d034108b123911b86f0bdc50f` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 155HP 4B1907401D 0281010494 351926.ori` | **1998–2009** | 512.0 KB | `8a67e1148763f1a7221608ef2f690c84` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 155HP 8D1907401A 0281010100 352924.ori` | **1998–2009** | 512.0 KB | `cacb9b62919701511988dff7285970cb` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 163HP 8E0907401AF 0281012142 375555.ori` | **1998–2009** | 1.00 MB | `7bdea853e29ed0ea13b473aac832d970` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 163HP 8E0907401S 0281011435 369443.ori` | **1998–2009** | 1.00 MB | `54c5fbe4de065cacce52047b1c533592` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 163HP E0907401M 0281011255 368106.ori` | **1998–2009** | 1.00 MB | `8ff27c2084fc84f24cb3822bc89bfa3d` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 180HP 8E0907401C 0281010493 362493.ori` | **1998–2009** | 512.0 KB | `6eb6d053db256a7cbe376ffc5d14e7bf` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 180HP 8E0907401D 0281010823 366614.ori` | **1998–2009** | 512.0 KB | `d43c86d448e2f696a796a9ceb2675e3a` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 180HP 8E0907401D 0281010823 367154.ori` | **1998–2009** | 512.0 KB | `ab69530586dec9877cb576f636863645` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI 8E0907401T 0281011444 367801.ori` | **1998–2009** | 1.00 MB | `0f18b43cfbd14ff0539141ec5387f2b6` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI AFB 150HP 8D0907401L 0281010155 145-146.ori` | **1998–2009** | 256.0 KB | `c5235ffcc86f4fb7068fc21bba26f0ac` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI AKE 180HP 8E0907401B 0281010446 360545.ori` | **1998–2009** | 512.0 KB | `ca242420780cc1cbb4b9082fe5d50ab8` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI BDG 163HP 8E0907401M 0281011255 369444.ori` | **1998–2009** | 1.00 MB | `5a98f014b78dfbfb08215e9f4a79411d` | Factory Binary Firmware Dump |
| `Audi A4 2.5TDI V6 150HP 8D0907401D 0281001812 359339.ori` | **1998–2009** | 256.0 KB | `4850a99b14fc047623b383cb2c3f4089` | Factory Binary Firmware Dump |
| `Audi A4 2.8 V6 4D0907551F 0261204687 357491.ori` | **1998–2009** | 128.0 KB | `ff5f0f72495f35bde55f0fdec5464154` | Factory Binary Firmware Dump |
| `Audi A4 3.0TDI 204HP 8E0907401AJ 377113.ori` | **1998–2009** | 512.0 KB | `f751b670a3c5f291669faba91d4e860e` | Factory Binary Firmware Dump |
| `Audi A4 3.0TDI 233HP 8K0907401 0281014014 392914.ori` | **1998–2009** | 2.00 MB | `2b115a9e58bb560545808536934562d2` | Factory Binary Firmware Dump |
| `Audi A4 quattro 2.5TDI 180HP 8E0907401C 0281010493 362493.ori` | **1998–2009** | 512.0 KB | `0ee09b8dba160a8cb3e5e1c9c6c4adc4` | Factory Binary Firmware Dump |
| `Audi A4 tdi 155ps orig.dat.bin` | **1998–2009** | 512.0 KB | `35699404f06ac3f295834c9d2642ae7d` | Factory Binary Firmware Dump |
| `Audi A4_D1900_R4V2T_66kW_0281010065_038906018FF_2150_xx167_168_crc9DA33691.ori` | **1998–2009** | 256.0 KB | `7e3442506713fe34211f75c223bf25b8` | Factory Binary Firmware Dump |
| `Audi A6 1.8T 150HP 4B0906018DC 0261207636 362358.ori` | **1998–2009** | 1.00 MB | `0718c63378abd8cfcbfcb3e0dad705f5` | Factory Binary Firmware Dump |
| `Audi A6 1.8T AEB 150HP 4B0907557A 0261204256 357473.ori` | **1998–2009** | 128.0 KB | `bea4579f3bbae91cf9e500f23c375769` | Factory Binary Firmware Dump |
| `Audi A6 1.8T AND 150HP 4B0906018L 0261206320 350703.ori` | **1998–2009** | 512.0 KB | `bf126f2366001c44c7bca5e28a68d6e6` | Factory Binary Firmware Dump |
| `Audi A6 1.9 TDI 038906018DG 0281001808 356001.ori` | **1998–2009** | 256.0 KB | `dfdc39abf65137a9aaba8573740fca1e` | Factory Binary Firmware Dump |
| `Audi A6 1.9TDI 115HP 03G906016JA 0281012723 1037377587.ori` | **1998–2009** | 2.00 MB | `91b547be8a35210e31e7c51439f9e728` | Factory Binary Firmware Dump |
| `Audi A6 1.9TDI 130HP 038906019CF 0281010405 362175.ori` | **1998–2009** | 512.0 KB | `ef36e7d1450aabbfc602de29f70f99ed` | Factory Binary Firmware Dump |
| `Audi A6 1.9TDI AFN 110HP 038906012AB 281010203 352258.ori` | **1998–2009** | 512.0 KB | `7939d5232d0ef88ffdc3449c27133548` | Factory Binary Firmware Dump |
| `Audi A6 1.9TDI AJM 115HP 038906019BS 0281010224 360072.ori` | **1998–2009** | 512.0 KB | `e15bab5c57623ff5fa77a56ebfae581a` | Factory Binary Firmware Dump |
| `Audi A6 1.9TDI AVF 130HP 038906019HM 0281011046 367002.ori` | **1998–2009** | 512.0 KB | `4e7afceebfe34310ceb9462fd7fb0976` | Factory Binary Firmware Dump |
| `Audi A6 1.9TDI AVF 130HP 038906019LM 0281011213 367408.ori` | **1998–2009** | 512.0 KB | `3b8841ac52197fa81c81b47e287ab552` | Factory Binary Firmware Dump |
| `Audi A6 2.0TDI 136HP 03G906016HQ 0281012555 383820.ori` | **1998–2009** | 2.00 MB | `d1f63e796e06b485208867f4ee85ab86` | Factory Binary Firmware Dump |
| `Audi A6 2.0TDI 140HP 03G906016BF_382716.BIN` | **1998–2009** | 2.00 MB | `00d9b3a5cb9b110b4a69e8c3eb7a3f4e` | Factory Binary Firmware Dump |
| `Audi A6 2.0TDI 140HP 03G906016GB 0281012112 383724.ori` | **1998–2009** | 2.00 MB | `805fcf171f25050c12aa992e5e62ec2b` | Factory Binary Firmware Dump |
| `Audi A6 2.0TDI 140HP 03G906016MG 393553.ori` | **1998–2009** | 512.0 KB | `6f501355178043ef1c753f94b33e69d0` | Factory Binary Firmware Dump |
| `Audi A6 2.2T AAN 230HP 4A0907551D 0261203603 358374.ori` | **1998–2009** | 64.0 KB | `fe78118e2647c341121bbb66ec596094` | Factory Binary Firmware Dump |
| `Audi A6 2.4 V6 177HP 3B0907552J 0261206122 350079.ori` | **1998–2009** | 512.0 KB | `2ebb7b9136dc54d0534b90d7506db0ed` | Factory Binary Firmware Dump |
| `Audi A6 2.5L 103kw 0281001478-2537355737.std` | **1998–2009** | 64.0 KB | `17bd2acca38a51813d2e8213d290cd13` | Factory Binary Firmware Dump |
| `Audi A6 2.5L 103kw 0281001478-2537355738.std` | **1998–2009** | 64.0 KB | `3e323daeb1d545c6edb438f9b3cefc0f` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 140HP 0281001321 355498.ori` | **1998–2009** | 128.0 KB | `d244c57dfe2c323a316377040842f4bc` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 140HP 4A0907401F 0281001255 358724.ori` | **1998–2009** | 128.0 KB | `8f7df9ed4bcdc0f402c7bd954065d4a4` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 150HP 0281010156 8D0907401M.ori` | **1998–2009** | 256.0 KB | `e01df5a76a2e4fa6e2dea87dd8f8a2d1` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 150HP 4B0907401C 0281001836 359393.ori` | **1998–2009** | 256.0 KB | `faf9c9eebba93f1fa889dd6baded5c4a` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 150HP 4B0907401H 0281001781 357690.ori` | **1998–2009** | 256.0 KB | `5811631112eafbd2b0ea16b1170a5359` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 150HP 4B0907401J 0281001772 357667.ori` | **1998–2009** | 256.0 KB | `c5fc0ee71939ab9ec4e5ffbb06d25097` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 150HP 4B0907401Q 0281010151 1037352649.ori` | **1998–2009** | 256.0 KB | `e35dd7456721db1d272e6bf40936bd88` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 150HP 4B0907401R 0281010152 1037351323.ori` | **1998–2009** | 256.0 KB | `10fd00e3ecfd98293b8c8f24f54b8eff` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 150HP 4B1907401A 0281010095 354255.ori` | **1998–2009** | 512.0 KB | `e9a07ae04a758bc72746bc78b7315b21` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 150HP 8D0907401N 0281010157 351050.ori` | **1998–2009** | 256.0 KB | `77542a87410658b767576200972a12f6` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 163HP  0281011255 8E0907401M 370841.ori` | **1998–2009** | 1.00 MB | `9ffd9b1fe470d8b964a7cde7bcc4d65c` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 163HP 8E0907401M 0281011255 367774.ori` | **1998–2009** | 1.00 MB | `b5bb44bd4102ce2f3080119d22ce263f` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 163HP 8E0907401P 0281011136 366619.ori` | **1998–2009** | 1.00 MB | `2f2963f90bd26c74ad8fb765daf059f9` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 163HP 8E0907401Q 0281011135 366644.ori` | **1998–2009** | 1.00 MB | `8fb2f4c96d2c2a4c4a1ea578cffe1733` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 4B2907401 0281010096 037354665.ori` | **1998–2009** | 512.0 KB | `7fba22c120094e91f391c4fef938b6bd` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 4B2907401 0281010096 350319.ori` | **1998–2009** | 512.0 KB | `1c63fec11118504f89fcf414938cb002` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 4B2907401 0281010096 354337.ori` | **1998–2009** | 512.0 KB | `36d33cbc7333315e04d96e19ad1904be` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 4B2907401B 0281010098 354335.ori` | **1998–2009** | 512.0 KB | `dded1427bbc88eed889e36125ff49509` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 4B2907401F 0281010443 362485.ori` | **1998–2009** | 512.0 KB | `44bc6d386d7f035f69449c85b8da9e6f` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 4B2907401J 0281010822 362761.ori` | **1998–2009** | 512.0 KB | `e2150ea9dce0bd78f6492eb623ae06d6` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 4B2907401J 0281010822 367153.ori` | **1998–2009** | 512.0 KB | `0cdd1071041aa6bc558a0c0f946ab466` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 4Z7907401A 0281010445 362124.ori` | **1998–2009** | 1.00 MB | `18d39a6dc52d272359fe252a3aa81282` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 8E0907401J 0281011387 367568.ori` | **1998–2009** | 1.00 MB | `a8852d53244525523aa24b2522cc1b53` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 8E0907401J 0281011387 367927.ori` | **1998–2009** | 1.00 MB | `bda7499b96241c33497dbc749b6a5a3e` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP 8E0907401N 0281011386 369512.ori` | **1998–2009** | 1.00 MB | `92d666a0d19c62613c4b19cfbca3c39b` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 180HP allroad 4Z7907401A 0281010445 354376.ori` | **1998–2009** | 512.0 KB | `4fffbcf8f0bb22ae75193d6bf7d77267` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI 4B0907401K 0281001931 350601.ori` | **1998–2009** | 256.0 KB | `847d2bd970ce1925b4bc24039190c2b8` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI AEL 140HP 4A0907401P 0281001321 355245.ori` | **1998–2009** | 64.0 KB | `b1fab4be8e59e78d5c7b29f0301c1eca` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI AEL 140HP 4A0907401P 0281001321 355246.ori` | **1998–2009** | 64.0 KB | `5267d0148b39aac9cba33fdfdf991b88` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI AFB 150HP 4B0907401AC 0281010399 351313.ori` | **1998–2009** | 512.0 KB | `64aa60af98699e08ce4205cca91dc541` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI AFB 150HP 4B0907401S 0281010148 351032.ori` | **1998–2009** | 256.0 KB | `c989b4771cc7d5fe6ab1ae7aca5c5e82` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI AKE 180HP 4B2907401D 0281010395 354333.ori` | **1998–2009** | 512.0 KB | `234dc91423e9cd98a5561a7cde6633fa` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI AKE 4B2907401J 0281010822 366611.ori` | **1998–2009** | 512.0 KB | `d12cdc90908c227243e6b58e20c9b4e1` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI AYM 155HP 4B1907401D 0281010494 363776.ori` | **1998–2009** | 512.0 KB | `1f5af0ac846b283cbb2e324b46b8df07` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI-180HP-AKE-0281010822-4B2907401J-1037363777.ori` | **1998–2009** | 512.0 KB | `39dc900cc9d47f9cb1adfc358d2c517b` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI-4B2907401E-0281010394-1037354332.ori` | **1998–2009** | 512.0 KB | `fe566b021befe57278f30f93d34c301b` | Factory Binary Firmware Dump |
| `Audi A6 2.5TDI-4B2907401E-0281010394-1037360719 .ori` | **1998–2009** | 512.0 KB | `d4ae4627ff1e595d4628efc471c29453` | Factory Binary Firmware Dump |
| `Audi A6 2.6 ABC 150HP4 A0907473D.ori` | **1998–2009** | 32.0 KB | `d1486d1ddc2cab23abac108416bbe6d3` | Factory Binary Firmware Dump |
| `Audi A6 2.7 TDI  180hp 0281012560 4F0907401B 7377319.orig.ori` | **1998–2009** | 2.00 MB | `910d5719eb3a70534f47517d4a377356` | Factory Binary Firmware Dump |
| `Audi A6 2.7T 265HP 4B0907551F 0261206378 350239.ori` | **1998–2009** | 1.00 MB | `d879360cb78911c4e408a03036a882fa` | Factory Binary Firmware Dump |
| `Audi A6 2.7T AJK 230HP 4B0907551G 0261206380 354065.ori` | **1998–2009** | 1.00 MB | `309f388866649043b48dc2774ef80a42` | Factory Binary Firmware Dump |
| `Audi A6 2.7TDI 163HP 4F0907401B 4F2910401S 377107.ori` | **1998–2009** | 2.00 MB | `806d361cfd59791e9fb23734d4711790` | Factory Binary Firmware Dump |
| `Audi A6 2.7TDI 180HP 4F2910401R 377106.ori` | **1998–2009** | 2.00 MB | `df054dfaca18338abbe2c48bf6a7b0b4` | Factory Binary Firmware Dump |
| `Audi A6 233HP 4F0910402E 381388.ori` | **1998–2009** | 2.00 MB | `60c2dc8dfdddda2b676b640e36c02246` | Factory Binary Firmware Dump |
| `Audi A6 233HP 4F9910401L 389130.ori` | **1998–2009** | 2.00 MB | `71fd93a050d10ddb601dc0a62dabcba7` | Factory Binary Firmware Dump |
| `Audi A6 3.0TDI 224HP 4F0907401B 1037374416.ori` | **1998–2009** | 2.00 MB | `37ba5d8d102c057698244284707d2c88` | Factory Binary Firmware Dump |
| `Audi A6 3.0TDI 4F0907401A 0281011569 371077.ori` | **1998–2009** | 2.00 MB | `7ea0413d07332336cb915b72fac2d4d6` | Factory Binary Firmware Dump |
| `Audi A6 3.0TDI 4F0907401A 372123.ori` | **1998–2009** | 2.00 MB | `8ef8c021cbefe448ef4789ec31463034` | Factory Binary Firmware Dump |
| `Audi A6 3.0TDI 4F0910401F 371077.ori` | **1998–2009** | 2.00 MB | `80d66ad45e49ca7d5a24b6a5b402c8f8` | Factory Binary Firmware Dump |
| `Audi A6 4.2 V8 4D0907558S 0261206204 352486.ori` | **1998–2009** | 1.00 MB | `e43cf6b511ab2cbba81ca1558a38f148` | Factory Binary Firmware Dump |
| `Audi A6 4.2i 4D0907560AE 0261206843 354728.ori` | **1998–2009** | 1.00 MB | `65a1b4c379d0cd37ee766c4338e74913` | Factory Binary Firmware Dump |
| `Audi A6 C4 2.5TDI 140HP 0281001321 355329.ori` | **1998–2009** | 128.0 KB | `f3d0589706cb015066a516fa13a0c947` | Factory Binary Firmware Dump |
| `Audi A6 allroad 2.5TDI 180HP 4Z7907401B 0281010897 366613.ori` | **1998–2009** | 512.0 KB | `20cfa1788de8b00f38904987825405aa` | Factory Binary Firmware Dump |
| `Audi A6 allroad 2.5TDI AKE 180HP 4Z7907401A 0281010445 362124.ori` | **1998–2009** | 512.0 KB | `38b3f645afad05aa9e57e5fd8e1b63b6` | Factory Binary Firmware Dump |
| `Audi A6 allroad 2.7T 263HP 4Z7907551N 0261207766 366367.ori` | **1998–2009** | 1.00 MB | `33cded4b9316d85f65d0f3a36b8e80db` | Factory Binary Firmware Dump |
| `Audi A6 allroad 2.7T 265HP 4Z7907551D 0261207137 354846.ori` | **1998–2009** | 1.00 MB | `cc2d944769c3df7ddb3ed5f2bd675992` | Factory Binary Firmware Dump |
| `Audi A6 allroad 2.7T BEL 250HP 4Z7907551R.ori` | **1998–2009** | 1.00 MB | `599e6d63aaa8999b3daa87e8b10c3b28` | Factory Binary Firmware Dump |
| `Audi A6-TDI 2,0 BLB-03G906016GN-0281012113-376101.ori` | **1998–2009** | 512.0 KB | `15ba4ec353625629bcc76ba706e720ed` | Factory Binary Firmware Dump |
| `Audi A8 2.5TDI 150HP 4D0907401G 0281001773 093.ori` | **1998–2009** | 256.0 KB | `6567b0c3582e4742e7abb56849301d15` | Factory Binary Firmware Dump |
| `Audi A8 2.5TDI 180HP 4D2907401 0281010160 354334.ori` | **1998–2009** | 512.0 KB | `d210c7ecec8790b671b8a5430d630b32` | Factory Binary Firmware Dump |
| `Audi A8 2.5TDI 180HP 4D2907401 0281010160 354666.ori` | **1998–2009** | 512.0 KB | `eb10c4f683703dd5d159d9c03a478c07` | Factory Binary Firmware Dump |
| `Audi A8 2.5TDI AFB 150HP 4D0907401N 0281010397 351308.ori` | **1998–2009** | 512.0 KB | `282771f00aef5d7b304889eed3ab23ea` | Factory Binary Firmware Dump |
| `Audi A8 3.3TDI 225HP 4D0907409C 0281010900 1037351707.ori` | **1998–2009** | 512.0 KB | `d884c8e20bb50ed090220d650cb123fc` | Factory Binary Firmware Dump |
| `Audi A8 3.3TDI AKF 224HP 4D0907409A 0281001867 351497.ori` | **1998–2009** | 512.0 KB | `ace859f28c4f4d00ec8938a7d6815b4b` | Factory Binary Firmware Dump |
| `Audi A8 4.2 V8 380HP 4D0907557G 0261204205 355159.ori` | **1998–2009** | 128.0 KB | `c6ad1dd3946048467517a65e62914bcf` | Factory Binary Firmware Dump |
| `Audi A8 4.2 V8 4D0907557B 0261203300 358194.ori` | **1998–2009** | 128.0 KB | `0ec808a96cc0e29cf3325a6a18904efd` | Factory Binary Firmware Dump |
| `Audi A8 6.0-450HP-4E0906018-0261208203-370953.ori` | **1998–2009** | 1.00 MB | `4063e60f5ed0a8afc760736e6db55b87` | Factory Binary Firmware Dump |
| `Audi A8_4.2_368674_208493_4E0910560K.ori` | **1998–2009** | 367.8 KB | `17ed8e12fc0bef2fc5ade8f7a62cb869` | Factory Binary Firmware Dump |
| `Audi Q5 2.0TDI 170HP 03L906022B 03L906022Q 500144.ori` | **1998–2009** | 2.00 MB | `3c590c86471993d44e1a5995f77274f6` | Factory Binary Firmware Dump |
| `Audi Q7 3.0TDI 4L0907401 390614.ori` | **1998–2009** | 2.00 MB | `fd4c154dc6461df1aa46c7f5587a2e23` | Factory Binary Firmware Dump |
| `Audi Q7 4.2TDI 326HP 4E1907409B 0281013013.ori` | **1998–2009** | 2.00 MB | `3eac1ec5502d8507f98fcea00d098872` | Factory Binary Firmware Dump |
| `Audi R8_0 261 S02 234_1037390288_MED91_4.2L V8 ori.bin` | **1998–2009** | 2.00 MB | `bf7cec9fa82a3a94382bcfa49fbf08f7` | Factory Binary Firmware Dump |
| `Audi RS4 2.7T 380HP 8D0907551Q 0261207141 360388.ori` | **1998–2009** | 1.00 MB | `a4b7cd6bdc0d86c4d211c098e9a1013a` | Factory Binary Firmware Dump |
| `Audi RS4 2.7T 8D0907551F 0261206635 354531.ori` | **1998–2009** | 1.00 MB | `fc837de318606923e877b6b4ef066dd0` | Factory Binary Firmware Dump |
| `Audi RS4 4.2FSI 8E1907560 0261S02165 379578.ori` | **1998–2009** | 2.00 MB | `2badc4fa79920d53ba69bbd5f6f92c1c` | Factory Binary Firmware Dump |
| `Audi RS6+ 4D1907558F 0261208728 373709.ori` | **1998–2009** | 1.00 MB | `4cec79534f249e29d682bda25fe2876d` | Factory Binary Firmware Dump |
| `Audi S2 2.2 ABH 220HP 0261203143 357360.ori` | **1998–2009** | 64.0 KB | `06bb3fb93947696eb86b050013ebeedd` | Factory Binary Firmware Dump |
| `Audi S3 (8L) 1.8 BAM-8N0906018BH-0261207751-1037362999.ori` | **1998–2009** | 1.00 MB | `af1cb4359fc1b304905144969b62c112` | Factory Binary Firmware Dump |
| `Audi S3 (8L) 1.8-AMK-8N0906018CH-0261208269-367511.ori` | **1998–2009** | 1.00 MB | `ff63a6efc3fef25445d03a29ea542cc2` | Factory Binary Firmware Dump |
| `Audi S3 1.8T 210HP 8L0906018K 0261206442 352377.ori` | **1998–2009** | 512.0 KB | `c882185bedce93bc223599298ae31f53` | Factory Binary Firmware Dump |
| `Audi S3 1.8T 210HP 8L0906018K 0261206442 352465.ori` | **1998–2009** | 512.0 KB | `a88cb89853a81145ca8def276594573c` | Factory Binary Firmware Dump |
| `Audi S3 1.8T 210HP 8N0906018J 0261206794 360284.ori` | **1998–2009** | 1.00 MB | `3ca85244bfe837ea895daa7c8abab3c4` | Factory Binary Firmware Dump |
| `Audi S3 1.8T 210HP 8N0906018J 0261206794 360314.ori` | **1998–2009** | 1.00 MB | `0dde632ffd4162be919d30034f439fd2` | Factory Binary Firmware Dump |
| `Audi S3 1.8T 210HP AMK 8N0906018AG 0261207213 360320.ori` | **1998–2009** | 1.00 MB | `d961a77feadf1ae667bb951fab875424` | Factory Binary Firmware Dump |
| `Audi S3 1.8T APY 210HP 8L0906018N 0261206796 352820.ori` | **1998–2009** | 512.0 KB | `ccb746ed44bbf6ebc924505ce49c82b0` | Factory Binary Firmware Dump |
| `Audi S3 2.0TFSI 265HP 8P0907115H 0261S02342 384214.ori` | **1998–2009** | 2.00 MB | `2eb53fc143fa679d8f290f0fc80a24f8` | Factory Binary Firmware Dump |
| `Audi S3 210HP 8L0906018N 0261206796 354092.ori` | **1998–2009** | 512.0 KB | `952751eb1c331957a18a7e726a614ae6` | Factory Binary Firmware Dump |
| `Audi S3 225HP 8N0906018BP 0261208054 366474.ori` | **1998–2009** | 1.00 MB | `8ea04671cfabf6cf749b8fd2b8d20e15` | Factory Binary Firmware Dump |
| `Audi S4 2.2T 260HP 4A0907551A 0261200465 356703.ori` | **1998–2009** | 64.0 KB | `4fcb9dbff678e3c1d0be14cb3e8695cb` | Factory Binary Firmware Dump |
| `Audi S4 2.2T 260HP 4A0907551AA 0261200465 356711.ori` | **1998–2009** | 64.0 KB | `e239472a8690fe7d44828afb8e2e5d42` | Factory Binary Firmware Dump |
| `Audi S4 2.2T 260HP 4A0907551AA 0261200465 357248.ori` | **1998–2009** | 64.0 KB | `d988862c04a00ee864558f33c06d23a7` | Factory Binary Firmware Dump |
| `Audi S4 2.2T 260HP 4A0907551AA 0261200465 357391.ori` | **1998–2009** | 64.0 KB | `8bcbbd3ff7345beba8702824dd0b4073` | Factory Binary Firmware Dump |
| `Audi S4 2.2T AAN 230HP 4A0907551B 0261203005 357249.ori` | **1998–2009** | 64.0 KB | `c90d08973dcaecd9708415da79dd8354` | Factory Binary Firmware Dump |
| `Audi S4 2.7 8D0907551G 0261206776 360855.ori` | **1998–2009** | 1.00 MB | `63273a1a83f2de867d34513d6b8731d3` | Factory Binary Firmware Dump |
| `Audi S4 2.7T 250HP 8D0907551D 0261206382 350243.ori` | **1998–2009** | 1.00 MB | `d8bbd2c5bcfe77d02b917c0c4a8b9850` | Factory Binary Firmware Dump |
| `Audi S4 2.7T 265HP 8D0907551A 0261206110 352345.ori` | **1998–2009** | 1.00 MB | `ae58bd292038cdb00cbe9a88527d5e4f` | Factory Binary Firmware Dump |
| `Audi S4 2.7T 265HP 8D0907551A 0261206110 352741.ori` | **1998–2009** | 1.00 MB | `e8b6f03d363eb0b6c21ac5156654f0f4` | Factory Binary Firmware Dump |
| `Audi S4 2.7T 265HP 8D0907551L 0261207004 354145.ori` | **1998–2009** | 1.00 MB | `146d346e4ed8bdcc7245ec2332f775a9` | Factory Binary Firmware Dump |
| `Audi S4 2.7T 265HP 8DO907551C 0261206108 350093.ori` | **1998–2009** | 512.0 KB | `63276e4d13f115a146c9ae90cd568f8e` | Factory Binary Firmware Dump |
| `Audi S4 4.2i 8E0907560H 0261208776 1037374035.ori` | **1998–2009** | 1.00 MB | `17602dc0c9559a98b855a74a904784e9` | Factory Binary Firmware Dump |
| `Audi S5 4.2 V8 8T0907560 0261S02329 390268.ori` | **1998–2009** | 2.00 MB | `ef2f2c2ad7c5ecdfbe3be98ac753afd7` | Factory Binary Firmware Dump |
| `Audi S6 4.2 V8 290HP 4A0907557B 0261203645 358378.ori` | **1998–2009** | 64.0 KB | `72462f45cc97fa341040d8f9d41002d3` | Factory Binary Firmware Dump |
| `Audi S6 4.2 V8 290HP 4A0907557C 0261203599 355858.ori` | **1998–2009** | 64.0 KB | `ad5441b1c451a99073327ec5e4d85190` | Factory Binary Firmware Dump |
| `Audi S8 4.2 V8 4D0907557N 0261204563 358953.ori` | **1998–2009** | 128.0 KB | `6288f95fb5752e720267e888fccba1a8` | Factory Binary Firmware Dump |
| `Audi S8 4.2i 360HP 4D0907559G  0261206096 352379.ori` | **1998–2009** | 1.00 MB | `b8cf0eef4541ab0c8a7f468e99e77936` | Factory Binary Firmware Dump |
| `Audi TT  1.8TFSI 160PS 0261201948 1037398687 ORI.bin` | **1998–2009** | 2.00 MB | `8beea1359b823ef73b2f6c0f6b6f9427` | Factory Binary Firmware Dump |
| `Audi TT 1.8 225HP 8N0906018F 0261206105 356615.ori` | **1998–2009** | 512.0 KB | `fc03faf1f7aeaf914ad57cc4b456b247` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 150HP 8D0907557T 0261204185 357482.ori` | **1998–2009** | 128.0 KB | `0bcc0b5a02eca0fbf0581e3ce3b984fa` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 180HP 8N0906018AB 0261207027 354503.ori` | **1998–2009** | 512.0 KB | `70612df7e6f3b224cb503806f9c9ec21` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 180HP 8N0906018AQ 0261207416 363478.ori` | **1998–2009** | 1.00 MB | `1692118aa4b78e27c3ee7386601b302f` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 180HP 8N0906018BR 0261208005 363675.ori` | **1998–2009** | 1.00 MB | `d99ed8d297a8720ac7230a18ad5410a5` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 180HP 8N0906018Q 0261206439 354510.ori` | **1998–2009** | 512.0 KB | `3de85a5327cfeca59284fbd092432afa` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 225HP 8L0906018M 0261206797 352821.ori` | **1998–2009** | 512.0 KB | `d7186cf639a7c62f7127ad4db93ab4b4` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 225HP 8L0906018M 0261206797 354094.ori` | **1998–2009** | 512.0 KB | `75ab0340010fa6730f2260ced4254694` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 225HP 8N0906018AN 0261207418 362588.ori` | **1998–2009** | 512.0 KB | `6f6abf8f11a9a91b81b9d8bc0a958391` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 225HP 8N0906018T 0261206228 354508.ori` | **1998–2009** | 512.0 KB | `859775ea2c2daf3379d52aa646d03819` | Factory Binary Firmware Dump |
| `Audi TT 1.8T 8N0906018BR 0261208005 369398.ori` | **1998–2009** | 1.00 MB | `7f6784476fb18c03bc16d268c37bcb6a` | Factory Binary Firmware Dump |
| `Audi TT 1.8T AJQ 180HP 8N0906018A 0261204898 359559.ori` | **1998–2009** | 512.0 KB | `9c67adfb4b86291a987db2ec29d0389a` | Factory Binary Firmware Dump |
| `Audi TT 1.8T AJQ 180HP 8N0906018B 0261204962 350294.ori` | **1998–2009** | 512.0 KB | `f232e3c437dcc9e4341c0e6a37aea41b` | Factory Binary Firmware Dump |
| `Audi TT 1.8T APX 225HP 8N0906018AE 0261207030 354178.ori` | **1998–2009** | 512.0 KB | `1bb54d5499f69709ac705efc3e939285` | Factory Binary Firmware Dump |
| `Audi TT 1.8T AUQ 180HP 8L0906018Q 0261206790 360287.ori` | **1998–2009** | 1.00 MB | `426194df85a2a51233c47d702878a008` | Factory Binary Firmware Dump |
| `Audi TT 1.8T AUQ 8L0906018Q 0261206790 354029.ori` | **1998–2009** | 1.00 MB | `79430b8eff8d4fcf1d68481ef0c157bc` | Factory Binary Firmware Dump |
| `Audi TT 1.8T BAM 225HP 8N0906018H 0261206795 360313.ori` | **1998–2009** | 1.00 MB | `b2c80d93ad69f566c6d03d2bcf793dbf` | Factory Binary Firmware Dump |
| `Audi TTS 2.0TFSI 272HP 8J0907115Q  0261S02581 393740.ori` | **1998–2009** | 2.00 MB | `9000a778cf5d2fb6db4cab7699fdcade` | Factory Binary Firmware Dump |
| `Audi a2 1,4 tdi 497.mod` | **1998–2009** | 512.0 KB | `e50c7dc9847ff6af915cea9eef4f89c8` | ECU Calibration Asset |
| `Audi a3 1.9TDI AFN 110HP 038906018BA 0281001756 357284.ori` | **1998–2009** | 256.0 KB | `58d6fe14f18a9e70946465624c693c6b` | Factory Binary Firmware Dump |
| `Audi a3 1.9TDI AHF 110HP 038906018AJ 0281001694 357590.ori` | **1998–2009** | 256.0 KB | `e9d53ff5d0951f2b601c88530c1cef2a` | Factory Binary Firmware Dump |
| `Audi a3 19TDI AGR 90HP 0281001693 0381001693 357319.ori` | **1998–2009** | 256.0 KB | `0ab1d701f71446853cfc24c071668707` | Factory Binary Firmware Dump |
| `Audi a3 19TDI AGR 90HP 038906018AH 0281001693 357791.ori` | **1998–2009** | 256.0 KB | `64f35351187a11f3c8086aa660e56bd8` | Factory Binary Firmware Dump |
| `Audi a4 1.9TDI AFN 110HP 028906021EA 0281001490 355111.ori` | **1998–2009** | 256.0 KB | `ba72528ae2ba4cc14db192d9d62a052c` | Factory Binary Firmware Dump |
| `Audi a4 quattro 1.9TDI AFN 110HP 028906021EM 0281001554 355538.ori` | **1998–2009** | 256.0 KB | `59d4d6911b314d7fb39fbb824b86ddbb` | Factory Binary Firmware Dump |
| `Audi_200_B2200_R5V4T_162kW_0261200451_447907404AA_xxx_1267356260_crcF50660DA.ori` | **1998–2009** | 8.0 KB | `63290a8403c51a82f2538a1b419943cf` | Factory Binary Firmware Dump |
| `Audi_200_B2200_R5V4T_162kW_0261200451_447907404AA_xxx_1267356462_crc0AE3CACD.ori` | **1998–2009** | 32.0 KB | `293d29aab3791d44ba9eb431f103fe1e` | Factory Binary Firmware Dump |
| `Audi_200_B2200_R5V4T_162kW_0261200451_447907404A_xxx_1267356259_crcE66098C8.ori` | **1998–2009** | 32.0 KB | `35d87ae2d290eabcebea3ddf5bf5a88d` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001133_8A0907401A_D06_2287357598.ori` | **1998–2009** | 32.0 KB | `e4516ed041d73ca1bd86a3ea8b186dca` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001133_8A0907401A_D06_2287357599.ori` | **1998–2009** | 32.0 KB | `d89f1b0fad5d79cc8369499cb4d1fe90` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001186_8A0907401B_D09_2287357913_crc94FCAED3.ori` | **1998–2009** | 32.0 KB | `c8d1b4426386ae6f11ded164c1f9fb5a` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001186_8A0907401B_D09_2287357914_crc0E0D2C00.ori` | **1998–2009** | 32.0 KB | `153aecc68d5dc6d3fe0a3babb7751fbc` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001198_028906021D_D21_2287358771_crc1DA0C54E.ori` | **1998–2009** | 64.0 KB | `56ef41a08b61734207566c65a58c3336` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001222_028906021E_D56_2287358725_crcD444EC2E.ori` | **1998–2009** | 64.0 KB | `5607b8a06f04fc84ea52d3c49ac6f8b9` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001222_028906021E_D56_2287358726_crcD444EC2E.ori` | **1998–2009** | 64.0 KB | `87f13dd33136dd1cf7425936f89291e2` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001330_028906021AR_D63_2287357893_crc69802A17.ori` | **1998–2009** | 64.0 KB | `4a34a38b350f80392a781874b3b384c6` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001330_028906021AR_D63_2287357894_crc841064DB.ori` | **1998–2009** | 64.0 KB | `d270976b2bf1e151c202aa03a15fb8fb` | Factory Binary Firmware Dump |
| `Audi_80_D1900_R4V2T_66kW_0281001568_028906021FD_KD04_1037358669_670_crc8A7DA418.ori` | **1998–2009** | 256.0 KB | `ffb917eafc5a9475a651799f324bdda7` | Factory Binary Firmware Dump |
| `Audi_A3_1_9l_TDI_PD_Bosch_EDC_16U1.bin` | **1998–2009** | 1.00 MB | `7f75ded28212db74ee0ec3db19d9a8f9` | Factory Binary Firmware Dump |
| `Audi_A3_B1800_R4V5T_165kW_0261206438_06A906032R_0002_1037352355_crc9C3CED82.bin` | **1998–2009** | 512.0 KB | `f86ad4225219bf4df6ed34f839bb316e` | Factory Binary Firmware Dump |
| `Audi_A3_D1900_R42VT_96kW_0281010308_038906019CK_1243_1037360044_crc33B3CFFC.ori` | **1998–2009** | 512.0 KB | `2fef183f3271401c6cc62b4340e0e26c` | Factory Binary Firmware Dump |
| `Audi_A3_D1900_R42VT_96kW_0281010561_038906019EF_1331_1037360585_crc3ED18F25.ori` | **1998–2009** | 512.0 KB | `80490b8f29a1c04af5195606dd5d99f9` | Factory Binary Firmware Dump |
| `Audi_A3_D1900_R4V2T_96kW_0281001308_038906019CK_1243_1037360044_crcF03BD0AF.ori` | **1998–2009** | 512.0 KB | `f4710f6b295ae87f94d540323698cbf3` | Factory Binary Firmware Dump |
| `Audi_A3_D1900_R4V2T_96kW_0281010308_038906019CK_1477_1037362845_crc97223402.ori` | **1998–2009** | 512.0 KB | `9678896614e169b414001b8ca4e93eac` | Factory Binary Firmware Dump |
| `Audi_A3_D1900_R4V2T_96kW_0281010981_038906019FT_1577_1037366273_crc9881DFF6.ori` | **1998–2009** | 512.0 KB | `192b67550e50ccb089e17db5039d42ee` | Factory Binary Firmware Dump |
| `Audi_A3_D2000_R4V4T_103kW_0281011450_03G906016AL_5249_1037368223_crcCFBDEB5B.ori` | **2000** | 1.00 MB | `15c0191cd0e7c19e696f77979b1338d4` | Factory Binary Firmware Dump |
| `Audi_A4_B1800_R4V5T_110kW_0261207854_8E0909518P_0001_1037363386_crc087E0E4B.ori` | **1998–2009** | 1.00 MB | `b24b3998c21e94dac96f1aed7f04d82e` | Factory Binary Firmware Dump |
| `Audi_A4_D1900_ATJ_R4V2T_85kW_0281010094_038906019AN_1063_1037354264.ori` | **1998–2009** | 512.0 KB | `55da173c62d602cd794608a6ac49daf4` | Factory Binary Firmware Dump |
| `Audi_A6_AAT_0281001254_1037355048.ori` | **1998–2009** | 64.0 KB | `1becd231b35898eee7a80802cdb5f7e0` | Factory Binary Firmware Dump |
| `Audi_A6_AAT_0281001254_1037355049.ori` | **1998–2009** | 64.0 KB | `6f0ad22eedbfd1b854034897c7042d77` | Factory Binary Firmware Dump |
| `Audi_A6_TDI_150PS_0281010005_8D1907401_354256_.ori` | **1998–2009** | 512.0 KB | `f0847198ce9a9a7ed7842ba69ddc68d7` | Factory Binary Firmware Dump |
| `Audi_Org_A4_TDI.bin` | **1998–2009** | 2.00 MB | `a897a77ce560306cc7c7e108b1eff156` | Factory Binary Firmware Dump |
| `Audi_Q7_TDI_V6_30_235_383721_4L0910401M_0030.ori` | **1998–2009** | 2.00 MB | `270fb10d695aac18799f92e982b25f96` | Factory Binary Firmware Dump |
| `B4 Passat - GQ - 357270 - LLL683 8.bin` | **1998–2009** | 128.0 KB | `adb1b984e4961020c7ee899911d703e6` | Factory Binary Firmware Dump |
| `B4 Passat - GQ - 357271 - HHH683 8.bin` | **1998–2009** | 128.0 KB | `3c277d1b532d160802637a095a76afe5` | Factory Binary Firmware Dump |
| `Caddy_1_9_TDI_PD_105PS_03G906021HS_381007.ori` | **1998–2009** | 512.0 KB | `f0f90621745293da42ab24f39b3b889d` | Factory Binary Firmware Dump |
| `E2PROM.bin` | **1998–2009** | 4.0 KB | `2f08adc6e4782f71318ae15e8f2a9b04` | Factory Binary Firmware Dump |
| `Eeprom.bin` | **1998–2009** | 4.0 KB | `430610d85d5c1f0045f8caa24633ce61` | Factory Binary Firmware Dump |
| `G3-s827.564.bin` | **1998–2009** | 128.0 KB | `fc1a611ffc2da287250cf91bce4943de` | Factory Binary Firmware Dump |
| `G3-s828.564.bin` | **1998–2009** | 128.0 KB | `2744049fab3a1ed00aa3c2a6c50f93c2` | Factory Binary Firmware Dump |
| `GTI325P.FST.bin` | **1998–2009** | 128.0 KB | `b1dba3033e677a59c827d652ef4a65c5` | Factory Binary Firmware Dump |
| `Golf 3 90PS 0 261 203 593-594 original.bin` | **1998–2009** | 64.0 KB | `3eedbd5b1b0e5ecbe16a82dbf2c96e0f` | Factory Binary Firmware Dump |
| `Golf7045.ori` | **1998–2009** | 256.0 KB | `1f01b9c3d642d184929e3195cd467d0b` | Factory Binary Firmware Dump |
| `HHH 0281001650_028906021GG_1443.bin` | **1998–2009** | 128.0 KB | `5b5b2acc8e7e5d9457003899d9d0749b` | Factory Binary Firmware Dump |
| `HHH 028906021DF_0801.bin` | **1998–2009** | 128.0 KB | `36d2857917e61730464d4986bf3db8a6` | Factory Binary Firmware Dump |
| `HHH_868_ Orig.BIN` | **1998–2009** | 128.0 KB | `9680d3d6f6d940e241ec6d742dd38ad4` | Factory Binary Firmware Dump |
| `IAW 4MV.DR 036906034DR golf 4 1.6 .ori` | **1998–2009** | 512.0 KB | `4e127675e2213c0e69e0378a3f65d68b` | Factory Binary Firmware Dump |
| `KD35.ori` | **1998–2009** | 512.0 KB | `3235a9ea0bae7bf590f2c1a0ce3f6035` | Factory Binary Firmware Dump |
| `LLL 0281001650_028906021GG_1443.bin` | **1998–2009** | 128.0 KB | `7a4e99ae1614f6a07a3942c1ef04f60f` | Factory Binary Firmware Dump |
| `LLL 028906021DF_0801.bin` | **1998–2009** | 128.0 KB | `2c637621095e4c2426a90919706bdcda` | Factory Binary Firmware Dump |
| `LLL_867_ Orig.BIN` | **1998–2009** | 128.0 KB | `d0fe3b53b92a74bf0e362a65f4a82341` | Factory Binary Firmware Dump |
| `MPC555.bin` | **1998–2009** | 232.7 KB | `fbb583722da59d77c0acf74eb30ba584` | Factory Binary Firmware Dump |
| `MPC555_1.bin` | **1998–2009** | 232.1 KB | `d26fffb60a31a87046d21c30fd66fae8` | Factory Binary Firmware Dump |
| `OriginalAudi706B.833.bin` | **1998–2009** | 128.0 KB | `47b1733d291ce86d894c49946b673dc5` | Factory Binary Firmware Dump |
| `OriginalAudi707B.833.bin` | **1998–2009** | 128.0 KB | `a45e96feaf2b1cb63af8122716958abb` | Factory Binary Firmware Dump |
| `PassatPd130.bin` | **1998–2009** | 512.0 KB | `e1c7a42311422d3ae0076e78aa3d74c3` | Factory Binary Firmware Dump |
| `Proc.bin` | **1998–2009** | 2.00 MB | `b81ab9dbcdaba30f2a08f00acc2b4ace` | Factory Binary Firmware Dump |
| `Q 7 full.bin` | **1998–2009** | 755.1 KB | `a0ca0d9c330e01ca17a4351bfa6a30d8` | Factory Binary Firmware Dump |
| `Sander_AUDI_TT_2001_224hp_Q.bin` | **2001** | 512.0 KB | `fb28c5864f8f4f72c9f72626f5c1a835` | Factory Binary Firmware Dump |
| `T4 AMV 022906032B_0261206239_354081.Bin` | **1998–2009** | 1.00 MB | `f9e62bc32cd13488c2616a307112c471` | Factory Binary Firmware Dump |
| `Tiguan_2.0TDi_CR_EDC17_3L906022G_sw106.ori` | **1998–2009** | 2.00 MB | `764a3c177a473e5f3dfb3bed3080c762` | Factory Binary Firmware Dump |
| `VOLKSWAGEN POLO 1300 1267356773 0261200306 27C256 E0D4.ori` | **1998–2009** | 32.0 KB | `91defb224b1bc20b0dec8ed337bdfaa2` | Factory Binary Firmware Dump |
| `VW  NEW BEETLE 1.9TDI 100HP 0281011539 038906019KR 368191.ori` | **1998–2009** | 512.0 KB | `c9cccc17d15a005736561c4822fe9c47` | Factory Binary Firmware Dump |
| `VW 1.6i 06A906033L 5WP4004.ori` | **1998–2009** | 512.0 KB | `37a326168f7055436f4932e1913ab4ed` | Factory Binary Firmware Dump |
| `VW 1.8T G60 Digifant 037997022B - WINOLS.ols` | **1998–2009** | 57.7 KB | `26f072899b84a8961a854c823e30e493` | WinOLS Project Workspace |
| `VW 2.0TDI CFGB 170HP EDC17C46 03L907309R 03L906018BC 1037524625 9784.bin` | **1998–2009** | 2.00 MB | `19a3fba3bffb30d26461fe084692994a` | Factory Binary Firmware Dump |
| `VW Beetle 1.8T 0261207341 06A906032FT 362333.ori` | **1998–2009** | 1.00 MB | `8b376c9e46c92e9b6104da8aaea74689` | Factory Binary Firmware Dump |
| `VW Beetle 1.9TDI 5spd ALH 90HP 038906012GQ 0281011035 366235.ori` | **1998–2009** | 512.0 KB | `7735d74698882f1a57822eb453784223` | Factory Binary Firmware Dump |
| `VW Beetle 1.9TDI auto 038906012FF 0281001655 362776.ori` | **1998–2009** | 512.0 KB | `7418ad592de234420440de5bae91135a` | Factory Binary Firmware Dump |
| `VW Bora 1.8T-150HP-06A906032DR-0261206887-1037360128.bin` | **1998–2009** | 1.00 MB | `c1739e133e36e4458f9f217074122199` | Factory Binary Firmware Dump |
| `VW Caddy 1.9TDI 105HP 03G906021PD 389297.ori` | **1998–2009** | 2.00 MB | `7f7b6aacf85046e4fb05c2b153ca9a04` | Factory Binary Firmware Dump |
| `VW Caddy2 1.9TDI BJB 105HP 03G906016DM 0281011882 371251.bin` | **1998–2009** | 1.00 MB | `5081a6f9585117898e78cfd95ed18322` | Factory Binary Firmware Dump |
| `VW Crafter 2.5 TDI  074906032BB 503934.ori` | **1998–2009** | 2.00 MB | `47df882ae7bb20b75a599fdf12ed5945` | Factory Binary Firmware Dump |
| `VW Crafter EDC16CP34 BDM 0281014133 1037386337.ori` | **1998–2009** | 447.5 KB | `5bbf685778e8305efa1994840ce91c8e` | Factory Binary Firmware Dump |
| `VW GOLF 1.9-100hp-0281011065-1037363709.ori` | **1998–2009** | 512.0 KB | `eb4931804002004f67f6072a3796da46` | Factory Binary Firmware Dump |
| `VW GOLF3 1.8-90hp-0261200784-1H0907311H.bin` | **1998–2009** | 64.0 KB | `603daa1d3851b85308c83a5846ab3248` | Factory Binary Firmware Dump |
| `VW Golf 150PS 1.8L R45VT-06A906018R-0261204673-358109.ori` | **1998–2009** | 256.0 KB | `348a76bcdb398f1e6edcd89633c29d13` | Factory Binary Firmware Dump |
| `VW Golf 2.3 V5 AGZ 150hp 071906018 0261204753 359144.ori` | **1998–2009** | 256.0 KB | `c49f603feba2908eff819a49f2e1fb57` | Factory Binary Firmware Dump |
| `VW Golf 5 1.9TDI BKC 105HP 03G906016CB 0281011900 371429.ori` | **1998–2009** | 1.44 MB | `2ac67ad52a9c2dfbeaa483b94960e8f9` | Factory Binary Firmware Dump |
| `VW Golf 5 3.2 VR6 260HP 022906032CE 0261208468 377419.ori` | **1998–2009** | 1.00 MB | `a54d5fa7b8e831a39b73efd07babb1c5` | Factory Binary Firmware Dump |
| `VW Golf IV ALH 90hp 038906012FA 0281010650 360773.bin` | **1998–2009** | 512.0 KB | `b6accdfacb004a0c23615e1b78702367` | Factory Binary Firmware Dump |
| `VW Golf VII GTI 2.0TFSI Simos18.1 5G0906259 0005 SC800F8300000.ori` | **1998–2009** | 4.50 MB | `6809d6021fe6e4e4479f21acfd2b0790` | Factory Binary Firmware Dump |
| `VW Golf4 1.8T 0261206518 352127.ori` | **1998–2009** | 256.0 KB | `4e7fce43727c39a43c70ca7d75d8150f` | Factory Binary Firmware Dump |
| `VW Golf4 1.8T 06A906032DL 0261206890 354821 Original.bin` | **1998–2009** | 1.00 MB | `37c254e5c7efbd4c21c8934dbde6e348` | Factory Binary Firmware Dump |
| `VW Golf4 1.9 TDI 90hp ALH 0281001979 038906012M 2813.bin` | **1998–2009** | 512.0 KB | `e7ec3df1b8d523336987ef9764a4e2b0` | Factory Binary Firmware Dump |
| `VW Golf4-(1J)-1,9-AGR-90HP-038906018D-0281001611.bin` | **1998–2009** | 256.0 KB | `7d103d5f7da182f4213f9583bfa1a508` | Factory Binary Firmware Dump |
| `VW Golf5 1.9TDI 105HP 0281012220 03G906016R 374183.ori` | **1998–2009** | 1.00 MB | `252f95a518d9c4faad741dc46c15cfd6` | Factory Binary Firmware Dump |
| `VW Golf5 1.9TDI 105HP 03G906021KH 0281013226 382083.ori` | **1998–2009** | 2.00 MB | `8641f69aa1a877bdfb997e118fa1f2dc` | Factory Binary Firmware Dump |
| `VW GolfV (1K) TDI 1,9 BKC-105hp-03G906016CB-0281011900-371094.bin` | **1998–2009** | 1.00 MB | `7c5c7e20d5f70bccb1daae641b615ffb` | Factory Binary Firmware Dump |
| `VW LT 2.5TDI 109HP 074906021AG 0281010088 893HHH.ori` | **1998–2009** | 128.0 KB | `7e93e23ca0334834c7e8419cd2a14669` | Factory Binary Firmware Dump |
| `VW LT 2.5TDI 109HP 074906021AG 0281010088 893LLL.ori` | **1998–2009** | 128.0 KB | `20fde25409a5718b915d0d77c8dddb0d` | Factory Binary Firmware Dump |
| `VW LT 2.5TDI AHD 102HP 074906021AK 0281010086.ori` | **1998–2009** | 256.0 KB | `3f47fd842e131d930c2a194524a9612b` | Factory Binary Firmware Dump |
| `VW LT 2.5TDI AHD 102HP 074906021J 0281001600 358946.ori` | **1998–2009** | 256.0 KB | `03b18870f02b65ba6af239b0c1bc241e` | Factory Binary Firmware Dump |
| `VW LT35 2.5TDI AVR 109HP 074906018BK 0281011385 367887.ori` | **1998–2009** | 512.0 KB | `0b65383a57d1ba1ac81b0965f553e46d` | Factory Binary Firmware Dump |
| `VW LT35 2.8TDI 158HP 2D0906019A 0281010588 365048.ori` | **1998–2009** | 512.0 KB | `c85724fca2968dbec833bcbe0a06fd0b` | Factory Binary Firmware Dump |
| `VW LT35 TDI 889 021AP HHH Original.bin` | **1998–2009** | 128.0 KB | `d7c7e13a14bf6e3a73c5e27572528520` | Factory Binary Firmware Dump |
| `VW LT35 TDI 889 021AP LLL Original.bin` | **1998–2009** | 128.0 KB | `3460e162e9a1425a679edb12abcddae6` | Factory Binary Firmware Dump |
| `VW Lupo 1.4l 16V 100HP 036906034AT IAW4LV.VA 61600.540.05.ori` | **1998–2009** | 512.0 KB | `43e9ebb6437ecc3cd6dfcb05fb88a44d` | Factory Binary Firmware Dump |
| `VW PAssat 2.0 140PS 0281012119 394115.ori` | **1998–2009** | 2.00 MB | `e402f7797f7649ad5be87afd91c64f23` | Factory Binary Firmware Dump |
| `VW PAssat 2.0 CR 140HP  03L906022BL 4145 399883.ori` | **1998–2009** | 2.00 MB | `458503de3e6125fe5336f9b4e42f7a82` | Factory Binary Firmware Dump |
| `VW PAssat 2.0 CR 140HP 03L906022BL 6221 507677.ori` | **1998–2009** | 2.00 MB | `4b09ea3e45a793e0ac9d6e191abaf073` | Factory Binary Firmware Dump |
| `VW POLO GTI 110KW_0261 201 628_1037 38 2997.ori` | **1998–2009** | 1.00 MB | `e02eab7502d361dc2e68d28c3a977e10` | Factory Binary Firmware Dump |
| `VW Passat  1.9TDI 105HP 3G906021LR 380420.ori` | **1998–2009** | 2.00 MB | `c86accc9a58e631081977992778f1abb` | Factory Binary Firmware Dump |
| `VW Passat 1.8T  4B0 906 018 DF  AWT ME7.5 0261207639 original.bin` | **1998–2009** | 1.00 MB | `685e9a63e81b7e16f9c35eb90b72bf48` | Factory Binary Firmware Dump |
| `VW Passat 1.8T 8D0907558E 0261204805 358123.bin` | **1998–2009** | 128.0 KB | `60fe810e387081bdbe51b47b6e34242c` | Factory Binary Firmware Dump |
| `VW Passat 1.9TDI 105HP 03G906021AB 381562.ori` | **1998–2009** | 2.00 MB | `310f95e88915c09faa53a64843bb0d46` | Factory Binary Firmware Dump |
| `VW Passat 1.9TDI 105HP 03G906021NK 382417.ori` | **1998–2009** | 2.00 MB | `2fac6e8648f99d7006957e8d5e825304` | Factory Binary Firmware Dump |
| `VW Passat 2.0 TDI BHW 136HP 038906016R 0281011982 371877.ori` | **1998–2009** | 512.0 KB | `c27a15e0889353aadff360f26515e9fd` | Factory Binary Firmware Dump |
| `VW Passat 2.0FSI 150HP 06F906056AN 0261S02135 376502.ori` | **1998–2009** | 2.00 MB | `3586e8059484d97c44452747e508cb44` | Factory Binary Firmware Dump |
| `VW Passat 2.0TDI  170HP 3L906022BM 396091.ori` | **1998–2009** | 2.00 MB | `8845c5be3aea78f2a93c84e1bc19ffef` | Factory Binary Firmware Dump |
| `VW Passat 2.0TDI 140HP  03G906021AB 03G906021MT 382427.ori` | **1998–2009** | 2.00 MB | `a805f89294609bcaa2dc5b633211e9c6` | Factory Binary Firmware Dump |
| `VW Passat 2.0TDI 140HP 0281012925_03G906021AD_378328.ori` | **1998–2009** | 2.00 MB | `0533cbdfcfb89d692d2bfa11a884764f` | Factory Binary Firmware Dump |
| `VW Passat 2.0TDI 140HP 03G906018CD 9627.ori` | **1998–2009** | 2.00 MB | `9fd5aaa3ff0e2ecad39ea7d99a459650` | Factory Binary Firmware Dump |
| `VW Passat 2.0TDI 140HP 03G906021AB 03G906021NK 399388.ori` | **1998–2009** | 2.00 MB | `cb2111d74e88d55009117423c831732d` | Factory Binary Firmware Dump |
| `VW Passat 2.0TDI 140HP 03G906021NK 1037394904.ori` | **1998–2009** | 2.00 MB | `0acac4297db30c54d5e38881e02b82b3` | Factory Binary Firmware Dump |
| `VW Passat 2.0TDI 170HP PPD 03G906018ER.ori` | **1998–2009** | 2.00 MB | `6762069d958bd729b9b0ea23d3bcb9fe` | Factory Binary Firmware Dump |
| `VW Passat 2.0TDI BKP 140.0PS 03G906018CD  SN000F7600000.bin` | **1998–2009** | 2.00 MB | `2a992c4568a848855a6530ce9c31c652` | Factory Binary Firmware Dump |
| `VW Passat 2.3 V5 0261206508 071906018AC 352012.ori` | **1998–2009** | 256.0 KB | `3236035c06ceb6c678b28627b2085b55` | Factory Binary Firmware Dump |
| `VW Passat 2.3 V5 906018AE 0261206620.ORI` | **1998–2009** | 256.0 KB | `81d89cedab07dd39d639e32cc39ff3ff` | Factory Binary Firmware Dump |
| `VW Passat 3.6 FSI 03H906032C  0261S02169 376323 FSI.ori` | **1998–2009** | 2.00 MB | `33c10f147d07780ce45a04a30e7acda1` | Factory Binary Firmware Dump |
| `VW Passat 3C 19 105ps BKC 0281012085 03G906021AN 374452.bin` | **1998–2009** | 2.00 MB | `3383ad601be09ac1e0173443e9289f12` | Factory Binary Firmware Dump |
| `VW Passat V8 4.0 BDN 07D906018C 0261207019 366337.ori` | **1998–2009** | 1.00 MB | `e4427d45ffc4103e14c52f05fc3d604a` | Factory Binary Firmware Dump |
| `VW Phaeton 3.2V6 AYT 241HP 022906032BN 0261207688 366305.ori` | **1998–2009** | 1.00 MB | `9350fc989abf149641f8dce0ca07fef0` | Factory Binary Firmware Dump |
| `VW Polo 1.7 SDI 44kW 038906013K 0281001749 1808 HHH.bin` | **1998–2009** | 128.0 KB | `c842ef7c5f3bafdf81cf45537028dc02` | Factory Binary Firmware Dump |
| `VW Polo 1.7 SDI 44kW 038906013K 0281001749 1808 LLL.bin` | **1998–2009** | 128.0 KB | `4dbc8d7fa9ed07519430f28e5b81f4ff` | Factory Binary Firmware Dump |
| `VW T4 2.5TDI 102HP 038906018AM 0281010458 360078.ori` | **1998–2009** | 512.0 KB | `ee2af0d8bf19688682c267f8fb757788` | Factory Binary Firmware Dump |
| `VW T4 2.5TDI 102HP 074906018AH 0281010681 362448.ori` | **1998–2009** | 512.0 KB | `1dca06f2517764a2b8bfbe326fb76dc1` | Factory Binary Firmware Dump |
| `VW T4 2.5TDI 102HP 074906018AL 0281010459 360077.ori` | **1998–2009** | 512.0 KB | `8ad9f38f2ae7c06a0ecc3437dc890cf1` | Factory Binary Firmware Dump |
| `VW T4 2.5TDI 88HP 074906018AK 0281010462 360076.ori` | **1998–2009** | 512.0 KB | `c62575761403b5c3580ea475bea38859` | Factory Binary Firmware Dump |
| `VW T4 2.5TDI 88HP 074906018B 0281010084.ori` | **1998–2009** | 512.0 KB | `14672b33489356cafb1061d42e982f76` | Factory Binary Firmware Dump |
| `VW T4 2.5TDI ACV 102HP 074906018C 0281010082.ori` | **1998–2009** | 512.0 KB | `7a2f6dbc81c97f9d3e6bb514a33ffcc5` | Factory Binary Firmware Dump |
| `VW T4 2.5TDI ACV 102HP 074906021L 0281001640 357796.ori` | **1998–2009** | 256.0 KB | `fb1beff674f2d88473d429ec161e486a` | Factory Binary Firmware Dump |
| `VW T5 2.5TDI 130HP 070997016C 0281012931 1037378311.ori` | **1998–2009** | 1.00 MB | `5b067957473bbf623ace15f94ab65eb2` | Factory Binary Firmware Dump |
| `VW T5 2.5TDI 130HP 070997016M 390979.mpc` | **1998–2009** | 251.8 KB | `036cfd92316eef20b367afb94c1ea56e` | ECU Calibration Asset |
| `VW T5 2.5TDI 130HP 070997016M 390979.ori` | **1998–2009** | 2.00 MB | `a95c85d34aeecc441bfaa51393709169` | Factory Binary Firmware Dump |
| `VW T5 2.5TDI 174HP  070906016BA 0281011664 372365.ori` | **1998–2009** | 1.00 MB | `026ca38d187ca4b9cabb2ab15250c462` | Factory Binary Firmware Dump |
| `VW T5 2.5TDI 174HP  070906016EB 0281014892 1037394113.ori` | **1998–2009** | 2.00 MB | `34ea5a5dda2fbce2eb8fc73b8680d873` | Factory Binary Firmware Dump |
| `VW T5 2.5TDI 174HP 070906016BD 0281011835 372944.ori` | **1998–2009** | 1.00 MB | `b0aae3240a6c1cfe93af5ebe141038e0` | Factory Binary Firmware Dump |
| `VW T5 2.5TDI BNZ 130.0PS 070906016EC  394114.bin` | **1998–2009** | 2.00 MB | `071844ec2195298e5e96333188ac4548` | Factory Binary Firmware Dump |
| `VW Tiguan 2.0 170 HP 03L906022G 395496.ori` | **1998–2009** | 2.00 MB | `11d5f6cb39a89045a137c82e0961458b` | Factory Binary Firmware Dump |
| `VW Tiguan 2.0TDI 03L906022G 396096 edc17p14.ori` | **1998–2009** | 2.00 MB | `e8d32f08f78a724dacc4eef2be5cfc0e` | Factory Binary Firmware Dump |
| `VW Touareg 2.5TDI BAC 174HP 070997016E 0281012926 381353.ori` | **1998–2009** | 1.00 MB | `a40e97b0876a2b0814f23997cf5e6dfd` | Factory Binary Firmware Dump |
| `VW Touareg 3.0l TDI 0281013686 7L0907401D 386372.ori` | **1998–2009** | 2.00 MB | `e37634f51a44616bb25366fdff767b3d` | Factory Binary Firmware Dump |
| `VW Touareg 4.2V8 AXQ 310hp 4D0907560BR 0261208009 367701.ori` | **1998–2009** | 1.00 MB | `9319f3693bac5eb772bfd6da66d1743e` | Factory Binary Firmware Dump |
| `VW Touareg 5.0V10TDI AYH 313hp 070906016AA 0281011481 368703.bin` | **1998–2009** | 1.00 MB | `e1b02890c72d112d7103907deb12077b` | Factory Binary Firmware Dump |
| `VW Touareg 5.0V10TDI AYH 313hp 070906016D 0281010736 367461.bin` | **1998–2009** | 1.00 MB | `f0a3143cbdc2b91e0cdba4cb5da7a9e6` | Factory Binary Firmware Dump |
| `VW Touran  2.0TDI 140HP  0281011907 03G906016FK 371267.ori` | **1998–2009** | 1.00 MB | `afba5278e43aef464216f8a9df66e5ca` | Factory Binary Firmware Dump |
| `VW Touran 1.9TDI 105HP 0281012361  03G906016HP 374119.ori` | **1998–2009** | 1.00 MB | `96879fb3158a20d54ec7f95425ed3823` | Factory Binary Firmware Dump |
| `VW Touran 1.9TDI 105HP 03G906021AB 03G906021MG 383708.ori` | **1998–2009** | 2.00 MB | `c061c5c140008d7f8ed46f7b385a52c7` | Factory Binary Firmware Dump |
| `VW Touran 1.9TDI 105HP 03G906021AN 03G906021KC 382090.ori` | **1998–2009** | 2.00 MB | `f964c693b1fd9eefcd89f6c44e22d6ad` | Factory Binary Firmware Dump |
| `VW Touran 1.9TDI 105HP 03G906021HK 394990.ori` | **1998–2009** | 2.00 MB | `a7fe1e69a8c02f207958de22915fa93e` | Factory Binary Firmware Dump |
| `VW Touran 1.9TDI 105HP 03G906021ND 396444.ori` | **1998–2009** | 2.00 MB | `09056a6ecf38e2211606b6f49e68f9a1` | Factory Binary Firmware Dump |
| `VW Touran 1.9TDI AVQ 105HP 03G906016A 0281010731 368159.ori` | **1998–2009** | 1.00 MB | `f03fc76d1669b577754fbbae70dc0bc0` | Factory Binary Firmware Dump |
| `VW Touran 2.0SDI 0281012272 03G906016HN 376308.ori` | **1998–2009** | 1.00 MB | `e46da2bc19ab71a6a83586d569fb4b3b` | Factory Binary Firmware Dump |
| `VW Touran 2.0TDI 140HP 03G906021AB 03G906021MJ 383709.ori` | **1998–2009** | 2.00 MB | `88ffe7e66c211d6b252ab5cfe6c04863` | Factory Binary Firmware Dump |
| `VW Touran 2.0TDI 140HP 03G906021GB 378847.ori` | **1998–2009** | 2.00 MB | `df4e699506f93812122f8447675f5620` | Factory Binary Firmware Dump |
| `VW Touran 2.0TDI 140HP 03G906021KF 381020.ori` | **1998–2009** | 2.00 MB | `0c5b88110b5e6129c7b8a9a48d094d4c` | Factory Binary Firmware Dump |
| `VW Transporter 2.5TDI AXD 131HP 070906016AJ 0281011568 372363.bin` | **1998–2009** | 1.00 MB | `e6cbaa19c6a6533e6abe5d5cbbf2b5ef` | Factory Binary Firmware Dump |
| `VW Transporter T5 1.9PD 85HP 0389060106AH 1037381380.bin` | **1998–2009** | 2.00 MB | `5fdb769dc7d7e1a6557f958b7f53cd1b` | Factory Binary Firmware Dump |
| `VW Transporter T5 1.9TDI 105HP   038906016AJ 390638.ori` | **1998–2009** | 2.00 MB | `ed34bcfc57ba7866b9e79bdbc2405670` | Factory Binary Firmware Dump |
| `VW Transporter T5 1.9TDI 74KW  0281012761 038906016T 384631.ori` | **1998–2009** | 2.00 MB | `50025eed776966ba84bea0eb1c8d91ca` | Factory Binary Firmware Dump |
| `VW Tuareg 3.0L BKS 7L0907401F  0281013686.bin` | **1998–2009** | 768.6 KB | `9cd6be8722b4747b745c352b8e1f6f5d` | Factory Binary Firmware Dump |
| `VW Tuareg 3.0L BKS 7L0907401F  0281013692.bin` | **1998–2009** | 768.0 KB | `4bbf12246b35447f882cebb8993de1d0` | Factory Binary Firmware Dump |
| `VW beetle 1.8T 150HP 06A906032GQ 0261207349 360345.ori` | **1998–2009** | 1.00 MB | `2a6d2715d805a51b8b324f39efb97a54` | Factory Binary Firmware Dump |
| `VW beetle 1.9TDI 100HP 038906019MT 0281011413 367412.ori` | **1998–2009** | 512.0 KB | `d36f041db9f195b75634fe7b4b508831` | Factory Binary Firmware Dump |
| `VW beetle 1.9TDI 100HP 038906019NN 0281011391 368225.ori` | **1998–2009** | 512.0 KB | `6d20f530a1adff288975b04501ea3dc1` | Factory Binary Firmware Dump |
| `VW beetle 1.9TDI ALH 90HP 038906012FH 0281010657 362437.ori` | **1998–2009** | 512.0 KB | `ee18d2bd13d67dde868ebaa8c3645421` | Factory Binary Firmware Dump |
| `VW beetle 1.9TDI ALH 90HP 038906012Q 0281010133 352571.ori` | **1998–2009** | 512.0 KB | `de326dcb9be2f5acd5baf7f44ea64308` | Factory Binary Firmware Dump |
| `VW beetle 1.9TDI ALH 90HP 038906018AP 0281001732 357743.ori` | **1998–2009** | 256.0 KB | `97ebae513f90444281cf374e95e34700` | Factory Binary Firmware Dump |
| `VW beetle 1.9TDI ALH 90HP 038906018M 0281001696 356243.ori` | **1998–2009** | 256.0 KB | `810b58c09dad58ddfbcf27da84cb8cf3` | Factory Binary Firmware Dump |
| `VW bora 1.6 BFQ 06A906033BN 5WP4019 4667.ori` | **1998–2009** | 512.0 KB | `5c814e5d023ebdfa1d4d7b658251287e` | Factory Binary Firmware Dump |
| `VW bora 1.6i 06A906033AQ 5WP4013.ori` | **1998–2009** | 512.0 KB | `2173d8f3877ebdf1f34d973c970237ca` | Factory Binary Firmware Dump |
| `VW bora 1.8T 180HP 06A906032SL 0261208529 371155.ori` | **1998–2009** | 1.00 MB | `02f08ce45017490a665279779c74d97c` | Factory Binary Firmware Dump |
| `VW bora 1.9TDI 115HP 038906019H 0281001910 350172.ori` | **1998–2009** | 512.0 KB | `a6863b47c520a363998e9af129017ed4` | Factory Binary Firmware Dump |
| `VW bora 1.9TDI AGR 90HP 038906012FD 0281010653 362774.ori` | **1998–2009** | 512.0 KB | `9b2fd3ee07ddb8733d90cb1c11cef93d` | Factory Binary Firmware Dump |
| `VW bora 2.0 APK 06A906018FK 0261206261 485757.ori` | **1998–2009** | 256.0 KB | `719bc76f82fb9a4a8a3b25dd099fbac2` | Factory Binary Firmware Dump |
| `VW caddy 1.9SDI 03G906016GP 0281012168 372600.ori` | **1998–2009** | 1.00 MB | `dc81dcd77b8ce1f4d39c7791491ce3c2` | Factory Binary Firmware Dump |
| `VW caddy 1.9SDI 68HP 038906012GJ 0281010965 363111.ori` | **1998–2009** | 512.0 KB | `8c8b291a1419a80ff327d2c85644c7f8` | Factory Binary Firmware Dump |
| `VW caddy 1.9TDI 105HP 03G906021AQ 0281012390 377585.ori` | **1998–2009** | 2.00 MB | `1cb9007134c24cb90377a0b7934fa4c2` | Factory Binary Firmware Dump |
| `VW caddy 1.9TDI 105HP 03G906021CG 0281012746 393550.ori` | **1998–2009** | 2.00 MB | `c5c0fc0fd5f672cfacf53d295cf45741` | Factory Binary Firmware Dump |
| `VW caddy 2.0SDI 75HP 0281011541 03G906016N 369948.ori` | **1998–2009** | 1.00 MB | `9ed34950d636b4a425f56d8cbe477b5c` | Factory Binary Firmware Dump |
| `VW corrado 1.8T PG G60 160HP 037906022B.ori` | **1998–2009** | 32.0 KB | `3bfdc82451740f18922a1e12f38bd879` | Factory Binary Firmware Dump |
| `VW corrado 2.9i VR6 ABV 021906258AG 0261203109 357531.ori` | **1998–2009** | 64.0 KB | `1ec38082794b57b5553d5619abbdceca` | Factory Binary Firmware Dump |
| `VW crafter 2.5TDI  0281014133 074906032AT 10373386337.ori` | **1998–2009** | 2.00 MB | `1d3eb4a3e566fa9a9333380077708d30` | Factory Binary Firmware Dump |
| `VW crafter 2.5TDI 074906032AG 1037383306.ori` | **1998–2009** | 2.00 MB | `9ace94647c49147c5550ef1b58f11c4e` | Factory Binary Firmware Dump |
| `VW crafter 2.5TDI 074906032E  0281012543 381010.ori` | **1998–2009** | 2.00 MB | `ed9d77535a0a6218e108253f6888837a` | Factory Binary Firmware Dump |
| `VW eos  2.0TDI 140HP DPF 03G906021AB 383799.ori` | **1998–2009** | 512.0 KB | `f2125981508b359d8f4b8f93f6ecf0db` | Factory Binary Firmware Dump |
| `VW golf 1.4i AXP 036906032P 0261207179 354828.ori` | **1998–2009** | 512.0 KB | `f5fa0b849ae31ba2ff5d1a04e3ac9602` | Factory Binary Firmware Dump |
| `VW golf 1.6i 06A906033AF 5WP4013.ori` | **1998–2009** | 512.0 KB | `56fc274b2601436ffda25dd64a6865b0` | Factory Binary Firmware Dump |
| `VW golf 1.6i 06A906033BN 5WP4015.ori` | **1998–2009** | 512.0 KB | `b0680a244d216b6d159f051a7b1f0c05` | Factory Binary Firmware Dump |
| `VW golf 1.8 AGN 130HP 06A906018CL 0261206076 359100.ori` | **1998–2009** | 256.0 KB | `1824c0d9f86b8edb06bd342f79c2d9ac` | Factory Binary Firmware Dump |
| `VW golf 1.8T  06A906032LQ 0261207956 367519.ori` | **1998–2009** | 1.00 MB | `a53b94975b53619c51ef88fbea19efba` | Factory Binary Firmware Dump |
| `VW golf 1.8T 150HP 06A906018R 0261204673 359591.ori` | **1998–2009** | 256.0 KB | `fad347545dfc62cea77e5b2be4e2f564` | Factory Binary Firmware Dump |
| `VW golf 1.8T 150HP 06A906032AR 0261206436 1037352758.ori` | **1998–2009** | 512.0 KB | `f427bb39e1bc9937c482246475c2253c` | Factory Binary Firmware Dump |
| `VW golf 1.8T ARZ 150HP 06A906032AR 0261206436 352357.ori` | **1998–2009** | 512.0 KB | `8a9fd00411768d05faf69b365cb5c649` | Factory Binary Firmware Dump |
| `VW golf 1.8T AWV 150HP 06A906032SK 0261208528 371152.ori` | **1998–2009** | 1.00 MB | `26ce9105ac8f2996062eac8bcc91c4d8` | Factory Binary Firmware Dump |
| `VW golf 1.9 110HP 028906021JG 0281001860 356933.ori` | **1998–2009** | 256.0 KB | `896b3291708a30ce9e0a3bd20866fa72` | Factory Binary Firmware Dump |
| `VW golf 1.9SDI 68HP 038906012DB 0281010373 354379.ori` | **1998–2009** | 512.0 KB | `e6e6176806420e74744c8bf495c2c9c0` | Factory Binary Firmware Dump |
| `VW golf 1.9SDI 68HP 038906013 0281001759 356428.ori` | **1998–2009** | 256.0 KB | `33205b8a9b681261b9c11e10cff14ed7` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 028906021ED 0281001541 357815.ori` | **1998–2009** | 256.0 KB | `54fe33db178caba737f813ce0a08b8f0` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 105HP 03G906016B 0281011478 375902.ori` | **1998–2009** | 1.00 MB | `48d29954546b1c97eb1324132160511c` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 105HP 03G906021AB 391847.ori` | **1998–2009** | 2.00 MB | `8f6bed791f410eabcc57dcc5b898e7eb` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 105HP 03G906021AN 382414.ori` | **1998–2009** | 2.00 MB | `fb45bce0e2f8427c20964aaeb3aab6e5` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 105HP 03G906021AN 389140.ori` | **1998–2009** | 2.00 MB | `1e0766cb92e5c156e8a84d9d4b121fd0` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 105HP 03G906021KH 0281013226 380437.ori` | **1998–2009** | 2.00 MB | `26d0fd2f2c5e0d78cab69e54cb2fa1be` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 105HP 03G906021KH 380437.ori` | **1998–2009** | 2.00 MB | `d1a4dfde1ce1b15cbc1da5bb7d315764` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 1Z 90HP 028906021BF 0281001422 355103.ori` | **1998–2009** | 256.0 KB | `8c8eba5fe1aa3f7d0d51bff79a590d30` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 90HP 038906018GR 0281010245 352615.ori` | **1998–2009** | 128.0 KB | `67dd6750177a8ca5c484b5e6f16b47ef` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 90HP 038906018GR 0281010245 352616.ori` | **1998–2009** | 128.0 KB | `e9f371e31dc9dac52bbf4f051369b14a` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 90HP 03G906016FS 0281011955 370811.ori` | **1998–2009** | 1.00 MB | `071951eb1fbb83669dc2bfe7a260deed` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI 90HP ALH 038906018AE 0281001851.ori` | **1998–2009** | 256.0 KB | `808cdabadb04b0a3d0f43f3a5ad0e590` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI AFN 110HP 028906021GT 0281001735.ori` | **1998–2009** | 256.0 KB | `40f5055d5472bb4ec632b96cd1f479f0` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI AGR 90HP 038906018BL 0281001845 359499.ori` | **1998–2009** | 256.0 KB | `916be227bdf5cddcc3d02540bbabb616` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI AHF 110 HP 038906018GP 0281010246 350618.ori` | **1998–2009** | 256.0 KB | `0ef1f8722af57fd5ebc8651f8c48803d` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI AHU 90HP 028906021GG 0281001650 357824.ori` | **1998–2009** | 256.0 KB | `1aabe8c028f055d36e84268dbcff4068` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI AJM 115HP 038906019FC 0281010751 362699.ori` | **1998–2009** | 512.0 KB | `4a03dbbdd0dc027e3e388e84521416ea` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ALE 90HP 028906021HD 0281001729 357948.ori` | **1998–2009** | 256.0 KB | `868484ded4e6431f4b477ac38aaaa2e8` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ALH 90HP 038906012CP 0281010385 354327.ori` | **1998–2009** | 512.0 KB | `950c680fa17d251ec7be7430067c198f` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ALH 90HP 038906012GK 0281010864 362681.ori` | **1998–2009** | 512.0 KB | `f02c07f896901853dc83c5cdc18d3ee8` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ARL 150HP 038906019AQ 0281010048 1037360004.ori` | **1998–2009** | 512.0 KB | `f736ee8592fff9de9e331b9861fec392` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ARL 150HP 038906019FE 0281010744 362470.ori` | **1998–2009** | 512.0 KB | `92e62a80383586ee027dfda32091d0fe` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ARL 150HP 038906019FE 0281010744 362684.ori` | **1998–2009** | 512.0 KB | `6112c6e7006f691e23d3c664c565336b` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ARL 150HP 038906019HH 0281010976 363171.ori` | **1998–2009** | 512.0 KB | `cbe5c16b9e10f79ba44c400140de324a` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ARL 150HP 038906019HH 0281010976 366661.ori` | **1998–2009** | 512.0 KB | `eab8c91667118839ba7e411ff18a6ac5` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ASZ 130HP 038906019HJ 0281010977 363142.ori` | **1998–2009** | 512.0 KB | `8832f81eb510830e802beb93f4190e28` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ASZ 130HP 038906019KJ 0281011216 368577.ori` | **1998–2009** | 512.0 KB | `0b094a024d942baa39907344457e0ba5` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ATD 100HP 038906019AT 0281010974 366203.ori` | **1998–2009** | 512.0 KB | `b1b4fe2889598af2a97bebf5e4e59c59` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ATD 100HP 038906019CR 0281010663 362817.ori` | **1998–2009** | 512.0 KB | `e8a8d77383df202bdca981cd88d97d83` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI ATD 100HP 038906019FF 0281010662 362734.ori` | **1998–2009** | 512.0 KB | `ffbae98f69051419772b9a68449dd657` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI AUY 115HP 038906019AM 0281010091 350875.ori` | **1998–2009** | 512.0 KB | `733c035679872e6a279f2654f2291401` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI AXR 100HP 038906019KP 0281011191 366912.ori` | **1998–2009** | 512.0 KB | `927351a68684b691d4ebf10b43df14c6` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI BKC 105HP 03G906016B 0281011478 368926.ori` | **1998–2009** | 1.00 MB | `e24b3c650be6a049d3a986a3ac82ee93` | Factory Binary Firmware Dump |
| `VW golf 1.9TDI BKC 105HP 03G906016B 0281011478 369564.ori` | **1998–2009** | 1.00 MB | `ca2c0f552f731745ab26cb8e1bcf8238` | Factory Binary Firmware Dump |
| `VW golf 2.0 TFSI 200HP 1K0907115F 0261S02217 377837.ori` | **1998–2009** | 2.00 MB | `8b3216f96ef5ef436c7d95f1fb35965c` | Factory Binary Firmware Dump |
| `VW golf 2.0GTI 037906024D FALA03001390.ori` | **1998–2009** | 32.0 KB | `6f1fafcdbf6af1ae17b0c6fa5c5bd6d9` | Factory Binary Firmware Dump |
| `VW golf 2.0TDI 140HP 03G906016AN 0281011477 368925.ori` | **1998–2009** | 1.00 MB | `944c6547cc56acd87444908a2e2a44b1` | Factory Binary Firmware Dump |
| `VW golf 2.0TDI 140HP 03G906016HJ 0281012253 372673.ori` | **1998–2009** | 1.00 MB | `c759d5370748ec03706d278e1703dc2b` | Factory Binary Firmware Dump |
| `VW golf 2.0TDI 140HP 03G906021PP 1037389263 1264.ori` | **1998–2009** | 2.00 MB | `8adaf9949903e825672315edf17e6921` | Factory Binary Firmware Dump |
| `VW golf 2.0TDI 140HP 03G906021PR 1037387083.ori` | **1998–2009** | 2.00 MB | `2debe8a06a1c1e7f945650099cdf5ada` | Factory Binary Firmware Dump |
| `VW golf 2.0TDI 170HP 03G906018FB.ori` | **1998–2009** | 2.00 MB | `c8c6482c1401718df1207404f1142487` | Factory Binary Firmware Dump |
| `VW golf 2.0TDI BKD 140HP 03G906021KK 0281013228 1037381019.ori` | **1998–2009** | 2.00 MB | `da5f1980f851a48681cd4adc71fd8328` | Factory Binary Firmware Dump |
| `VW golf 2.0TFSI 1K0907115 0261S02078 387570.ori` | **1998–2009** | 2.00 MB | `7f6e7f7c51a131412243f144ac0d7471` | Factory Binary Firmware Dump |
| `VW golf 2.0TFSI 200HP 1K0907115 0261S02078  377862.ori` | **1998–2009** | 2.00 MB | `3135c24ff5b32c60bd0b0b260e537ec9` | Factory Binary Firmware Dump |
| `VW golf 2.0TFSI 200HP 1K0907115 0261S02078 372620.ori` | **1998–2009** | 2.00 MB | `3b0b28b5c43aa7e357db16421c0d13f1` | Factory Binary Firmware Dump |
| `VW golf 2.0TFSI 200HP 1K0907115J 0261S02331 386464.ori` | **1998–2009** | 2.00 MB | `c20b23ff6c115dc1cd766139cc18dc36` | Factory Binary Firmware Dump |
| `VW golf 2.8 VR6 021906258CL 0261203559 358929.ori` | **1998–2009** | 64.0 KB | `821b7f208e07508cc162d69da64f1347` | Factory Binary Firmware Dump |
| `VW golf 2.8 VR6 AAA 021906258A 0261200496 357205.ori` | **1998–2009** | 64.0 KB | `dc1b1c577f336811f8f506af1aacbaff` | Factory Binary Firmware Dump |
| `VW golf 2.8V6 174HP 021906018R 0261206814 360624.ori` | **1998–2009** | 512.0 KB | `db066ef5c39da3f467d8a3b91afabe7e` | Factory Binary Firmware Dump |
| `VW golf 3 1.9SDI 028906021FJ 0281001560 781-782.ori` | **1998–2009** | 256.0 KB | `ae7c5882107a172a9db57521a59daf2d` | Factory Binary Firmware Dump |
| `VW golf 3 1.9TDI 90HP 028906021C 0281001171.ori` | **1998–2009** | 64.0 KB | `effb6af4ba8e1c997834f7c8b5508b87` | Factory Binary Firmware Dump |
| `VW golf 3 1.9TDI 90HP 028906021HG 0281001730 357946.ORI` | **1998–2009** | 256.0 KB | `1cfb6d94a17e01980e5784b49ef6d4cc` | Factory Binary Firmware Dump |
| `VW golf 3 1.9TDI AFN 110HP 028906021GH 0281001652 358905.ori` | **1998–2009** | 256.0 KB | `9d429577a010b5eac949be899f00756d` | Factory Binary Firmware Dump |
| `VW golf 3 2.8 VR6 174HP 021906258CH 0261203569 358928.ori` | **1998–2009** | 64.0 KB | `69876639239f102ac69dbcd2253e8183` | Factory Binary Firmware Dump |
| `VW golf 3 2.8V6 174HP 021906256 0261203969 559385.ori` | **1998–2009** | 128.0 KB | `bb2564f6b165eab46be6ca4e3ef855e0` | Factory Binary Firmware Dump |
| `VW golf 3 VR6 2.8 174HP 0261203117 021906258AF 357529.ori` | **1998–2009** | 64.0 KB | `89818de6bccaaecd81532da8c17b6214` | Factory Binary Firmware Dump |
| `VW golf 3.2 VR6 250HP 022906032EG 0261208344 373693.ori` | **1998–2009** | 1.00 MB | `88574cb164be12f0995d8450913ca799` | Factory Binary Firmware Dump |
| `VW golf 4 1.6 06A906019AK 5WP4417 (1B6F).ori` | **1998–2009** | 256.0 KB | `d909d7f2b28bc68c7eded156cdce91db` | Factory Binary Firmware Dump |
| `VW golf 4 1.6 5WP4448.03 (7001).ori` | **1998–2009** | 256.0 KB | `3d7cbc922eae7047b0e0a21bb9010a3c` | Factory Binary Firmware Dump |
| `VW golf 4 1.6 5WP4872.03 (2704).ori` | **1998–2009** | 256.0 KB | `16426dfdd2be08215fa06aed71759e7f` | Factory Binary Firmware Dump |
| `VW golf 4 1.9TDI 130HP 038906019FG 0281010702 362796.ori` | **1998–2009** | 512.0 KB | `e2cc21028126cafc864faf3909bd5cc1` | Factory Binary Firmware Dump |
| `VW golf 4 1.9TDI AHF 110HP 038906012L 0281010112 352566.ori` | **1998–2009** | 512.0 KB | `c28a74ea0cb5e2d6efb40b57fcd4ca3a` | Factory Binary Firmware Dump |
| `VW golf 4 1.9TDI AWX 130HP 038906019JQ 0281011142 366047.ori` | **1998–2009** | 512.0 KB | `b0aa6fd1b08feb2ddffaa0eb31568dfd` | Factory Binary Firmware Dump |
| `VW golf 4 16 5WP4426.02 (6A4E).ori` | **1998–2009** | 256.0 KB | `74a5d5f26d7d25244c7c2adc88d6d041` | Factory Binary Firmware Dump |
| `VW golf 5 1.9SDI 0281011617 03G906016M 370652.ori` | **1998–2009** | 1.00 MB | `88cfcaf36e8fd9a4a250794edd87168b` | Factory Binary Firmware Dump |
| `VW golf 5 1.9SDI 69HP 03G906016GJ 0281012221 372340.ori` | **1998–2009** | 1.00 MB | `22b87e5952a7f501a1b883e1405b27b7` | Factory Binary Firmware Dump |
| `VW golf 5 1.9TDI 038906016H 0281011146 371297.ori` | **1998–2009** | 2.00 MB | `12d0f0ba8a750fccf96d5126cfc06ad9` | Factory Binary Firmware Dump |
| `VW golf 5 2.0TDI 140HP 03G906016ET 0281011843 375890.ori` | **1998–2009** | 1.00 MB | `28c17ae124ef1342f57d14e3c575a08a` | Factory Binary Firmware Dump |
| `VW golf 5 2.0TFSI 200HP 1K0907115 0261S02078 374094.ori` | **1998–2009** | 2.00 MB | `92592259ff8bdb20f047d727e3e67d93` | Factory Binary Firmware Dump |
| `VW golf 5 R32 022906032CD 0261208467 377452.ori` | **1998–2009** | 1.00 MB | `014cb3e812402f4bc3d05c0b3d367fce` | Factory Binary Firmware Dump |
| `VW golf IV 1.9TDI AHF 110HP 038906018J 0281001613.ori` | **1998–2009** | 256.0 KB | `9cbbb00fce72ed0a8a1c4893fd1bb5f1` | Factory Binary Firmware Dump |
| `VW golf IV 1.9TDI AJM 115HP 038906019CJ 0281010302 352930.ori` | **1998–2009** | 512.0 KB | `0bdfdefddbdbf22fac9858f4707b3b5e` | Factory Binary Firmware Dump |
| `VW golf IV 1.9TDI ARL 150HP 038906019FE 0281010744 362706.ori` | **1998–2009** | 512.0 KB | `ec621cad44bfbf599b3dfaf2522bdfbc` | Factory Binary Firmware Dump |
| `VW golf IV 1.9TDI ASV 110HP 038906012AP 0281010126 352577.ori` | **1998–2009** | 512.0 KB | `83d4d2233ab0b099dce395d89449bab9` | Factory Binary Firmware Dump |
| `VW golf V 2.0TDI 140HP DPF 03G906021JG 394134.ori` | **1998–2009** | 2.00 MB | `39a9f3f88348d2e58514b19e1adcef68` | Factory Binary Firmware Dump |
| `VW golf4 AHF 110hp 038906018BM 0281001846 356590.ori` | **1998–2009** | 256.0 KB | `3b2aa5c36d4fe93410ddf6db5c768763` | Factory Binary Firmware Dump |
| `VW golf4 ALH 90HP 038906012M 0281001979 352564.ori` | **1998–2009** | 512.0 KB | `b0f7eafd6a82287ed2c129c5ddd8a386` | Factory Binary Firmware Dump |
| `VW golf4 ALH P0HP 038906018AN 0281001733.ori` | **1998–2009** | 256.0 KB | `2ba8ecb731390c1bf1bcc6fb92004e18` | Factory Binary Firmware Dump |
| `VW golf5 2.0TFSI 1K0907115K 0261S02332 380991.ori` | **1998–2009** | 2.00 MB | `39248a1974d057ffdd784ffc816f5119` | Factory Binary Firmware Dump |
| `VW golf5 2.0TFSI DSG 1K0907115E 0261S02082 387576.ori` | **1998–2009** | 2.00 MB | `11bd2121434b833a171b1b742b350e83` | Factory Binary Firmware Dump |
| `VW industrial engine 1.9TDI AFD 82HP 028906021JQ 0281010266.ori` | **1998–2009** | 256.0 KB | `f5f065e0d070b8b1faf742618b6b1461` | Factory Binary Firmware Dump |
| `VW jetta 1.8T AWD 150HP 06A906032CL 0261206552 1037354128.ori` | **1998–2009** | 512.0 KB | `fd354e45f7d6d1130cb52b94f457d821` | Factory Binary Firmware Dump |
| `VW jetta 2.0TDI CBEA 03L906022KS 397837.ori` | **1998–2009** | 2.00 MB | `7cb48bc84a41fd3f5dcb01f60efbf7a9` | Factory Binary Firmware Dump |
| `VW jetta 2.8 VR6 021906018M 0261206486 352765.ori` | **1998–2009** | 512.0 KB | `a7be15ab5f8cfa6f20d3570a698cbdd3` | Factory Binary Firmware Dump |
| `VW lupo 1.2TDI 61HP 045906019Q 0281010258 1037352679.ori` | **1998–2009** | 512.0 KB | `a82ca3191ee41a204d39400c58cf0f02` | Factory Binary Firmware Dump |
| `VW lupo 1.2TDI 61HP 045906019Q 0281010258 352999.ori` | **1998–2009** | 512.0 KB | `c6731a4862158f992f031d798fe3bee1` | Factory Binary Firmware Dump |
| `VW lupo 1.4TDI 75HP 045906019L 0281010049 352592.ori` | **1998–2009** | 512.0 KB | `5419965ce70858c14488b74fcd96219c` | Factory Binary Firmware Dump |
| `VW lupo 3L 1.2TDI 61HP 0281010015 045906019K 1211 354603.ori` | **1998–2009** | 512.0 KB | `119316a0d67783da8a98231857f3edaa` | Factory Binary Firmware Dump |
| `VW lupo 3L 1.2TDI 61HP 0281010505 045906019AA 1313 360520.ori` | **1998–2009** | 512.0 KB | `8adf1042f8c4cf6eeb0d5cb7d935132e` | Factory Binary Firmware Dump |
| `VW lupo 3L 1.2TDI 61HP 0281010628 045906019AE 1508 351992.ori` | **1998–2009** | 512.0 KB | `bdde56c6368f3e793c6cb062d84c0ebb` | Factory Binary Firmware Dump |
| `VW lupo 3L 1.2TDI 61HP 0281010628 045906019AE 1537 363567.ori` | **1998–2009** | 512.0 KB | `98ae1757481629a8a2e532fa8255f922` | Factory Binary Firmware Dump |
| `VW pasat 2.5TDI 150HP 3B1907401F 0281010444 354375.ori` | **1998–2009** | 512.0 KB | `2aed0537df12d18754142603b5eaa141` | Factory Binary Firmware Dump |
| `VW passat 1.8T 150HP 4B0906018AG 0261206453 352151.ori` | **1998–2009** | 512.0 KB | `9800dd92b807b0a393edf95cde99a6c6` | Factory Binary Firmware Dump |
| `VW passat 1.8T 163HP 8E0909018A 0261207928 366497.ori` | **1998–2009** | 1.00 MB | `5ae48132a1da15114e27ec06e90f3822` | Factory Binary Firmware Dump |
| `VW passat 1.8T 4B0906018CC 0261206871 354009.ori` | **1998–2009** | 1.00 MB | `31485a44e78a62a13663251062bb184b` | Factory Binary Firmware Dump |
| `VW passat 1.8T ADR 8D0907558S 0261204956 356669.ori` | **1998–2009** | 128.0 KB | `b1a6a8316b8bbbf9911dee4f50c800ed` | Factory Binary Firmware Dump |
| `VW passat 1.8T ANB 150HP 4B0906018BF 0261206525 352710.ori` | **1998–2009** | 512.0 KB | `18d5c2c157eda469b63b205a6cdb3c9e` | Factory Binary Firmware Dump |
| `VW passat 1.8T APU 150HP 4B0906018B 0261206050 350229.ori` | **1998–2009** | 512.0 KB | `9bc64e151b5437b47af5e7f7c4cf26e7` | Factory Binary Firmware Dump |
| `VW passat 1.8i APT 125HP 8D0906018F 0261204875 350087.ori` | **1998–2009** | 512.0 KB | `fbdcbd97f835180209a48462087af90f` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 100HP 038906019BM 0281010307 1037360022.ori` | **1998–2009** | 512.0 KB | `721209421b36ab3206bfda06539156c2` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 100HP 038906019BM 0281010307 1037360476.ori` | **1998–2009** | 512.0 KB | `3e0653a8b2772071ada8207d4e71c226` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 115HP 038906019AJ 0281010303 352975.ori` | **1998–2009** | 512.0 KB | `161814a282497d33265b8dbb0b2a3db9` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 130HP 038906019EP 0281010701 362631.ori` | **1998–2009** | 512.0 KB | `082df225eceaf13429a6ae9735c7f188` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 130HP 038906019EQ 0281010700 362632.ori` | **1998–2009** | 512.0 KB | `9b954a56ff58885f5f49e68bb48559cd` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 1Z 90HP 0281001328 355573.ori` | **1998–2009** | 64.0 KB | `8ec954e536622f90729d313430722d40` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 1Z 90HP 0281001328 355574.ori` | **1998–2009** | 64.0 KB | `06ee3b096b6033949b760645626f2381` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 1Z 90HP 028906021AT 0281001369 355101.ori` | **1998–2009** | 256.0 KB | `a7647fb21b38e2902175de7a222cf6da` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI 90HP 038906018FG 0281010063 350164.ori` | **1998–2009** | 256.0 KB | `0ae6940c52a789e8cd256f244d37c68b` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AFN 110HP 028906021GL 0281001656 357830.ori` | **1998–2009** | 256.0 KB | `838c0e7fada5aa8a73b78a5f6f17a82b` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AFN 110HP 038906018FE 0281010064.bin` | **1998–2009** | 256.0 KB | `20448663dd9e802b17c10f4ff1eadf63` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AFN 110HP 038906018GA 0281010170 920.ori` | **1998–2009** | 256.0 KB | `d2591d95d5c31e968c45d741e96721c1` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AFN 110HP 038906018P 0281001720 356815.ori` | **1998–2009** | 256.0 KB | `c5fcf922173fe7ab842d5dd77c4b75d5` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AFN 110HP 038906018P 0281001720 358385.ori` | **1998–2009** | 256.0 KB | `e8bcd6b451fa138c40df1dae117bb654` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AHH 90HP 038906018AS 0281001724 359461.ori` | **1998–2009** | 256.0 KB | `e0aa69c32ba56da86130420088578ef4` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AHU 028906021EG 0281001558 355806.ori` | **1998–2009** | 256.0 KB | `6194accaeaed634157b7db7dbaf8c578` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AHU 90HP 028906021GG 0281001650 357824.ori` | **1998–2009** | 256.0 KB | `aff0b63a4c86c6102d59e723b67b0d86` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AHU 90HP 028906021GK 0281001654 357832.ori` | **1998–2009** | 256.0 KB | `0c2d2fd90b54f418c987aaa2bdd1a7e1` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AHU 90HP 028906021GK 0281001654.ori` | **1998–2009** | 256.0 KB | `d5cf880aebb99e93037e6cb81a91fe70` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AHU 90HP 038906018FQ 0281001172 350924.ori` | **1998–2009** | 256.0 KB | `de28df053646acdd4c351ae1a2e0f8c3` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AJM 115HP 038906019A 0281001691 350100.ori` | **1998–2009** | 512.0 KB | `90db9c2bb59f2f18af7c4b04e1c47ca9` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AJM 115HP 038906019AJ 0281010303 354614.ori` | **1998–2009** | 512.0 KB | `8791eac02741c3ce67bae09f36860e72` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AJM 115HP 038906019BJ 0281010176 350953.ori` | **1998–2009** | 512.0 KB | `c9725849105da4b935aa2f9c49dcf5ff` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AJM 115HP 038906019BK 0281010305 352976.ori` | **1998–2009** | 512.0 KB | `d1b3be3eda85841e014fc00988b5a76c` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AJM 115HP 038906019CD 0281010218 352904.ori` | **1998–2009** | 512.0 KB | `074e256aba5cde43bc956d131f021c85` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI ARL 130HP 038906019KE 0281011201 366297.ori` | **1998–2009** | 512.0 KB | `08edf8cc2e42fae1d74c607a94206421` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI ATJ 115HP 038906019DM 0281010470 354455.ori` | **1998–2009** | 512.0 KB | `41dc7162a150a50af2dbf3e75fd58c35` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVB 100 HP 038906019EJ 0281010665 362053.ori` | **1998–2009** | 512.0 KB | `886fb6de0080e8494f08a578cd077e70` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVB 100HP 038906019EB 0281010553 360009.ori` | **1998–2009** | 512.0 KB | `c4905d64f50198c07f8db49b2d13a184` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVB 100HP 038906019EK 0281010667 362051.ori` | **1998–2009** | 512.0 KB | `48a423b75b682b6f95f878654f7ddcf4` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVB 100HP 038906019GK 0281010943 362893.ori` | **1998–2009** | 512.0 KB | `982340d8b2a7c81d8cf7294511a40f05` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVB 100HP 038906019GL 0281010944 362894.ori` | **1998–2009** | 512.0 KB | `4ce4f73c46e5984614ac0a729fdf4abc` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVB 115HP 038906019EA 0281010554 360477.ori` | **1998–2009** | 512.0 KB | `5db1ae5c56293f95e7c976c86439dcfe` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVF 130HP 038906019BN 0281010404 360707.ori` | **1998–2009** | 512.0 KB | `6ac0a11713427cd335a751acdef7987b` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVF 130HP 038906019DS 0281010543 360449.ori` | **1998–2009** | 512.0 KB | `156a9b0036f787e905a02cff581a4713` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVF 130HP 038906019DS 0281010543 360705.ori` | **1998–2009** | 512.0 KB | `1a67793460eae74d228b13eba3e6c696` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVF 130HP 038906019EN 0281010705 362633.ori` | **1998–2009** | 512.0 KB | `3cd9dcc8a344289b9d8b534cc7fa5695` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVF 130HP 038906019GQ 0281010941 363213.ori` | **1998–2009** | 512.0 KB | `8fd0e887826a084a45d9cc3d3f80b1c6` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AVF 130HP 038906019KD 0281011205 366501.ori` | **1998–2009** | 512.0 KB | `e3b4775aa95809cea4d2d80050cb6262` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AWX 130HP 038906019EH 0281010558 360706.ori` | **1998–2009** | 512.0 KB | `a1a77fef6d52e4c9c1dc752301586930` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AWX 130HP 038906019ER 0281010704 362704.ori` | **1998–2009** | 512.0 KB | `1e7c362c94be8b9512a3059b8227bf11` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI AWX 130HP 038906019GS 0281010940 366946.ori` | **1998–2009** | 512.0 KB | `7429682a211db4f32ae3c1f7d4c3b450` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI BKC 105HP 03G906021DP 0281012724 1037377575.ori` | **1998–2009** | 2.00 MB | `80e4f51a5d9222da24097c05c20ababd` | Factory Binary Firmware Dump |
| `VW passat 1.9TDI PD 130HP 038906019GS 0281010940 363212.ori` | **1998–2009** | 512.0 KB | `e59cfbb289c03cbf5ba92fe29d747cd3` | Factory Binary Firmware Dump |
| `VW passat 2.0TD 140HP 03G906018 9722.ori` | **1998–2009** | 2.00 MB | `ddde058a7198ed0e3b4cae72d164b4a3` | Factory Binary Firmware Dump |
| `VW passat 2.0TDI 140HP 038906016K 0281011145 372127.bin` | **1998–2009** | 512.0 KB | `321f19a1afa9bedc8222b78eb154b52b` | Factory Binary Firmware Dump |
| `VW passat 2.5 AVB 150HP 3B1907401B 0281010447 360452.ori` | **1998–2009** | 512.0 KB | `fe6382f0cfefee3c6bf70804eb85fc8d` | Factory Binary Firmware Dump |
| `VW passat 2.5TDI 150HP 3B0907401H 0281010145 351026.ori` | **1998–2009** | 256.0 KB | `22296ff51c06beb6e3a9fbf4130596f1` | Factory Binary Firmware Dump |
| `VW passat 2.5TDI 150HP 3B1907401B  0281010447 366617.ori` | **1998–2009** | 512.0 KB | `ffbff51ea216ef5a9b4d83122c7317f4` | Factory Binary Firmware Dump |
| `VW passat 2.5TDI 150HP 3B1907401B 0281010447 366617.ori` | **1998–2009** | 512.0 KB | `be4914ab0b8522a0c335a52b396de006` | Factory Binary Firmware Dump |
| `VW passat 2.5TDI AFB 150HP 3B0907401 0281001938 359796.ori` | **1998–2009** | 256.0 KB | `3f8d1ba4239f679b33be809b87bb6746` | Factory Binary Firmware Dump |
| `VW passat 2.5TDI AFB 150HP 3B0907401G 0281010146 027-028.ori` | **1998–2009** | 256.0 KB | `8a025c1414ac5dde65818fa09a6f955b` | Factory Binary Firmware Dump |
| `VW polo 1.4TDI 75HP 045906019BF 0281011241 368175.ori` | **1998–2009** | 512.0 KB | `d9860605253ec837506182ef832cc470` | Factory Binary Firmware Dump |
| `VW polo 1.4TDI AMF 75HP 045906019AB 0281010503 354620.ori` | **1998–2009** | 512.0 KB | `00938d44d1dfea1d20b432489c60ad2e` | Factory Binary Firmware Dump |
| `VW polo 1.4TDI AMF 75HP 045906019AP 0281010865 363954.ori` | **1998–2009** | 512.0 KB | `40dcdd8c4576d621da812b009732cc18` | Factory Binary Firmware Dump |
| `VW polo 1.9SDI 64HP 038906012AR 0281010109 350846.ori` | **1998–2009** | 512.0 KB | `5d3042c5ed8c677ff88fef894320d0d1` | Factory Binary Firmware Dump |
| `VW polo 1.9SDI 74HP 038906012HL 0281011319 367056.ori` | **1998–2009** | 512.0 KB | `00372e7c222587dee90506cc536a0b30` | Factory Binary Firmware Dump |
| `VW polo 1.9TDI ALH 90HP 038906018ED 0281001915 356955.ori` | **1998–2009** | 256.0 KB | `56126d6c979bb801e339d670c2860049` | Factory Binary Firmware Dump |
| `VW polo 1.9TDI ATD 110HP 038906019JK 0281011075 363985.ori` | **1998–2009** | 512.0 KB | `ed12eedc788da4c71fab028392a00fa8` | Factory Binary Firmware Dump |
| `VW polo 1.9TDI AXR 100HP 038906019NC 0281011819 371274.ori` | **1998–2009** | 512.0 KB | `02dbe4d08a22dcf0d72a33aa4d207fed` | Factory Binary Firmware Dump |
| `VW polo 1.9TDI AXR 100HP 03890619JM 0281011029 363220.ori` | **1998–2009** | 512.0 KB | `b8eda2105e43489407961408a8ce1aa3` | Factory Binary Firmware Dump |
| `VW sharan 1.9TDI 1Z 90HP 028906021ES 0281001531 357820.ori` | **1998–2009** | 256.0 KB | `52add5d710256971fdf103504ac73746` | Factory Binary Firmware Dump |
| `VW sharan 1.9TDI AJM 115HP 038906019FC 0281010751 362766.ori` | **1998–2009** | 512.0 KB | `b348575f0b5decb0019075ccc642e555` | Factory Binary Firmware Dump |
| `VW sharan 1.9TDI AJM 115HP 038906019FC 0281010751 363162.ori` | **1998–2009** | 512.0 KB | `04bcbce1f4cc08b348e24b7cd9f9f3fc` | Factory Binary Firmware Dump |
| `VW sharan 1.9TDI AJM 130HP 038906019FC 0281010751 363953.ori` | **1998–2009** | 512.0 KB | `ce878127a630a5096a7d85f190ef4e71` | Factory Binary Firmware Dump |
| `VW sharan 1.9TDI ANU 90HP 038906019AB 0281001865 354276.ori` | **1998–2009** | 512.0 KB | `9316aa4e21ee4f640774f949e6a02a56` | Factory Binary Firmware Dump |
| `VW sharan 1.9TDI ARL 150HP 038906019NQ 0281012287 372714.ori` | **1998–2009** | 512.0 KB | `7553a33bc5b2461688b62807004c914b` | Factory Binary Firmware Dump |
| `VW sharan 1.9TDI ASZ 130HP 0281011199 69546.ori` | **1998–2009** | 512.0 KB | `96df0f37bd801d18bff41ee6dfdb0c57` | Factory Binary Firmware Dump |
| `VW sharan 1.9TDI AUY 115HP 038906019LQ 0281011144 366943.ori` | **1998–2009** | 512.0 KB | `56579d841d560ac5d6eb51382b57bc81` | Factory Binary Firmware Dump |
| `VW sharan 2.8V6 174HP021906256Q 0261203665 355640.ori` | **1998–2009** | 128.0 KB | `ae0716b04aee667ff4cba28d52ee768d` | Factory Binary Firmware Dump |
| `VW touareg 2.5TDI 174HP 070997016E 387080.ori` | **1998–2009** | 1.00 MB | `e656c4350eaa10c3dd6e2634ccd341a0` | Factory Binary Firmware Dump |
| `VW touareg 2.5TDI BAC 174HP 070906016BL 0281011859 371909.ori` | **1998–2009** | 1.00 MB | `28d737cdf67a2081e3d07e08f2b4518c` | Factory Binary Firmware Dump |
| `VW touareg 3.0TDI 8E0907401AB 7L0907401 0281011960 374592.ori` | **1998–2009** | 2.00 MB | `f33a779af12f29c5105fdf9a2e370504` | Factory Binary Firmware Dump |
| `VW touareg 5.0TDI 313HP 070906016D 0281010736 368400.ori` | **1998–2009** | 1.00 MB | `541a1c7422d71018058de38d7178e24d` | Factory Binary Firmware Dump |
| `VW touran 1.9TDI 105HP 0281011945 03G906016CD 371097.ori` | **1998–2009** | 1.00 MB | `8924996fbf05e3b404036de3e78da66c` | Factory Binary Firmware Dump |
| `VW touran 1.9TDI 105HP 03G906021AN 383726.ori` | **1998–2009** | 2.00 MB | `3a47c0fde2c74a3fb21b65a8080d90b0` | Factory Binary Firmware Dump |
| `VW touran 1.9TDI AVQ 105HP 0281011761 37600.ori` | **1998–2009** | 1.00 MB | `f45e4f381b2ead4ef2bb0e5f0103f65c` | Factory Binary Firmware Dump |
| `VW touran 2.0TDI 140HP 03G906016EH 0281011786 375893.ori` | **1998–2009** | 1.00 MB | `e0d4f6cc96027c43ff4dd4da071a92bd` | Factory Binary Firmware Dump |
| `VW touran 2.0TDI 170HP PPD 03G906018EH 0498.ori` | **1998–2009** | 2.00 MB | `afb9c9d820efb2b0b320d5738480ec71` | Factory Binary Firmware Dump |
| `VW touran 2.0TDI BKD 140HP 03G906016BQ 0281011906 371266 SW6254.ori` | **1998–2009** | 1.00 MB | `482ebe8bc748d0e6d06ca2f73beaf547` | Factory Binary Firmware Dump |
| `VW touran 2.0TDI BKD 140HP 03G906016BQ 0281011906 391561.bin` | **1998–2009** | 1.00 MB | `beb614bcecbeefa7ad314ddacb99c007` | Factory Binary Firmware Dump |
| `VW transporter 1.9TDI 85HP 038906016 0281010734 368205.ori` | **1998–2009** | 1.00 MB | `ff3e8a304209cf2d833993de21f04969` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI 102HP 074906018BG 0281010631 362439.ori` | **1998–2009** | 512.0 KB | `98e8ebada56243afd4263601f7f53ce3` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI 102HP 074906021A 0281001306 865.ori` | **1998–2009** | 256.0 KB | `8f34df7d9d3b0a6f99a947dd8eb1313a` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI 130HP 070906016A 0281010733 368186.ori` | **1998–2009** | 1.00 MB | `0220b5031639a9865f03f04ba8b832b9` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI 130HP 070997016M 1037394151.ori` | **1998–2009** | 2.00 MB | `8e831a58e6d3223e67d6479e719b0986` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI 174HP 0281011271 372941.ori` | **1998–2009** | 1.00 MB | `f6f121c6f5590ed4692e1a6ebf404d03` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI 174HP 070906016A 0281010733 368413.ori` | **1998–2009** | 1.00 MB | `012869d2878ce53463e82d17af14b73c` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI 174HP 070906016BF 0281011837 372367.ori` | **1998–2009** | 1.00 MB | `3ec2400b7ecb0337f5141088b3d938df` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI AHY 150HP 074906018AN 0281010490 354499.ori` | **1998–2009** | 512.0 KB | `949c134a4145fb151ccb6bd3dd192816` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI AJT 87HP 074906018 0281010462 362446.ori` | **1998–2009** | 512.0 KB | `352183e187d7b8b4e71f0130f6d23383` | Factory Binary Firmware Dump |
| `VW transporter 2.5TDI AXE 174HP 070906016A 0281010733 370230.ori` | **1998–2009** | 1.00 MB | `29b90a840525a0f7485b41833967cf43` | Factory Binary Firmware Dump |
| `VW transporter 2.8i AES 021906256H 0261203971 355227.ori` | **1998–2009** | 128.0 KB | `a6a66fcea594f74e49e2bff14cf49625` | Factory Binary Firmware Dump |
| `VW-Caddy-1_9TDI-03G906021PF-AB.bin` | **1998–2009** | 2.00 MB | `d35dcd6b2e9c647dcf6a9a07b8a48410` | Factory Binary Firmware Dump |
| `VW-golf-AHU-90hp-028906021JB-1037358314-lll778.bin` | **1998–2009** | 128.0 KB | `6b936898f293f6327919c1b9828f39b4` | Factory Binary Firmware Dump |
| `VW-golf-AHU-90hp-028906021JB-1037358315-hhh778.BIN` | **1998–2009** | 128.0 KB | `b278cbd6083b5a703d48985dc7a369ec` | Factory Binary Firmware Dump |
| `VWTransporterT4-4592443.ORI` | **1998–2009** | 512.0 KB | `0d2069fa8649b14f50c6ab507bea1af0` | Factory Binary Firmware Dump |
| `VW_Audi_115_Cv._0281010176_1037350953.ori` | **1998–2009** | 512.0 KB | `6b48a5c5b6c8347d0fe6ecb308d24ad3` | Factory Binary Firmware Dump |
| `VW_Bora_D1900_R4V2T_96kW_0281010702_038906019FG_1420_1037362471_crc69AA584A.ori` | **1998–2009** | 512.0 KB | `b51a2b5761b7c6ed2d9f8fc9510d9607` | Factory Binary Firmware Dump |
| `VW_Bora_D1900_R4V2T_96kW_0281010702_038906019FG_1470_1037362796_crcBE32A56A.ori` | **1998–2009** | 512.0 KB | `59ccbe3ec6f0e30eb225a1ef87faf7eb` | Factory Binary Firmware Dump |
| `VW_Golf3_D1900_R4V2_47kW_0281001408_028906021CQ_D7X_2537355973_crc9938199D.ori` | **1998–2009** | 64.0 KB | `47c0a9cd23b29248256bc290d4bc3908` | Factory Binary Firmware Dump |
| `VW_Golf3_D1900_R4V2_47kW_0281001408_028906021CQ_D7X_2537355974_crcD85057C8.ori` | **1998–2009** | 64.0 KB | `81173452d3674ee4a30d56e2ed812fde` | Factory Binary Firmware Dump |
| `VW_Golf4_D1900_R4V2T_74KW_0281010662_038906019FF_1355_1037362018_CRC1A832F65.ori` | **1998–2009** | 512.0 KB | `4ee160c5157aa37c06b542d4a6b388bb` | Factory Binary Firmware Dump |
| `VW_Golf4_D1900_R4V2T_74kW_0281010497_038906019DF_1237_1037360018_crc896A38D2.ori` | **1998–2009** | 512.0 KB | `4d26a2f4b344c47c5942e8ecac583b52` | Factory Binary Firmware Dump |
| `VW_Golf_GT_1,4TSI_170PS_0261201770_03C906032C_500422_.ori` | **1998–2009** | 2.00 MB | `43cda77858898850babea98f8ec23635` | Factory Binary Firmware Dump |
| `VW_Golf_MK3_2.0_ABA_115hp_0261203720_1037355532.bin` | **1998–2009** | 512.0 KB | `3a03ba6ffef7ad98ea17d4378da5c917` | Factory Binary Firmware Dump |
| `VW_Golf_MK3_2.0_ABA_115hp_0261204634_1037358768.bin` | **1998–2009** | 512.0 KB | `8f917b85ba5b1be016a7c156023e2a2b` | Factory Binary Firmware Dump |
| `VW_Jetta_IV_1_9l_TDI_PD_Bosch_EDC_16U34.bin` | **1998–2009** | 512.0 KB | `8a1c5688ff914790dd5235337dcab554` | Factory Binary Firmware Dump |
| `VW_Passat_(B5)_1_8l_Turbo_Bosch_ME_7_5.bin` | **1998–2009** | 512.0 KB | `4ef1b557faaf8de9a8d13c69e79e7d57` | Factory Binary Firmware Dump |
| `VW_Passat_1.9Tdi_66kW_0281001727_038906018N_1615_1037357703.ols` | **1998–2009** | 545.1 KB | `6115530f4efece130b541cb550c9a9f4` | WinOLS Project Workspace |
| `VW_Passat_130PSPD_0281010705_038906019EN_362701_1463.ori` | **1998–2009** | 512.0 KB | `feff955fe01dbc8a7f294cbd1ecbc4b8` | Factory Binary Firmware Dump |
| `VW_Passat_D1900_R4V2T_66kW_0281001727_038906018N_1615_1037357703_crcF4227CA9.ori` | **1998–2009** | 256.0 KB | `d65565efb2acae8600c402d3c29910f4` | Factory Binary Firmware Dump |
| `VW_Passat_D1900_R4V2T_81kW_0281010170_038906018GA_3102_1037354238_239_crcCD39720D.ori` | **1998–2009** | 256.0 KB | `665790c3e1c9f7db49bb8bd18ffc5d91` | Factory Binary Firmware Dump |
| `VW_Passat_D2500_V6V4T_132kW_0281011387_8E0907401J_0004_1037367775_crc81E4BFE5.ori` | **1998–2009** | 1.00 MB | `67b12da06a2ce710e2e09e6b0731c882` | Factory Binary Firmware Dump |
| `VW_Passat_v6_2.5tdi_0281010147__HHH.bin` | **1998–2009** | 128.0 KB | `f7e91a5bdaa80883c2939b4b68bc23b3` | Factory Binary Firmware Dump |
| `VW_Passat_v6_2.5tdi_0281010147__LLL.bin` | **1998–2009** | 128.0 KB | `d0e037cf873251c913256dce8b887042` | Factory Binary Firmware Dump |
| `VW_Sharan_D1900_R4V2T_85kW_0281010216_038906019J_1254_1037360085_crc6DEB4AE4.ori` | **1998–2009** | 512.0 KB | `5ce77db0480f3962f1ac9d2aba56bd7c` | Factory Binary Firmware Dump |
| `VW_Sharan_D1900_R4V2T_85kW_0281011144_038906019LQ_1594_1037366943_crc428A525A.ori` | **1998–2009** | 512.0 KB | `4abf873aa36c41fb7205f3ab7f7729fa` | Factory Binary Firmware Dump |
| `VW_T4_D2500_R5V2T_111kW_0281010078_074906018N_2529_1037352548_crc0741FC58.ori` | **1998–2009** | 512.0 KB | `8b107acc9760f88492c44803a2da59c8` | Factory Binary Firmware Dump |
| `VW_T4_D2500_R5V2T_111kW_0281010079_074906018D_2531_1037352222_crcCC55EE0E.ori` | **1998–2009** | 512.0 KB | `7d601db95617dbceaac773644c368493` | Factory Binary Firmware Dump |
| `VW_T4_D2500_R5V2T_111kW_0281010461_074906018AJ_3323_1037360079_crc7E14F711.ori` | **1998–2009** | 512.0 KB | `dcf2f271ec56a084a4a38a3802b34330` | Factory Binary Firmware Dump |
| `VW_T4_D2500_R5V2T_111kW_0281010461_074906018AJ_3908_1037362445_crc6C2E0DDC.ori` | **1998–2009** | 512.0 KB | `75825974bbaca6b04fde56a0fc96e092` | Factory Binary Firmware Dump |
| `VW_Touareg_3_0l_TDI_V6_Bosch_EDC_16CP_386372.bin` | **1998–2009** | 512.0 KB | `544ff77dae7123d7501a039ae29339aa` | Factory Binary Firmware Dump |
| `VW_Touareg_D5000_V10V4T_230kW_0281010736_070906016D_4939_367325_crc698F0982.ori` | **1998–2009** | 1.00 MB | `dcca18acb173c4d7c8a9bdb90bb14ade` | Factory Binary Firmware Dump |
| `VWbo18t890stock.BIN` | **1998–2009** | 1.00 MB | `374fa11618194e1c05baabb77e1b3682` | Factory Binary Firmware Dump |
| `Vw Caddy 19Tdi  105HP 03G906021_0281012469.ori` | **1998–2009** | 2.00 MB | `078c08230849cdd1151871a13e94d15a` | Factory Binary Firmware Dump |
| `Vw Touareg V6 3.2L 4 Motion Aut 2004 022906032FT-0261208619-1037371624.ori` | **2004** | 1.00 MB | `53c5d325dad3cceda282574b1c1d730b` | Factory Binary Firmware Dump |
| `Vw passat 1.9TDI 105HP 03G906021AN_03G906021LR 382088.ori` | **1998–2009** | 2.00 MB | `e92b3256b9b632df982f567be9358490` | Factory Binary Firmware Dump |
| `Vw sharan 2.8LV6 174HP 021906256Q 0261203665 355640.ori` | **1998–2009** | 128.0 KB | `8bcaa9699dfd131616430d4ab3ecd18c` | Factory Binary Firmware Dump |
| `Vw touareg V6 3.2L 4Motion 022906032BF 0261207566 1037368623.ori` | **1998–2009** | 1.00 MB | `6c5add705d4392adc080edf859f758e0` | Factory Binary Firmware Dump |
| `Vw_Polo_TDI_PD_19_100_0281011820_371260_6118_019ND.ori` | **1998–2009** | 512.0 KB | `03c5f708c26c8e88677e85c7f93c2117` | Factory Binary Firmware Dump |
| `WV Passat B6 1.9 TDI PD 03G906021NG 394906.ori` | **1998–2009** | 2.00 MB | `30e012335f15d96dc4e3ece5d01613a3` | Factory Binary Firmware Dump |
| `WinOLS (Audi Q7 (Original) as (All elements) - 396098).bin` | **1998–2009** | 512.0 KB | `0b82d0bbb0a2598acd18ada5c72c2047` | Factory Binary Firmware Dump |
| `a6-8057.ori` | **1998–2009** | 128.0 KB | `ec2dc829d6a2c63eeb2feb6f2a36e22f` | Factory Binary Firmware Dump |
| `a6-8058.ori` | **1998–2009** | 128.0 KB | `d8ffe8a728dcbd4398574557e15e5de3` | Factory Binary Firmware Dump |
| `eeprom.bin` | **1998–2009** | 4.0 KB | `414ca09ce41aa17293c91231d18617ed` | Factory Binary Firmware Dump |
| `eeprom_1.bin` | **1998–2009** | 4.0 KB | `34874a877917aa088fce8ef4f55f1948` | Factory Binary Firmware Dump |
| `flash.bin` | **1998–2009** | 1.00 MB | `d91886127113e1a0335ab14d8c7554ac` | Factory Binary Firmware Dump |
| `flash_cmd.bin` | **1998–2009** | 2.00 MB | `4512b2ca9d87c105a8a2e903b9e2320b` | Factory Binary Firmware Dump |
| `mcu.ori` | **1998–2009** | 232.8 KB | `c2e78212668d70c8b170417baf04ed45` | Factory Binary Firmware Dump |
| `mpc.bin` | **1998–2009** | 232.2 KB | `ef2fd35aa185e896bb0eb7a8734e385e` | Factory Binary Firmware Dump |
| `mpc555.bin` | **1998–2009** | 452.0 KB | `860da135541449bd6bdda96ec2e1b8f3` | Factory Binary Firmware Dump |
| `orginal.bin` | **1998–2009** | 1.00 MB | `782d9f95b1a377816a5cca12e7b24499` | Factory Binary Firmware Dump |
| `orig585.bin` | **1998–2009** | 64.0 KB | `3e8dcb98f0ed342cff406fb54bcced1c` | Factory Binary Firmware Dump |
| `orig586.BIN` | **1998–2009** | 64.0 KB | `631dde9eba853e5530c710fd6a37e44a` | Factory Binary Firmware Dump |
| `orig696.bin` | **1998–2009** | 64.0 KB | `dc128b1b7dbc2052ed34494eee042860` | Factory Binary Firmware Dump |
| `orig697.bin` | **1998–2009** | 64.0 KB | `d5c3f75c485dd7edb4f5e29c9cb8f4b5` | Factory Binary Firmware Dump |
| `original-hhh.bin` | **1998–2009** | 128.0 KB | `b56ff22f33ca5a2813aeb13b29b98e57` | Factory Binary Firmware Dump |
| `original-lll.bin` | **1998–2009** | 128.0 KB | `3062c271e7224b0c7f7d38e44266bc11` | Factory Binary Firmware Dump |
| `original.bin` | **1998–2009** | 32.0 KB | `a0d5502dd2254d32ea12a790d8e8ee04` | Factory Binary Firmware Dump |
| `pastdi358702.ori` | **1998–2009** | 64.0 KB | `a285afca93d718bc95f554250e1926b2` | Factory Binary Firmware Dump |
| `pastdi358703.ori` | **1998–2009** | 64.0 KB | `e3fc83c18ee45a8322f85193b2b43a1f` | Factory Binary Firmware Dump |
| `serial e2prom.bin` | **1998–2009** | 4.0 KB | `fe35e2e525f59b2f4377ba9e479a4041` | Factory Binary Firmware Dump |
| `sharan370538.ori` | **1998–2009** | 1.00 MB | `af809d320a7e61c1e11f7ecf672d2b6a` | Factory Binary Firmware Dump |
| `sharan_90hp_019LP.bin` | **1998–2009** | 512.0 KB | `e73843ab960a444b74f60fba647b7c60` | Factory Binary Firmware Dump |
| `t5_flash.bin` | **1998–2009** | 2.00 MB | `031a000c2f9317971bfadf8384824b74` | Factory Binary Firmware Dump |
| `vw golf 1.9tdi 150bhp 038906019HH 366661.ori` | **1998–2009** | 512.0 KB | `78117ba9adf7c1c88eca0fed32da5485` | Factory Binary Firmware Dump |

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
