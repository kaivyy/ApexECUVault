# PRELUDE ACCORD - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/PRELUDE_ACCORD`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `55 files` (16 binary/calibration dumps, 37 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `PRELUDE_ACCORD` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Accord & Prelude V6/I4 Engine Management Platform. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

* **Rentang Tahun / Model Year**: 1992–2017

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `37805-5A2-A160_Honda_Accord_2013_LX__LX-S__Sport_2.4L__L4_-_Gas.xdf` | **2013** | 103.9 KB | `05041a03d038568b7e712845cce96cd8` | TunerPro Binary Definition Map |
| `37805-5AM-A050_Honda_Accord_2014_EX__EX-L_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | **2014** | 130.1 KB | `9c05036c128a262328310259126a0410` | TunerPro Binary Definition Map |
| `37805-5G2-A050_Honda_Accord_2013_EX-L_3.5L_V6_-_Gas.xdf` | **2013** | 71.3 KB | `a574cc7e0feb3628229d1a255351d648` | TunerPro Binary Definition Map |
| `37805-5G2-A120_Honda_Accord_2015_EX-L_3.5L_V6_-_Gas.xdf` | **2015** | 70.2 KB | `2c563d443a483fd84d48c5de3addcb30` | TunerPro Binary Definition Map |
| `37805-R40-A240_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | **2008–2009** | 4.9 KB | `5d6bf66d4ff12e5bd7bc391b42fa96c8` | TunerPro Binary Definition Map |
| `37805-R40-A340_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas___ECU_Honda_Accord.xdf` | **2010** | 5.0 KB | `212b05816de64cc56eaf79dfa9cb0e74` | TunerPro Binary Definition Map |
| `37805-R40-A340_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas___ECU_Honda_Accord_2.4_16v_200Hp_KEIHIN_37820-R40-A3X_SH7058_1Mb_37805-R40-A340_37805-R40-A330_37805-R40-A320_37805-R40-A310.xdf` | **2010** | 5.0 KB | `212b05816de64cc56eaf79dfa9cb0e74` | TunerPro Binary Definition Map |
| `37805-R40-A590_Honda_Accord_2012_LX_2.4L__L4_-_Gas.xdf` | **2012** | 4.9 KB | `2696c57ff5c17001ce200c1da4a05426` | TunerPro Binary Definition Map |
| `37805-R40-A730_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | **2008–2009** | 4.9 KB | `d8c04dd9cd5537f76d56dd1c8b3456c9` | TunerPro Binary Definition Map |
| `37805-R40-A830_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas.xdf` | **2010** | 4.9 KB | `cda6fc28b2df9d2c1901becce9958606` | TunerPro Binary Definition Map |
| `37805-R40-K030_Honda_Accord_2011_2012_LX__LX-P__SE_LX_2.4L__L4_-_Gas.xdf` | **2011–2012** | 4.9 KB | `c0539a39ea2f7fb497dd512b884f7e71` | TunerPro Binary Definition Map |
| `37805-R41-L590_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | **1992–2017** | 4.9 KB | `ed4832833006c4ef0f5e7d708e406b43` | TunerPro Binary Definition Map |
| `37805-R41-L630_Honda_Accord_2008_2009_LX__LX-P_2.4L__L4_-_Gas.xdf` | **2008–2009** | 4.9 KB | `120694395f8ff55b55233b8690a413d8` | TunerPro Binary Definition Map |
| `37805-R41-L730_Honda_Accord_2010_LX__LX-P_2.4L__L4_-_Gas.xdf` | **2010** | 4.9 KB | `2ed72b7f7c8af959bc1d5afa06bc7bdd` | TunerPro Binary Definition Map |
| `37805-R42-A090_Honda_Accord_2012_LX__LX-P__SE_2.4L__L4_-_Gas___ECU_Honda_Ac.xdf` | **2012** | 5.1 KB | `f7de58cdd1eff48b7f77d510f08391e9` | TunerPro Binary Definition Map |
| `37805-R42-A090_Honda_Accord_2012_LX__LX-P__SE_2.4L__L4_-_Gas___ECU_Honda_Accord_2.4_16v_200Hp_KEIHIN_37820-R42-A0X_SH7058_1Mb_37805-R42-A090_37805-R42-A080_37805-R42-A070_37805-R42-A060_37805-R42-A050_37805-R42-A040_37805-R42-A030_37805-R42-A020.xdf` | **2012** | 5.1 KB | `f7de58cdd1eff48b7f77d510f08391e9` | TunerPro Binary Definition Map |
| `37805-R42-A140_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | **2008–2009** | 5.0 KB | `ebb8e24c63aa9910e2a7ed6f1992ea42` | TunerPro Binary Definition Map |
| `37805-R42-A140_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | **2008–2009** | 5.0 KB | `ebb8e24c63aa9910e2a7ed6f1992ea42` | TunerPro Binary Definition Map |
| `37805-R42-A240_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | **2010** | 4.9 KB | `8953af00c7bd9794869fe48840f5e5de` | TunerPro Binary Definition Map |
| `37805-R42-A240_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | **2010** | 4.9 KB | `8953af00c7bd9794869fe48840f5e5de` | TunerPro Binary Definition Map |
| `37805-R42-A590_Honda_Accord_2012_EX__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | **2012** | 4.9 KB | `0fe55e5685f5da94b5fdecbb472b620f` | TunerPro Binary Definition Map |
| `37805-R42-A630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | **2008–2009** | 5.0 KB | `fe053f8ef3e511b2d02f323795ed50ad` | TunerPro Binary Definition Map |
| `37805-R42-A630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | **2008–2009** | 5.0 KB | `fe053f8ef3e511b2d02f323795ed50ad` | TunerPro Binary Definition Map |
| `37805-R42-A730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | **2010** | 4.9 KB | `ae762a9f968727a9f7f7814d8f7c5853` | TunerPro Binary Definition Map |
| `37805-R42-A730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_Gas.xdf` | **2010** | 4.9 KB | `ae762a9f968727a9f7f7814d8f7c5853` | TunerPro Binary Definition Map |
| `37805-R43-L590_Honda_Accord_2012_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | **2012** | 5.1 KB | `38a61842733f2ead15e8f3e30982065f` | TunerPro Binary Definition Map |
| `37805-R43-L630_Honda_Accord_2008_2009_EX__EX-L__LX-S_EX__EX-L__LX_2.4L__L4_.xdf` | **2008–2009** | 5.0 KB | `f7a2facef00fcad9be2aad5472b80dbe` | TunerPro Binary Definition Map |
| `37805-R43-L730_Honda_Accord_2010_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | **2010** | 4.9 KB | `e04b325df52a1eedc1b9d4466cc8f08f` | TunerPro Binary Definition Map |
| `37805-R44-X630_Honda_Accord_2012_EX__EX-L__LX-S_2.4L__L4_-_Gas__3.5L__V6_-_.xdf` | **2012** | 5.0 KB | `0a0625428d29a68df435525681a0ccd1` | TunerPro Binary Definition Map |
| `37805-R46-X630_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | **1992–2017** | 4.9 KB | `7777ddfb046f17ea5395f19e4ffe6a84` | TunerPro Binary Definition Map |
| `37805-R60-M540_Honda_Accord_2.4_16v_SH7058_1Mb.xdf` | **1992–2017** | 3.8 KB | `595a4f054526c8509de4b0473ce84428` | TunerPro Binary Definition Map |
| `37805-RCA-A250_Honda_Accord_2003_EX_3.0L__V6_-_Gas.xdf` | **2003** | 4.4 KB | `3fbd026bbb0ee4ce74d8851bb3610c48` | TunerPro Binary Definition Map |
| `37805-RCA-A470_Honda_Accord_2007_EX_3.0L__V6_-_Gas.xdf` | **2007** | 4.4 KB | `cac716931c5553942b2ca0f9e63678d4` | TunerPro Binary Definition Map |
| `37805-RCA-A750_Honda_Accord_2005_EX_3.0L__V6_-_Gas.xdf` | **2005** | 4.4 KB | `09e5fd993789118dec6d184930414506` | TunerPro Binary Definition Map |
| `37805-RCA-L470_Honda_Accord_2006_2007_EX_3.0L__V6_-_Gas.xdf` | **2006–2007** | 4.4 KB | `2f96725c54a57e47329ce393fa967015` | TunerPro Binary Definition Map |
| `37805-RCA-L750_Honda_Accord_2005_EX_3.0L__V6_-_Gas.xdf` | **2005** | 4.4 KB | `093658c93c06c70059423b0045101b1b` | TunerPro Binary Definition Map |
| `37805-RCA-M550_Honda_Accord_2005_EX__LX__SE_3.0L__V6_-_Gas.xdf` | **2005** | 4.4 KB | `e4959e08c3b1536e739d0d3599a13fc4` | TunerPro Binary Definition Map |
| `37820-P11-G00.bin` | **1992–2017** | 32.0 KB | `12431f916cb60a1a11e4bed842c032a2` | Factory Binary Firmware Dump |
| `37820-P13-Q00.bin` | **1992–2017** | 32.0 KB | `10e3b40b1c35cc5892b2c5daf30086a3` | Factory Binary Firmware Dump |
| `HONDA_ACCORD_CR2_2013-2017_2.4L_K24W_EARTH_DREAMS_KEIHIN_37805-5A0-X920-M1.rwd` | **2013–2017** | 1.94 MB | `2fe5720f96ff8d3e0a6c95981d04176d` | Factory Binary Firmware Dump |
| `P13-G00-C3.bin` | **1992–2017** | 32.0 KB | `dd2ab0cbce8b917e36b95cdecaba9bd3` | Factory Binary Firmware Dump |
| `P13-N01-E6.bin` | **1992–2017** | 32.0 KB | `0616d775ed0f05abc0c89926bb6be62d` | Factory Binary Firmware Dump |
| `P13.JDM.Prelude.BIN` | **1992–2017** | 32.0 KB | `eeb76d7f481a10fa0b41c5db63b4dec1` | Factory Binary Firmware Dump |
| `P13OEMJ50AT.bin` | **1992–2017** | 32.0 KB | `4280cfe9efa8f48f4d14cf00aecf0556` | Factory Binary Firmware Dump |
| `P14-A11_stock.bin` | **1992–2017** | 32.0 KB | `edab280f82e9b0c13bcec3811f7dd7a5` | Factory Binary Firmware Dump |
| `PH3-0732-88-89-Accord.bin` | **1992–2017** | 32.0 KB | `0afc6b335298abe6fb3afb946112ad78` | Factory Binary Firmware Dump |
| `PT3_A54.BIN` | **1992–2017** | 32.0 KB | `934bf62d67c0edae9010aebd9eac1c02` | Factory Binary Firmware Dump |
| `p12-a00.bin` | **1992–2017** | 32.0 KB | `ce6733dda695f826457098a5dc352ae6` | Factory Binary Firmware Dump |
| `p12-a00.rom` | **1992–2017** | 32.0 KB | `d22fc62dc86320f0e6b63bb6df437b55` | Factory Binary Firmware Dump |
| `p14-q00-c0.bin` | **1992–2017** | 32.0 KB | `60b68e94957775ec5a48894ed31f966b` | Factory Binary Firmware Dump |
| `p14-q52-e4.bin` | **1992–2017** | 32.0 KB | `846df3c0def3e4fd97f729f7be7d2527` | Factory Binary Firmware Dump |
| `p14.bin` | **1992–2017** | 32.0 KB | `5cbf7ab6b4a2f567e3c06304d794d493` | Factory Binary Firmware Dump |
| `pt3-q50-83.bin` | **1992–2017** | 32.0 KB | `13be07dcae2c9ecfaa7e029db5dfb81d` | Factory Binary Firmware Dump |
| `pt6-j50-d2.bin` | **1992–2017** | 32.0 KB | `91c39cdebd673e5292a44cddd0dd852e` | Factory Binary Firmware Dump |
| `pt6-q50-97.rom` | **1992–2017** | 32.0 KB | `88ebb79ca253654084892734b2598547` | Factory Binary Firmware Dump |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
