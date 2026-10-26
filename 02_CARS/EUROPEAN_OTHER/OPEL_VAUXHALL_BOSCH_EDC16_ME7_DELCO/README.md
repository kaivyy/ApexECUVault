# OPEL & VAUXHALL - Bosch EDC16, Motronic ME7.6 & Delco Multec Suite

**Repository Path**: `02_CARS/EUROPEAN_OTHER/OPEL_VAUXHALL_BOSCH_EDC16_ME7_DELCO`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `116 files` (116 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Koleksi 116 berkas biner hardware dumps (.ori/.bin) untuk kendaraan Opel dan Vauxhall (Astra G/H, Corsa C/D, Vectra B/C, Zafira A/B, Meriva, Insignia, Frontera) dengan mesin 1.3 CDTI, 1.7 CDTI/DTI, 1.9 CDTI, 2.0 DTI, serta varian bensin 1.6/1.8/2.0 Turbo (Z20LET/LEH). Pengontrol Bosch EDC16C39 pada Opel 1.9 CDTI (Z19DTH) adalah varian platform bersama General Motors yang identik dengan arsitektur ECU Fiat JTDm dan Saab TiD.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Bosch EDC15M, EDC16C9, EDC16C39, Motronic ME7.6.2, Siemens Simtec, Delco Multec`
- **Arsitektur MCU & Memori**: `Infineon ST10 / Motorola MPC555 / MPC562 / MPC564 512KB-2MB Flash`
- **Protokol Diagnostik & Flashing**: `K-Line (ISO 14230 KWP2000) / CAN-Bus (GMLAN / ISO 15765) / BDM100`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`, `0110C6`, `MS430069`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`, `32920-xxxxx`): Nomor resmi Denso MCU firmware flash untuk mobil dan motor.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx-xxxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **VAG Hardware / Software IDs** (misal `038906012xx`, `03G906021xx`, `8D0907558xx`): Nomor bagian resmi Volkswagen Audi Group untuk identifikasi kalibrasi mesin EDC15, EDC16, dan ME7.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: OEM Production

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `0-281-001-793_Opel_Frontera_22DTi_HHH.16B.bin` | **OEM Production** | 256.0 KB | `e2c0be59314a51179dff43cb71906d63` | Factory Binary Firmware Dump |
| `0-281-010-026_Opel_Frontera_22DTi.ori` | **OEM Production** | 256.0 KB | `cc64bed7b2b4c622ac5ea546928f49fc` | Factory Binary Firmware Dump |
| `0-281-010-448_Opel_Frontera_2.2DTi.ori` | **OEM Production** | 256.0 KB | `0f3183243347facad69bd5d71ede132b` | Factory Binary Firmware Dump |
| `001632h.ori.bin` | **OEM Production** | 128.0 KB | `54a8bbc1d8e1e9e2377855d4da190c1a` | Factory Binary Firmware Dump |
| `001632l.ori.bin` | **OEM Production** | 128.0 KB | `36adfe1099e0ed9baa982c84454e2de3` | Factory Binary Firmware Dump |
| `0281001214 2537355342 .Ori` | **OEM Production** | 32.0 KB | `f3b76d7d46f7ccf660ef960d5bfd7fcf` | Factory Binary Firmware Dump |
| `0281001214 2537355394 .Ori` | **OEM Production** | 32.0 KB | `aa5d0af1011366860aa1d1a079dbaa18` | Factory Binary Firmware Dump |
| `0281001634 051 LLL.ori` | **OEM Production** | 128.0 KB | `067ff396b20c36be626044a4634b30a1` | Factory Binary Firmware Dump |
| `0281001634 052 HHH.ori` | **OEM Production** | 128.0 KB | `e4ab97dc0d8c081a1f77f1a6ce0c40bc` | Factory Binary Firmware Dump |
| `0281010267- B585300016ABB HHH.ori` | **OEM Production** | 128.0 KB | `b97efdf54c8d69d8b585c33ff9055fbf` | Factory Binary Firmware Dump |
| `0281010267- B585300016ABB LLL.ori` | **OEM Production** | 128.0 KB | `4ee80cb792b7b48670134974cda7e87c` | Factory Binary Firmware Dump |
| `0281013409_1037A50286_Vectra_CDTI_120PS.bin` | **OEM Production** | 1.00 MB | `155e5c800c6eac2bcec999a42e5f7aac` | Factory Binary Firmware Dump |
| `1.7 CDTI 0281011380-1037370433.ORI` | **OEM Production** | 1.00 MB | `35e0848136eb646dba67ce4a1774f416` | Factory Binary Firmware Dump |
| `1.7 CDTI 0281011380-1037374424.ori` | **OEM Production** | 1.00 MB | `1094c74e3a9c38248670c9b827099154` | Factory Binary Firmware Dump |
| `1.7 CDTI 0281011943-1037372298.BIN` | **OEM Production** | 1.00 MB | `1e26adfdab1f63d00e9d61f814cac087` | Factory Binary Firmware Dump |
| `1.7 CDTI 0281011943-1037374425.ORI` | **OEM Production** | 1.00 MB | `6ef3c423d368bb165ee54a0a7699982d` | Factory Binary Firmware Dump |
| `1.7 CDTI 0281012694-1037376412.ori` | **OEM Production** | 1.00 MB | `ed79dbb80d633ecbfd82d772f4b46861` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281011448-1037370816.ori` | **OEM Production** | 1.00 MB | `45f60be7c99bfb6c9306163bce77976d` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281011449-1037372385.ori` | **OEM Production** | 1.00 MB | `8f718b538d2038475c69863446a61b87` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281011449-1037379356.ORI` | **OEM Production** | 1.00 MB | `3783182df0f8ced1152140ffb28af7b9` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281011667-1037379413.ori` | **OEM Production** | 1.00 MB | `591f111f7ee00746ba05d32baa17711b` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281011914-1037371351.ORI` | **OEM Production** | 1.00 MB | `ed54451cddb59cb3b10b1e4e038f9393` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281011914-1037372745.ORI` | **OEM Production** | 1.00 MB | `a363b794430b9b579661538d0da82e2d` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281011914-1037379357.ORI` | **OEM Production** | 1.00 MB | `8025a6ac0a8185ec6c7fbc7ed4aa117e` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281011915-1037372742.ori` | **OEM Production** | 1.00 MB | `9d95bf7e40fbf95075f2a9b3e78a03bb` | Factory Binary Firmware Dump |
| `1.9 CDTI 0281012533-1037379019.ori` | **OEM Production** | 1.00 MB | `f979678b7747cf606c021c1a4c97f910` | Factory Binary Firmware Dump |
| `90569370.bin` | **OEM Production** | 112.0 KB | `5f29ac91a24e09d56d43648f63beb6c1` | Factory Binary Firmware Dump |
| `ASTRA CDTI 1,9-0281012122-1037371870.bin` | **OEM Production** | 1.00 MB | `e1609c95f3614ddfa0201eb26af35c08` | Factory Binary Firmware Dump |
| `Astra 1.9 CDTI 150HP 0281011667 371868.ori` | **OEM Production** | 1.00 MB | `25d14772a865591b8316d7f6e1eeb7ae` | Factory Binary Firmware Dump |
| `Astra 2.0 16V GSi 0261200487 357099.ori` | **OEM Production** | 32.0 KB | `21d78b327c5a90593b39ae4d61312394` | Factory Binary Firmware Dump |
| `Bosch_EDC16_OPEL_0281012549_1037379426.ori` | **OEM Production** | 1.00 MB | `f4dff2d6a13d263c0e1e903afcc04c41` | Factory Binary Firmware Dump |
| `Cosa D_0261208940_1037381910 ori.bin` | **OEM Production** | 832.0 KB | `2aba6078e856e21a2f96543f5625edb2` | Factory Binary Firmware Dump |
| `DTI-SHH.873.bin` | **OEM Production** | 128.0 KB | `5a9a2da797c3ca69114dba9be15179b4` | Factory Binary Firmware Dump |
| `DTI-SLL.873.bin` | **OEM Production** | 128.0 KB | `3a22c6ff0ea784f85ca8dc3517a6f81e` | Factory Binary Firmware Dump |
| `F22-SHH.023.bin` | **OEM Production** | 128.0 KB | `09b42c5c18ddd8108a10d2e123cf2f83` | Factory Binary Firmware Dump |
| `F22-SLL.023.bin` | **OEM Production** | 128.0 KB | `279acb369b37e033da3834f720f91dd6` | Factory Binary Firmware Dump |
| `OPEL 1.9 CDTI EDC16+ 0281013567-1037380490.ori` | **OEM Production** | 2.00 MB | `cd65602bc6e9c439521dcd8a97718280` | Factory Binary Firmware Dump |
| `OPEL ASTRA 1.9 CDTI 0281013409-1037383690.ori` | **OEM Production** | 1.00 MB | `600dc4fb6bc6f9fde1d6c9ff4e7b321e` | Factory Binary Firmware Dump |
| `OPEL ASTRA 1.9 CDTI 0281014025-383480.ori` | **OEM Production** | 2.00 MB | `39279f33c700ca1bd76b4a05153c8c48` | Factory Binary Firmware Dump |
| `OPEL ASTRA 1.9 CDTI-0281013409-1037379432.ori` | **OEM Production** | 1.00 MB | `9baefb9cd5aa5bb8a09bd775cef56aa9` | Factory Binary Firmware Dump |
| `OPEL ASTRA CDTI 1,9-0281012548-379085.bin` | **OEM Production** | 1.00 MB | `47fbfdab560b5f0a9397802c17ffdc38` | Factory Binary Firmware Dump |
| `Opel 1.9 CDTi 150bhp - 0281014451 - 1037387386.ori` | **OEM Production** | 2.00 MB | `b339de51f8a658929083f40a680076fd` | Factory Binary Firmware Dump |
| `Opel 1.9CDTI 0281012548 378432.ori` | **OEM Production** | 1.00 MB | `eeb44ec0ec5fca6c5ee4c28bd3896baf` | Factory Binary Firmware Dump |
| `Opel 1.9CDTI 150HP 0281011915 379081.ori` | **OEM Production** | 1.00 MB | `731c53cf9a8b70ffcbb73ad19408ce1d` | Factory Binary Firmware Dump |
| `Opel Astra 2.0 16v (C20XE) 0261203017 357369.ori` | **OEM Production** | 64.0 KB | `db7ac64a50fa28a7859eebd034ac3f54` | Factory Binary Firmware Dump |
| `Opel Astra-G 1.6 16V 75HP 16227049 D98003 CNHR.ori` | **OEM Production** | 128.0 KB | `bffd6d40c2328cea73e8231b75f11734` | Factory Binary Firmware Dump |
| `Opel Frontera 2.2DTI_0281010023 VU2M2S30.ori` | **OEM Production** | 256.0 KB | `2eea2b5d8d56cc3638cf6fb983990b62` | Factory Binary Firmware Dump |
| `Opel Monvano 2.5DCI  0281011432 368929.ori` | **OEM Production** | 512.0 KB | `ccc195ca83c824f0510e2f402291ced3` | Factory Binary Firmware Dump |
| `Opel Vectra 1.9CDTI 150HP 0281013408 379428.ori` | **OEM Production** | 1.00 MB | `6c79494b56969eaafad280d9603323e5` | Factory Binary Firmware Dump |
| `Opel Vectra B 1.8i 115HP 5WK9073 GM90506365.ori` | **OEM Production** | 128.0 KB | `9154a82ecdfe7b805d01c86baa954bce` | Factory Binary Firmware Dump |
| `Opel Vivaro 2.5 CDTI 2006 - 370878.zip.bin` | **2006** | 512.0 KB | `7b6295a96a0b462dff8d73f7225f2bf7` | Factory Binary Firmware Dump |
| `Opel Vivaro 2.5CDTI 145HP 386228.ori` | **OEM Production** | 2.00 MB | `376c4df081b58b5026ecda94b73a2715` | Factory Binary Firmware Dump |
| `Opel Zafira  1.9CDTI 120HP 0281012549 1037A50292.ori` | **OEM Production** | 1.00 MB | `983e14c7fda0b2e12dad014ed202d278` | Factory Binary Firmware Dump |
| `Opel astra 1.7CDTI 0281011943 382477.ori` | **OEM Production** | 1.00 MB | `2211b07a263427411035423adba93b3c` | Factory Binary Firmware Dump |
| `Opel astra 1.7CDTI 90HP 0281010859 367182.ori` | **OEM Production** | 512.0 KB | `3d0318d9791aa53b0d4daff48c68b3a9` | Factory Binary Firmware Dump |
| `Opel astra 1.7DTI 75HP DCWB Delco.ori` | **OEM Production** | 208.0 KB | `06898c0b6f31ace2874a93a50c2901af` | Factory Binary Firmware Dump |
| `Opel astra 1.7DTI 75HP DHCR - delco.ori` | **OEM Production** | 208.0 KB | `9f25e9fb700386aece6ffde91dc66029` | Factory Binary Firmware Dump |
| `Opel astra 1.7DTI 75HP DMRW Delco.ori` | **OEM Production** | 256.0 KB | `9aee4c93f7524239956e9d6380f6a43a` | Factory Binary Firmware Dump |
| `Opel astra 1.7DTI 75HP DYRX  Delco.ori` | **OEM Production** | 256.0 KB | `9709d04341466d4f164ab3328876b5aa` | Factory Binary Firmware Dump |
| `Opel astra 1.9 CDTI 150HP 0281012867 380280.ori` | **OEM Production** | 2.00 MB | `420a9e93c48a93542b47b5fd8af08d04` | Factory Binary Firmware Dump |
| `Opel astra 2.0 16V 0261200487 356590.ori` | **OEM Production** | 32.0 KB | `38a11c4b7829a3ff96b2b0bcc854397a` | Factory Binary Firmware Dump |
| `Opel astra 2.0DTI 100HP 0281001869 vtomw060.ori` | **OEM Production** | 192.0 KB | `2b7233ddc6ab639afbd375444b2f05a2` | Factory Binary Firmware Dump |
| `Opel astra 2.0DTI 100HP 0281001874.ori` | **OEM Production** | 256.0 KB | `73da159c468975486346f142d575959e` | Factory Binary Firmware Dump |
| `Opel astra 2.0T 193HP 0261206332 354961.ori` | **OEM Production** | 512.0 KB | `6d5e1e52d3dd46482829303daface9ab` | Factory Binary Firmware Dump |
| `Opel astra G 1.7CDTI 80HP 0281010859 367182.ori` | **OEM Production** | 512.0 KB | `bc89b77281ab4980264d40942e1a8676` | Factory Binary Firmware Dump |
| `Opel astra H 1.7CDTI 80HP 0281011943 372298.ori` | **OEM Production** | 1.00 MB | `a7555010ade33fa8b39b331a5e1bdca1` | Factory Binary Firmware Dump |
| `Opel astra H 1.9CDTI 120HP 0281012123 372342.ori` | **OEM Production** | 1.00 MB | `34dad9b03aa85ce4607a860126bdb389` | Factory Binary Firmware Dump |
| `Opel astra H 1.9CDTI 120HP 0281014025 383480.ori` | **OEM Production** | 2.00 MB | `3f839bcc8301a50b65fe35efc58c2112` | Factory Binary Firmware Dump |
| `Opel astra H 1.9CDTI 150HP 0281011668 1037372341.ori` | **OEM Production** | 1.00 MB | `945bc4fb7928b8285bbf8d89db366bb4` | Factory Binary Firmware Dump |
| `Opel astra coupe 2.0T 193HP 0261206332 360526.ori` | **OEM Production** | 512.0 KB | `d429557ebdeaffe23e04f7793fc6a008` | Factory Binary Firmware Dump |
| `Opel calibra 2.0T 204HP 0261203014 357220.ori` | **OEM Production** | 32.0 KB | `317307800cbe846f126fbb77a207b4c6` | Factory Binary Firmware Dump |
| `Opel calibra 2.5 V6 170HP 0261203080 358003.ori` | **OEM Production** | 128.0 KB | `8f1c9ef4e283cc706aacde53e5a09f80` | Factory Binary Firmware Dump |
| `Opel combo 1.7DT 100HP Z17DTH.ori` | **OEM Production** | 512.0 KB | `964dd60a6a317a5e066f707ece65e699` | Factory Binary Firmware Dump |
| `Opel corsa 1.0 12V 0261204058 (EAE6).ori` | **OEM Production** | 128.0 KB | `58c962d74e9ac715c339088f75dfd3f3` | Factory Binary Firmware Dump |
| `Opel corsa 1.2i 16V 0261207960 363893.ori` | **OEM Production** | 512.0 KB | `571801b325fd9a56743045a147e7feec` | Factory Binary Firmware Dump |
| `Opel corsa 1.2i 75HP 0261207962 370316.ori` | **OEM Production** | 512.0 KB | `5f7afe88136a2efc169d93943e96c774` | Factory Binary Firmware Dump |
| `Opel corsa 1.3CDTI 01246JO01D 1320X375.ori` | **OEM Production** | 452.0 KB | `2905b501a59391cd388942cc0269e64a` | Factory Binary Firmware Dump |
| `Opel corsa 1.4 16v 16214239 JS D96017 BWJN.ori` | **OEM Production** | 128.0 KB | `ad76efc952976a5a205ba6de4ad1ac4f` | Factory Binary Firmware Dump |
| `Opel kadet 2.0 0261200186 356500.ori` | **OEM Production** | 32.0 KB | `35786ed473ae2ea1e0a5459a5a572bb4` | Factory Binary Firmware Dump |
| `Opel kadet 2.0 0261200372 356158.ori` | **OEM Production** | 32.0 KB | `feac53c77f7d84dc44684d335a63c58b` | Factory Binary Firmware Dump |
| `Opel kadet 2.0 16V 0261200185 355631.ori` | **OEM Production** | 32.0 KB | `83633c5d5ab931e1812cfb83a2d44c65` | Factory Binary Firmware Dump |
| `Opel kadett 2.0 16V 0261200185 355474.ori` | **OEM Production** | 32.0 KB | `488917df007267ca292a3a70515087f0` | Factory Binary Firmware Dump |
| `Opel kadett GSI 2.0 16V 0261200185 356242.ori` | **OEM Production** | 32.0 KB | `8c0f51396916f3d97b23ea0e1518c6a2` | Factory Binary Firmware Dump |
| `Opel kadett GSI 2.0 16V 0261200185 356397.ori` | **OEM Production** | 32.0 KB | `60cf95c363f61a10d2b9e01de57f87a8` | Factory Binary Firmware Dump |
| `Opel omega 2.2DTI 0281010274.ori` | **OEM Production** | 256.0 KB | `299ee6129161b9889a664db539e87db1` | Factory Binary Firmware Dump |
| `Opel omega 2.5TD 115HP 0281001215 2287358809.ori` | **OEM Production** | 32.0 KB | `71f5604f687a18049951cfd31d0f5d24` | Factory Binary Firmware Dump |
| `Opel omega 2.5TD 130HP 0281001427 355007.ori` | **OEM Production** | 32.0 KB | `4a7069846b93eae968efb7611b3a2ecf` | Factory Binary Firmware Dump |
| `Opel omega 3.0 V6 205HP 0261203589 358933.ori` | **OEM Production** | 64.0 KB | `c3c10b539e929e1c1ef7d40a8b0a922c` | Factory Binary Firmware Dump |
| `Opel signum 1.9CDTI 150HP 0281011449 1037370821.ori` | **OEM Production** | 1.00 MB | `aee35b2036a4efccb51ca80187eb14bc` | Factory Binary Firmware Dump |
| `Opel sintra 2.2DTI 0281001637.ori` | **OEM Production** | 256.0 KB | `3974e0a1a18f06715e44c0a8fff025e6` | Factory Binary Firmware Dump |
| `Opel vectra 1.9CDTI  0281012534 383687.ori` | **OEM Production** | 1.00 MB | `05c50c6d2cce6fa55d6e8b1b1ed5fbd6` | Factory Binary Firmware Dump |
| `Opel vectra 1.9CDTI 120HP 0281012534 377187.ori` | **OEM Production** | 1.00 MB | `ea75e36cbf8694fbdac75763ef21ba8b` | Factory Binary Firmware Dump |
| `Opel vectra 1.9CDTI 150HP 0281011448 372750.ori` | **OEM Production** | 1.00 MB | `d9d08fed5d61a627a56aa20b361dafbc` | Factory Binary Firmware Dump |
| `Opel vectra 1.9CDTI 150HP 0281012869 384337 BDM.ori` | **OEM Production** | 2.00 MB | `adfdbd10a7b69dd3906b43df3f4d0761` | Factory Binary Firmware Dump |
| `Opel vectra 2.0DTI 0281001633 356489.ori` | **OEM Production** | 256.0 KB | `af17b31f0ca033c970c70a94965e84ad` | Factory Binary Firmware Dump |
| `Opel vectra 2.0DTI 0281010269.ori` | **OEM Production** | 256.0 KB | `e7c53b163b3830f26bb10f0f3372a083` | Factory Binary Firmware Dump |
| `Opel vectra 2.0DTI 100HP 0281001871 CT 09136116.ori` | **OEM Production** | 256.0 KB | `638ec0a39e34d092ae4ebfd23286dd6c` | Factory Binary Firmware Dump |
| `Opel vectra 2.0DTI 100HP 0281010269.ori` | **OEM Production** | 256.0 KB | `22be8429368b4ce1e26d9eab9a82473b` | Factory Binary Firmware Dump |
| `Opel vectra 2.2DTI 0281010271.ori` | **OEM Production** | 256.0 KB | `784b376cbce45120e96e764576bfaa10` | Factory Binary Firmware Dump |
| `Opel vectra B 2.0 16V 136HP 5WK9073 X20XEV.ori` | **OEM Production** | 128.0 KB | `e095f7d4dc0f9526fa37943e1fce8b89` | Factory Binary Firmware Dump |
| `Opel vivaro 2.0CDTI 114HP 386540.ori` | **OEM Production** | 2.00 MB | `e10dcaed0562e0e18eed00131d1e623e` | Factory Binary Firmware Dump |
| `Opel zafira 1.9CDTI 120HP 0281014452 387387.ori` | **OEM Production** | 256.0 KB | `aa02df62869e5a74e18f7c0555b0226d` | Factory Binary Firmware Dump |
| `Opel zafira 1.9CDTI 1540HP 0281014452 389374.ori` | **OEM Production** | 2.00 MB | `59dcbd924d4c208a4d8e191d07d4f2ca` | Factory Binary Firmware Dump |
| `Opel zafira 2.0DTI 0281010021 VM0M1010.ori` | **OEM Production** | 256.0 KB | `372e2947e3fc3e1b9b8565b1d165d9bf` | Factory Binary Firmware Dump |
| `Opel zafira 2.0DTI 0281010268.ori` | **OEM Production** | 256.0 KB | `dfb13c1af861185442d8dd9824e33f06` | Factory Binary Firmware Dump |
| `Opel_Astra_D1700_R4V2T_55kW_0113386350_97240621_DLCC_9391249_crcAF2F28F6.ori` | **OEM Production** | 256.0 KB | `e14ba91b5bedba8ce4849d36e90bcfe8` | Factory Binary Firmware Dump |
| `Opel_Astra_D1700_R4V4T_55kW_0113386350_97227225_DLNB_0939429_crcA432D8C9.ori` | **OEM Production** | 256.0 KB | `2f2aeba9cc7adbae284b18fefdbf2ab7` | Factory Binary Firmware Dump |
| `Opel_Frontera_D2200_R4V2T_85kW_0281010025_09173933_VU2M2W30_xxx_crc52CD7F87.ori` | **2014–2020** | 256.0 KB | `87bd521bd66b6a0d891273ffa7f1cb48` | Factory Binary Firmware Dump |
| `Opel_Zafira_B2000_R4V4T_141kW_0261207448_xxx_xxx_1037362726_crcE45766C9.ori` | **2000** | 512.0 KB | `9ecb85e7eb8c289b14ea0ac5de3d8a68` | Factory Binary Firmware Dump |
| `Opel_Zafira_R4V2_D2000_59kW_0281010268_96171442_HM7M4010_xxx_crc14d4a7c5.ori` | **2000** | 256.0 KB | `bf942b859fcf6fe71c3b6ec5fa265345` | Factory Binary Firmware Dump |
| `Opel_Zafira_R4V2_D2000_59kW_0281010268_96171442_KM7M3020_xxx_crc8dbf7fef.ori` | **2000** | 256.0 KB | `d25a263e1bf12c2750c8d9b865ed1337` | Factory Binary Firmware Dump |
| `Vauxhall -Opel Astra G 1.7dti 97240621 EADLNF.ori` | **OEM Production** | 256.0 KB | `24ff475a34ca66315997c253f6361846` | Factory Binary Firmware Dump |
| `Vectra 1.9CDTI 120PS 0281014450 1037390674P48 ORI.bin` | **OEM Production** | 2.00 MB | `6d7a687a47b3ff9b578c3ae83ec7cf67` | Factory Binary Firmware Dump |
| `eeprom.bin` | **OEM Production** | 4.0 KB | `84404ac7e43c19fde7960b7c9e16a014` | Factory Binary Firmware Dump |
| `mpc555.bin` | **OEM Production** | 452.0 KB | `51d33ff0fd5e9fee0c6022dc1f5eaa9c` | Factory Binary Firmware Dump |
| `z13dt.ori.bin` | **OEM Production** | 448.0 KB | `2d4c9f12e27deda47cc42680ba07d3f8` | Factory Binary Firmware Dump |

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
