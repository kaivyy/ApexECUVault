# UNDERBONE_SONIC_GTR_SUPRA_WAVE - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/UNDERBONE_SONIC_GTR_SUPRA_WAVE`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `88 files` (11 binary dumps, 77 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `UNDERBONE_SONIC_GTR_SUPRA_WAVE` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `GENERATIONAL_38770-K56-N11_Honda_Supra_GTR_150___Winner_150_Gen_1_2016_2019.xdf` | **2016–2019** | 2.5 KB | `31e1c88bae5ce092750c2c4cb8f905ff` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K56-V01_Honda_Supra_GTR_150_Facelift___Winner_X_Gen_2_2020_2025.xdf` | **2020–2025** | 2.5 KB | `81a935aa05dbf578f054d1433f740657` | TunerPro Binary Definition Map |
| `HONDA_38770-K03-H01_Wave_110i_(2019-2020).xdf` | **2019–2020** | 16.3 KB | `83c66f3e176403cd768dbae3d7e55a9c` | TunerPro Binary Definition Map |
| `HONDA_38770-K03-N32_Wave_110i_(2019-2020).xdf` | **2019–2020** | 16.3 KB | `015881b8365da9ceae6370da66897617` | TunerPro Binary Definition Map |
| `HONDA_38770-K03-T61_Wave_110i_(2019-2020).xdf` | **2019–2020** | 16.3 KB | `539ea836ebe64f39dae29a55f7d71a09` | TunerPro Binary Definition Map |
| `HONDA_38770-K0G-962_Super_Cub_110_Pro.xdf` | **2000–2024** | 16.3 KB | `9c4130552261fc3d513df19fc895795d` | TunerPro Binary Definition Map |
| `HONDA_38770-K1M-T01_Wave_110i_AT.xdf` | **2000–2024** | 16.3 KB | `fef0fa3a1ad066a622742850f6452b24` | TunerPro Binary Definition Map |
| `HONDA_38770-K2J-T01_Wave_110i___Super_Cub_(2021-2024).xdf` | **2021–2024** | 16.3 KB | `ba90f63f75a5fce6715a6440099297f7` | TunerPro Binary Definition Map |
| `HONDA_38770-K2J-TH1_Wave_110i___Super_Cub_(2021-2024).xdf` | **2021–2024** | 16.3 KB | `5a0c0b639829b5e5a179abd244107d8d` | TunerPro Binary Definition Map |
| `HONDA_38770-K3F-T01_Wave_125i_(2023-2024).xdf` | **2023–2024** | 16.3 KB | `f6ef6f4fba5792d31d9f86efc3a3469e` | TunerPro Binary Definition Map |
| `HONDA_38770-K41-N01_Honda_Generic_ECM.xdf` | **2000–2024** | 16.3 KB | `d043342651d733c15524b86dd4bf3e95` | TunerPro Binary Definition Map |
| `HONDA_38770-K56-M01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | **2000–2024** | 16.3 KB | `22874846d9f56b0346582d6505a8a99c` | TunerPro Binary Definition Map |
| `HONDA_38770-K56-M91_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | **2000–2024** | 16.3 KB | `c923a3291944f11190f0495b710a5ab0` | TunerPro Binary Definition Map |
| `HONDA_38770-K56-N01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | **2000–2024** | 16.3 KB | `1ee2606f0f0a71796ba6055fce096ff4` | TunerPro Binary Definition Map |
| `HONDA_38770-K56-N11_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | **2000–2024** | 16.3 KB | `8c3bd6e09366cb58639ab1acfd56b23f` | TunerPro Binary Definition Map |
| `HONDA_38770-K56-NJ1_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | **2000–2024** | 16.3 KB | `6d24822a012224bd66152eb4b51662d0` | TunerPro Binary Definition Map |
| `HONDA_38770-K56-V01_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | **2000–2024** | 16.3 KB | `7624073fdb3cd06250e5849d1af93495` | TunerPro Binary Definition Map |
| `HONDA_38770-K56-V51_Sonic_150R___Winner_150___Supra_GTR_150.xdf` | **2000–2024** | 16.3 KB | `2142c033cb4ad34b34b1dfdc924be487` | TunerPro Binary Definition Map |
| `HONDA_38770-K58-N41_Wave_110i___Wave_125i_(2020-2022).xdf` | **2020–2022** | 16.3 KB | `8bcac327a7bd537a753932bca153b9ac` | TunerPro Binary Definition Map |
| `HONDA_38770-K58-T81_Wave_110i___Wave_125i_(2020-2022).xdf` | **2020–2022** | 16.3 KB | `f9db79628a955871b1f53fc14e0b362b` | TunerPro Binary Definition Map |
| `HONDA_38770-K58-TC2_Wave_110i___Wave_125i_(2020-2022).xdf` | **2020–2022** | 16.3 KB | `f770e2ea15d577912f27499461f5c7c6` | TunerPro Binary Definition Map |
| `HONDA_38770-K73-M41_Wave_125i_LED_(2018-2022).xdf` | **2018–2022** | 16.3 KB | `9dbfd5162b5b6ba7bc1d5606e747de6e` | TunerPro Binary Definition Map |
| `HONDA_38770-K73-M62_Wave_125i_LED_(2018-2022).xdf` | **2018–2022** | 16.3 KB | `fa0b5ad99a903974a448d5e3503198bc` | TunerPro Binary Definition Map |
| `HONDA_38770-K73-T32_Wave_125i_LED_(2018-2022).xdf` | **2018–2022** | 16.3 KB | `5df4e799416553c5fabfb2a5d1dada91` | TunerPro Binary Definition Map |
| `HONDA_38770-K73-T61_Wave_125i_LED_(2018-2022).xdf` | **2018–2022** | 16.3 KB | `5a5ce89eb9bce0398a807f97945b1284` | TunerPro Binary Definition Map |
| `HONDA_38770-K73-TC2_Wave_125i_LED_(2018-2022).xdf` | **2018–2022** | 16.3 KB | `a6fb52a298ae790b99d6809f2386ebe7` | TunerPro Binary Definition Map |
| `HONDA_38770-K73-V42_Wave_125i_LED_(2018-2022).xdf` | **2018–2022** | 16.3 KB | `eb9d639164306c16cdb0190b7b67d428` | TunerPro Binary Definition Map |
| `HONDA_38770-KWW-642_Wave_110i_(2009-2018).xdf` | **2009–2018** | 16.3 KB | `4f958d2f80bd6516da4f48186f425ece` | TunerPro Binary Definition Map |
| `HONDA_38770-KWW-643_Wave_110i_(2009-2018).xdf` | **2009–2018** | 16.3 KB | `3e4475b1a650d89731d288da22bf6f0e` | TunerPro Binary Definition Map |
| `HONDA_38770-KYZ-713_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | **2012–2017** | 16.3 KB | `d25fc4d7dfd904a3c6e2b5381cf15ea8` | TunerPro Binary Definition Map |
| `HONDA_38770-KYZ-T03_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | **2012–2017** | 16.3 KB | `85fcd3d80b80926dac880192e385f125` | TunerPro Binary Definition Map |
| `HONDA_38770-KYZ-T41_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | **2012–2017** | 16.3 KB | `8ae487239fe180e49085f8240f4dcf0a` | TunerPro Binary Definition Map |
| `HONDA_38770-KYZ-V21_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | **2012–2017** | 16.3 KB | `a6786c118ec0acb4d8f3803d6403fd44` | TunerPro Binary Definition Map |
| `HONDA_38770-KYZ-V71_Wave_125i_ปลาวาฬ_(2012-2017).xdf` | **2012–2017** | 16.3 KB | `72955f4fac3e9fe514cbdf8a054d60e3` | TunerPro Binary Definition Map |
| `HONDA_38770-KZV-A61_Dream_Super_Cub_110_(2013-2017).xdf` | **2013–2017** | 16.3 KB | `41597f2fff8c5060b79fe97944ed87b4` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-613_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `2934588c1b859b09463f3a2894ad9ae1` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-622_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `2239cfb6e9b438ffd3f29f661b979a5b` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-643_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `828375be4c525eee96da16f234b4769f` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-A21_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `197c727f4e6a8e631f9c80703ceebfe6` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-A22_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `54a2a10cee06d9093ad96319e1468fb5` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-D01_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `4fa6fcf1fd1370b57bf833cba154c0a2` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-D21_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `eef57e7ed5da588c3ea974dfea6181ff` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-F21_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `9bdec75b341d0ee2d05cd226b49e092d` | TunerPro Binary Definition Map |
| `HONDA_38770-MEL-L22_CBR1000RR_Fireblade_(2004-2007).xdf` | **2004–2007** | 16.3 KB | `ef46533c82313270826d446ef63e2d91` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-622_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `18c351aa7acdabfd767e9a8542750047` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-644_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `a45bb09a434feb3d9ee40d516cfbba66` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-671_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `c3b49e4258fec87c636c010317c3f300` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-691_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `1602707b8fd98a561ab4ae94fcd921fb` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-702_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `ee183962fdba5fe6fa4f830bbca73f37` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-741_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `09baf8993cbcf5df48c28d1875a7ab72` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-761_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `7c439c75f77451a2133170a4af2ee46f` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-773_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `597c88bde2023a936c2d326cd4efc174` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-861_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `7d75e51eb9861254238541673683b454` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-871_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `659e4a8fc6966b68cf6245f92c26bd95` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-A21_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `e66ff030ff3f591c972089d54fde8d67` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-D21_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `9b7a8e331ba756825e3dfe455dfeb365` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-F21_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `41a34771ec0eb070e6c01c6252ff7bf9` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-J21_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `56a0ec70362dca374b5d0582b79a3c61` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-J41_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `17362fd573330f00f299a0f95a9d4ac4` | TunerPro Binary Definition Map |
| `HONDA_38770-MFL-L21_CBR1000RR_Fireblade_(2008-2011).xdf` | **2008–2011** | 16.3 KB | `f70c066b7cd1c65cad421776692dfb1d` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-A01_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `cf7ef363198b243fe7692c3b68060fce` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-A92_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `8f3a1a84ac4ac626d9de3fa62817da42` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-D01_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `07586808c5981b56a6673314b4bc049e` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-D62_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `484bd1eeb3d16f010b7ffdbbcfb90313` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-F01_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `a5b5683e57ccbb5e00f05f33dcfd4a18` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-F63_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `466ef4475fb88608fffaf7ebde6210ca` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-J01_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `798cad1b5afca3e7d2d72aa47eac875b` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-L01_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `0262a1ed1e79f53163f11db0a7a6cdf6` | TunerPro Binary Definition Map |
| `HONDA_38770-MGP-T42_CBR1000RR_Fireblade_(2012-2016).xdf` | **2012–2016** | 16.3 KB | `0223fe427a6c1e8014d9cc1713ab5347` | TunerPro Binary Definition Map |
| `HONDA_38770-MKF-A22_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | **2017–2019** | 16.3 KB | `ce2c7a5e3616501e9ec5ae216934d225` | TunerPro Binary Definition Map |
| `HONDA_38770-MKF-D43_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | **2017–2019** | 16.3 KB | `7d9f6456ca0152826f65c8ba3491bc32` | TunerPro Binary Definition Map |
| `HONDA_38770-MKF-D72_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | **2017–2019** | 16.3 KB | `93e51c0b4a5a951f8a8137c10f65cb7e` | TunerPro Binary Definition Map |
| `HONDA_38770-MKF-H11_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | **2017–2019** | 16.3 KB | `30ddab21f88a5cf36e7a61cce4c7be4e` | TunerPro Binary Definition Map |
| `HONDA_38770-MKF-L13_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | **2017–2019** | 16.3 KB | `c3052b3d2d121850ed4eaeb477a113f5` | TunerPro Binary Definition Map |
| `HONDA_38770-MKFA-A22_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | **2017–2019** | 16.3 KB | `54c1bf7ebc0498d2577af82d5d51d67f` | TunerPro Binary Definition Map |
| `HONDA_38770-MKFA-D72_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | **2017–2019** | 16.3 KB | `8bc493e1b4cb80d9258e2e3029a6e839` | TunerPro Binary Definition Map |
| `HONDA_38770-MKFA-DK2_CBR1000RR_SP___Fireblade_(2017-2019).xdf` | **2017–2019** | 16.3 KB | `78b297db896d5d5b8f33deaa05f4701a` | TunerPro Binary Definition Map |
| `HONDA_DREAM_SUPERCUB_38770_K1M_T01_64KB_ORI.bin` | **2000–2024** | 64.0 KB | `d7127626ab25d97c258b52ce9d61e379` | Factory Binary Firmware Dump |
| `HONDA_SUPERCUB_38770_KZV_T03_48KB_ORI.bin` | **2000–2024** | 48.0 KB | `dfb8614f4c3f2b499816ec7fbd0ffa18` | Factory Binary Firmware Dump |
| `HONDA_SUPRA_X_125_38770_KYL_T01_56KB_ORI.bin` | **2000–2024** | 56.0 KB | `49083bb3b77b24bf3315f20210305ef9` | Factory Binary Firmware Dump |
| `HONDA_SUPRA_X_125_38770_KYZ_T03_48KB_ORI.bin` | **2000–2024** | 48.0 KB | `8a26ef3852ab48cbc5173a4bc7f3429e` | Factory Binary Firmware Dump |
| `HONDA_SUPRA_X_125_38770_KYZ_T41_64KB_ORI.bin` | **2000–2024** | 64.0 KB | `32a9cfa3ebb6ef3f9db696059dd74d26` | Factory Binary Firmware Dump |
| `HONDA_SUPRA_X_125_HELMIN_38770_K73_T32_64KB_ORI.bin` | **2000–2024** | 64.0 KB | `d6828dbad35fdbd830fdcc3b63808201` | Factory Binary Firmware Dump |
| `HONDA_WAVE_REVO_110I_38770_K03_H01_64KB_ORI.bin` | **2000–2024** | 64.0 KB | `98800e165fe238eb602fe06612315f32` | Factory Binary Firmware Dump |
| `HONDA_WAVE_REVO_110I_38770_K03_T61_48KB_ORI.bin` | **2000–2024** | 48.0 KB | `dfb8614f4c3f2b499816ec7fbd0ffa18` | Factory Binary Firmware Dump |
| `HONDA_WAVE_REVO_110I_38770_K2J_T01_64KB_ORI.bin` | **2000–2024** | 64.0 KB | `e15af43c7a6e5e44acbc0eede9fc5060` | Factory Binary Firmware Dump |
| `HONDA_WAVE_REVO_110I_38770_K58_T81_64KB_ORI.bin` | **2000–2024** | 64.0 KB | `cf8a1f9c9b67a6559725bf4fcc8fec16` | Factory Binary Firmware Dump |
| `HONDA_WAVE_REVO_110I_38770_KWW_643_48KB_ORI.bin` | **2000–2024** | 48.0 KB | `46db456c64520cbe0ea2c11d8d125b4b` | Factory Binary Firmware Dump |

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
