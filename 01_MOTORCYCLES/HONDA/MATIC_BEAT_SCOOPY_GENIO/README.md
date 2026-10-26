# HONDA MATIC BEAT SCOOPY GENIO SPACY - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/MATIC_BEAT_SCOOPY_GENIO`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `99 files` (6 binary/calibration dumps, 93 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `MATIC_BEAT_SCOOPY_GENIO` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda 110cc PGM-FI Matic Fleet (Beat FI/eSP, Scoopy FI/eSP, Genio, Spacy FI, Zoomer X) Keihin/Shindengen ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

* **Rentang Tahun / Model Year**: 2012–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `GENERATIONAL_30400-K1A-N01_Honda_All_New_Beat_LED_Gen_4_Smart_Key___Alarm_(2024-2026).xdf` | **2024–2026** | 5.5 KB | `3d797f52e1dda89237a6099e28114f52` | TunerPro Binary Definition Map |
| `GENERATIONAL_30400-K2F-N11_Honda_All_New_Scoopy_Gen_4_Facelift_(2024-2026).xdf` | **2024–2026** | 5.5 KB | `9863856d9db5e54589d9fd1439a8aca5` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K93-N01_Honda_Scoopy_Ring_12_eSP_Gen_2_(2017-2020).xdf` | **2017–2020** | 5.4 KB | `00b9ead743264432ecda5a1cd50820e3` | TunerPro Binary Definition Map |
| `HONDA_30400-K0J-N01_Honda_Generic_ECM.xdf` | **2019–2024** | 16.3 KB | `2bcb790fa3dbaa1154900f365d4421c7` | TunerPro Binary Definition Map |
| `HONDA_30400-K20J-T21_Zoomer-X_2015-2017_Zoomer-X_(2015-2020).xdf` | **2015–2017** | 9.9 KB | `694c940ad507ddafd323cfadc35fe956` | TunerPro Binary Definition Map |
| `HONDA_30400-K2F-N11_Scoopy-i_(2021-2024).xdf` | **2021–2024** | 16.3 KB | `575b3de110d0661def867ec83efae373` | TunerPro Binary Definition Map |
| `HONDA_30400-K2SF-T01_CLICK160_Scoopy-i_(2013-2016).xdf` | **2013–2016** | 9.9 KB | `b60e94b86c52a9631118b97fa269d97c` | TunerPro Binary Definition Map |
| `HONDA_30400-K2TA-T02_LEAD125_4V_Lead_125_4V_(2022-2024).xdf` | **2022–2024** | 9.9 KB | `b107652d6ef0a42edbac4bf0d158b0c8` | TunerPro Binary Definition Map |
| `HONDA_30400-K3MF-T01_GIONRO_125_Giorno+_125_(2023-2024).xdf` | **2023–2024** | 9.9 KB | `7e16e57fe25b19c8be6a677ecb2a5c63` | TunerPro Binary Definition Map |
| `HONDA_30400-K93-N01_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `34b5c5ba9e76676764d23a132c485f79` | TunerPro Binary Definition Map |
| `HONDA_30400-K93-T01_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `de66b0bbe85c87ef6611fb5ed3b42ae5` | TunerPro Binary Definition Map |
| `HONDA_38770-G90-V02_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `6b1ce979094b58061112020e048cbdcd` | TunerPro Binary Definition Map |
| `HONDA_38770-GFM-601_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `32c7939345dee87ea567c67cb459a6a0` | TunerPro Binary Definition Map |
| `HONDA_38770-GGE-901_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `a8cc719388c87d646ee539eaaaf86cb8` | TunerPro Binary Definition Map |
| `HONDA_38770-GGE-941_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `efcc7b825fb5d934b26622f2b7d2f080` | TunerPro Binary Definition Map |
| `HONDA_38770-HL6-A05_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `e6846bed35139efb003d185e728ec44c` | TunerPro Binary Definition Map |
| `HONDA_38770-HR6-MO2_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `5ea536da247444bfb07b5ad1615b7cb4` | TunerPro Binary Definition Map |
| `HONDA_38770-K25-901_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `e9163da50566710455b80c2f397e880c` | TunerPro Binary Definition Map |
| `HONDA_38770-K28-A62_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `8a3e68bde9c68a1c599d2a91e607767a` | TunerPro Binary Definition Map |
| `HONDA_38770-K2F-N01_Scoopy-i_(2021-2024).xdf` | **2021–2024** | 16.3 KB | `82f2e995ed7e4751a248363310ca0b34` | TunerPro Binary Definition Map |
| `HONDA_38770-K47-M01_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `90bd6bd17222805d0f447a793d903cf0` | TunerPro Binary Definition Map |
| `HONDA_38770-K53-D03_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `00d6f131cfbaebe362a54ae37c1912b5` | TunerPro Binary Definition Map |
| `HONDA_38770-K53-DB2_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `f1b68ae3c67f8168c6c5267ee1665327` | TunerPro Binary Definition Map |
| `HONDA_38770-K76-M02_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `2f8c2ea2ea5e53efaa0c3e22ed7b1847` | TunerPro Binary Definition Map |
| `HONDA_38770-K76-T62_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `a515b91eba895fea400ebf5b15d20d05` | TunerPro Binary Definition Map |
| `HONDA_38770-K87-T52_Rebel_300_(2017-2024).xdf` | **2017–2024** | 16.3 KB | `a6368718feb2aeeca3919dac48090fd0` | TunerPro Binary Definition Map |
| `HONDA_38770-K95-A41_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `605a2c17c0ffbe53e32673bd32615687` | TunerPro Binary Definition Map |
| `HONDA_38770-K99-B02_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `49b912cf06953062c5395e9f462e03a4` | TunerPro Binary Definition Map |
| `HONDA_38770-KOA-T11_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `bd8dfa75472aca13e540edc2cad519f0` | TunerPro Binary Definition Map |
| `HONDA_38770-KPG-H01_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `273f5f5fc47a3cd8a5e082e2eac5cdbc` | TunerPro Binary Definition Map |
| `HONDA_38770-KTW-903_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `ba713d3f17fd41b54cc8ae33b5b9dc05` | TunerPro Binary Definition Map |
| `HONDA_38770-KTW-B02_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `04eced5e18f77e8f935bc01604f70075` | TunerPro Binary Definition Map |
| `HONDA_38770-KTY-H52_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `cdb5ccfe582f27a45c195dfcf941d69d` | TunerPro Binary Definition Map |
| `HONDA_38770-KVK-B31_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `f74cc599da0b6de445e74a9a72f70a25` | TunerPro Binary Definition Map |
| `HONDA_38770-KWT-703_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `aad7d66360b306cbac155d9a54f2e311` | TunerPro Binary Definition Map |
| `HONDA_38770-KYE-942_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `e8e16e8d88130503c53f3e7ad8dc65be` | TunerPro Binary Definition Map |
| `HONDA_38770-KYJ-922_CBR250R_(2011-2014).xdf` | **2011–2014** | 16.3 KB | `f8d2deb279e8e6777f097e7381f02a03` | TunerPro Binary Definition Map |
| `HONDA_38770-KYJ-971_CBR250R_(2011-2014).xdf` | **2011–2014** | 16.3 KB | `80e616cdec66df3f957529b561750270` | TunerPro Binary Definition Map |
| `HONDA_38770-KYJ-R11_CBR250R_(2011-2014).xdf` | **2011–2014** | 16.3 KB | `93d57c55e038693046e7b1a9d52b8a8a` | TunerPro Binary Definition Map |
| `HONDA_38770-KZL-C31_Spacy-i___Zoomer-X_(2012-2014).xdf` | **2012–2014** | 16.3 KB | `9737a16174d77172c0e6ef57a847e7e8` | TunerPro Binary Definition Map |
| `HONDA_38770-KZL-E12_Spacy-i___Zoomer-X_(2012-2014).xdf` | **2012–2014** | 16.3 KB | `693f6f3b4b92b2a747e76d8848e74098` | TunerPro Binary Definition Map |
| `HONDA_38770-MCG-602_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `34b7b3fc9c9d2d5b5ac21b594dbec0a6` | TunerPro Binary Definition Map |
| `HONDA_38770-MEW-D41_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `1156062687174d995ca812eb77b9b9c6` | TunerPro Binary Definition Map |
| `HONDA_38770-MFA-D03_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `551192253411d471adeffb5e95eb7fd1` | TunerPro Binary Definition Map |
| `HONDA_38770-MFG-D02_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `bd9f026a55999e152ab44a5875a7a7a2` | TunerPro Binary Definition Map |
| `HONDA_38770-MFM-651_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `2cb45c8ae3fe48450e52f687cd32ca72` | TunerPro Binary Definition Map |
| `HONDA_38770-MFM-702_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `0cac77b1f41f101fcc7f0ea146a873d7` | TunerPro Binary Definition Map |
| `HONDA_38770-MFN-D01_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `6ecd74183524581c4e0f46db01cc813a` | TunerPro Binary Definition Map |
| `HONDA_38770-MFN-F01_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `e98d5b429de491a9e2a0eb332c759757` | TunerPro Binary Definition Map |
| `HONDA_38770-MFR-642_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `9d1001ad437921986d651a58739dbf3b` | TunerPro Binary Definition Map |
| `HONDA_38770-MFT-642_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `7c07370364ab336ad398aedae4819b9d` | TunerPro Binary Definition Map |
| `HONDA_38770-MGC-D32_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `254bc1b4c9a8a20cc8d3409dce75f542` | TunerPro Binary Definition Map |
| `HONDA_38770-MGE-623_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `98fd891ac631b618c5f253b8569c379f` | TunerPro Binary Definition Map |
| `HONDA_38770-MGE-D01_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `15b9a259b320073d0630a88926ea792a` | TunerPro Binary Definition Map |
| `HONDA_38770-MGE-D02_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `e9185936034418255be82c827fd8cd60` | TunerPro Binary Definition Map |
| `HONDA_38770-MGE-D41_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `cf885e2d480547f351254cb55c34f8a8` | TunerPro Binary Definition Map |
| `HONDA_38770-MGE-F02_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `f7392c9ba6df778aab5f2c215d8763e9` | TunerPro Binary Definition Map |
| `HONDA_38770-MGE-F11_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `e897c22ca12183ca5d7bc508de244d8f` | TunerPro Binary Definition Map |
| `HONDA_38770-MGF-D12_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `f8c1d47e1a54ab0a299933a4ece662a9` | TunerPro Binary Definition Map |
| `HONDA_38770-MGH-641_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `16058330c98af612d59c70ce52393a30` | TunerPro Binary Definition Map |
| `HONDA_38770-MGH-D21_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `13e5561fceea4dd2fee1ec49dcae999e` | TunerPro Binary Definition Map |
| `HONDA_38770-MGH-F21_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `42930eb77dbddb30dd25c8170344624f` | TunerPro Binary Definition Map |
| `HONDA_38770-MGH-M12_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `b3ce4e1294a203869fb5341a01ff313f` | TunerPro Binary Definition Map |
| `HONDA_38770-MGH-N12_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `01095622236de325048c9e6baf9d68ca` | TunerPro Binary Definition Map |
| `HONDA_38770-MGM-D11_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `a471a667fba68b253bc010600bfde3ef` | TunerPro Binary Definition Map |
| `HONDA_38770-MJL-Y11_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `bd206d28a33af78e565595e88d0925d4` | TunerPro Binary Definition Map |
| `HONDA_38770-MJP-DA1_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `a8e0ae2ca46b43581b6266dbc11fba96` | TunerPro Binary Definition Map |
| `HONDA_38770-MKA-D71_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `b0b8d252fb9207c956fe31f4493f75bc` | TunerPro Binary Definition Map |
| `HONDA_38770-MKG-N52_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `330b1775688867f6c0478c9f6d551b78` | TunerPro Binary Definition Map |
| `HONDA_38770-MKJ-D02_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `a9c2742a05e680a60a99426d7ca9bb88` | TunerPro Binary Definition Map |
| `HONDA_38770-N1A-D00_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `7a1aa851b4aab2ae7ef520dda46680a5` | TunerPro Binary Definition Map |
| `HONDA_38770-N1A-D11_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `12c473f70ccfcba70fd6a4a6ee5dafd3` | TunerPro Binary Definition Map |
| `HONDA_38770-NLR-B31_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `3c9fa82f5566bce579fa1ac03879a04f` | TunerPro Binary Definition Map |
| `HONDA_38770-NLS-000_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `3094f144129e88c3eea8d71f823bbc60` | TunerPro Binary Definition Map |
| `HONDA_SCOOPY_I_38770_K16_B01_48KB_ORI.bin` | **2012–2024** | 48.0 KB | `20bff8176d6dd0a0453ce5b6abbabc1b` | Factory Binary Firmware Dump |
| `HONDA_SCOOPY_I_K16_901_48KB_ORI.bin` | **2012–2024** | 48.0 KB | `762b842e5f4105bea1461f27c80b1c4c` | Factory Binary Firmware Dump |
| `HONDA_SCOOPY_I_K16_B61_64KB_ORI.bin` | **2012–2024** | 64.0 KB | `54c5c6bd2951704720af9a8eedc84fd4` | Factory Binary Firmware Dump |
| `HONDA_SCOOPY_I_K16_H01_48KB_ORI.bin` | **2012–2024** | 48.0 KB | `20bff8176d6dd0a0453ce5b6abbabc1b` | Factory Binary Firmware Dump |
| `HONDA_SPACY_BEAT_FI_KZL_C03_48KB_ORI.bin` | **2012–2024** | 48.0 KB | `980c96240d2d64e53371285cc772ae46` | Factory Binary Firmware Dump |
| `HONDA_ZOOMER_X_BEAT_ESP_K20_T01_64KB_ORI.bin` | **2012–2024** | 64.0 KB | `e7d8baa1fc333dcd47bd6d8cce2a0ea1` | Factory Binary Firmware Dump |
| `Honda_38770-K0J-N01_Genio_256KB.xdf` | **2019–2024** | 8.6 KB | `f77215112fed7b0d3004d839b51efb67` | TunerPro Binary Definition Map |
| `Honda_38770-K0W-N01_ADV_256KB.xdf` | **2019–2022** | 8.6 KB | `489f1940c66b696a7ddf64dbf87a06fd` | TunerPro Binary Definition Map |
| `Honda_38770-K15-903_CB150R_64KB.xdf` | **2012–2018** | 7.8 KB | `a19efec5dc03556d85c1175112f91074` | TunerPro Binary Definition Map |
| `Honda_38770-K15-921_All_256KB.xdf` | **2012–2018** | 8.6 KB | `2e71ebf1790efe962e141bc2bdcd319f` | TunerPro Binary Definition Map |
| `Honda_38770-K16-901_Scoopy_64KB.xdf` | **2012–2024** | 7.8 KB | `0b26ab50691293a80c7bf6b164fdd300` | TunerPro Binary Definition Map |
| `Honda_38770-K1Z-N01_PCX_256KB.xdf` | **2021–2026** | 8.6 KB | `7c1de29786d3582ebb3209b7be56b1e8` | TunerPro Binary Definition Map |
| `Honda_38770-K1Z-N21_PCX_256KB.xdf` | **2021–2026** | 8.6 KB | `c09f390197cbb07be2cfbd9489bfac5a` | TunerPro Binary Definition Map |
| `Honda_38770-K20-901_Spacy_64KB.xdf` | **2012–2024** | 7.8 KB | `bf76d8587ff132f13cbb6d4e3dd6ebd8` | TunerPro Binary Definition Map |
| `Honda_38770-K25-601_Beat_64KB.xdf` | **2012–2024** | 7.8 KB | `82060ba73ed2d9bdef867f992ccff205` | TunerPro Binary Definition Map |
| `Honda_38770-K25-901_Beat_64KB.xdf` | **2012–2024** | 7.8 KB | `d3ee65f54c68a0b0e17c5c22691f942a` | TunerPro Binary Definition Map |
| `Honda_38770-K2F-N01_All_256KB.xdf` | **2012–2024** | 8.6 KB | `feae7628eeeb4d794e9d88f825503ede` | TunerPro Binary Definition Map |
| `Honda_38770-K41-N01_Blade_64KB.xdf` | **2012–2024** | 7.8 KB | `b89844e9011476ed2830d03cc0378c07` | TunerPro Binary Definition Map |
| `Honda_38770-K44-V01_Beat_64KB.xdf` | **2012–2024** | 7.8 KB | `ebab528018d00431d2c384a6b3545100` | TunerPro Binary Definition Map |
| `Honda_38770-K46-N01_Vario_64KB.xdf` | **2012–2024** | 7.8 KB | `893bf743d1b3c7909cf9ead2c2dcc2b1` | TunerPro Binary Definition Map |
| `Honda_38770-K56-N01_Sonic_256KB.xdf` | **2015–2024** | 8.6 KB | `8981d79fd3f4269aa3601a659d17bcde` | TunerPro Binary Definition Map |
| `Honda_38770-K59-A11_Vario_256KB.xdf` | **2015–2021** | 8.6 KB | `2e577b870e9707d97670ce731b48566a` | TunerPro Binary Definition Map |
| `Honda_38770-K60-B11_Vario_256KB.xdf` | **2015–2024** | 8.6 KB | `3d68e853b1daa4fdaeb1ba3393eb5dd3` | TunerPro Binary Definition Map |
| `Honda_38770-K97-N01_PCX_256KB.xdf` | **2012–2024** | 8.6 KB | `19f77f3ac16416d0082a13710567e9f3` | TunerPro Binary Definition Map |
| `Honda_38770-KVG-V42_Vario_64KB.xdf` | **2012–2024** | 7.8 KB | `3554b4dd1bc6a57faf7e2a71dab99520` | TunerPro Binary Definition Map |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
