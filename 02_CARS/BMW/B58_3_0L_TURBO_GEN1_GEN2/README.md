# B58_3_0L_TURBO_GEN1_GEN2 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/B58_3_0L_TURBO_GEN1_GEN2`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `405 files` (140 binary dumps, 265 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `B58_3_0L_TURBO_GEN1_GEN2` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2015–2026

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `00003076501103.xdf` | **2015–2026** | 1.44 MB | `00217d4176a16d454d25229812820efa` | TunerPro Binary Definition Map |
| `00003076501103_MapSwitchBase.bin` | **2015–2026** | 7.50 MB | `76f8861793f099c08644bb01631034da` | Factory Binary Firmware Dump |
| `00003076501103_original.bin` | **2015–2026** | 7.50 MB | `8b9573bf5009b1e4d65ee3391848b28b` | Factory Binary Firmware Dump |
| `00003076501D02.xdf` | **2015–2026** | 1.44 MB | `e8d52842acbb00f1a4f6dbb05173e287` | TunerPro Binary Definition Map |
| `00003076501D02_MapSwitchBase.bin` | **2015–2026** | 7.50 MB | `c759b8a34de0f24a5dddaed493f8851a` | Factory Binary Firmware Dump |
| `00003076501D02_original.bin` | **2015–2026** | 7.50 MB | `707e5620335e88155cf16fb11924b354` | Factory Binary Firmware Dump |
| `000030765A3205.xdf` | **2015–2026** | 1.42 MB | `9045002b8d2935ea3ca96319c86b24e7` | TunerPro Binary Definition Map |
| `000030765A3C06.xdf` | **2015–2026** | 1.43 MB | `18b7bdbda2628b943b0950d03064e022` | TunerPro Binary Definition Map |
| `000030765A3C06_MapSwitchBase.bin` | **2015–2026** | 7.50 MB | `e6ccbc87ad6bfc132e6d7e40529dd83f` | Factory Binary Firmware Dump |
| `000030765A3C06_original.bin` | **2015–2026** | 7.50 MB | `337685cc630cd3b2170fdace8d3eea80` | Factory Binary Firmware Dump |
| `000030765A5005.xdf` | **2015–2026** | 1.50 MB | `37e94e15a37afe7d6b693eb2743ce0a2` | TunerPro Binary Definition Map |
| `00003081501102.xdf` | **2015–2026** | 1.42 MB | `3110580438b22b045162e30175492b0f` | TunerPro Binary Definition Map |
| `00003081501102_MapSwitchBase.bin` | **2015–2026** | 7.50 MB | `d361517f6421e448f0213c4a09805db7` | Factory Binary Firmware Dump |
| `00003081501102_original.bin` | **2015–2026** | 7.50 MB | `bcb970a18d374f84ba2233b8a1778892` | Factory Binary Firmware Dump |
| `00003081501D04.xdf` | **2015–2026** | 1.42 MB | `f517518bb78c841b01ff9bc14cb445d0` | TunerPro Binary Definition Map |
| `00003081501D04_MapSwitchBase.bin` | **2015–2026** | 7.50 MB | `3d124aaa145b1bb8dda7c04d9b8a4421` | Factory Binary Firmware Dump |
| `00003081501D04_original.bin` | **2015–2026** | 7.50 MB | `dad0c5753740123a16ebe8e1014082bd` | Factory Binary Firmware Dump |
| `00005D55289606.xdf` | **2015–2026** | 1.70 MB | `2606c69f1a2dc6580809f3950d40e517` | TunerPro Binary Definition Map |
| `00005D55289606_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `bcae1f9b2c9ce546f68a5b1405f8e0a0` | Factory Binary Firmware Dump |
| `00005D55289606_original.bin` | **2015–2026** | 8.00 MB | `e443aa6005f91b68731985e3e8c572f1` | Factory Binary Firmware Dump |
| `00005D5528AA06.xdf` | **2015–2026** | 1.71 MB | `1db2be013ffd670a067a0e3dd4d0b337` | TunerPro Binary Definition Map |
| `00005D5528AA06_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `da41f76f2f36257fc58b3e02c0b0d818` | Factory Binary Firmware Dump |
| `00005D5528AA06_original.bin` | **2015–2026** | 8.00 MB | `3b901ecad128789e7a6cff0042ca9ead` | Factory Binary Firmware Dump |
| `00005D5528B405.xdf` | **2015–2026** | 1.70 MB | `ef069ae74c531526780999ca4b326e47` | TunerPro Binary Definition Map |
| `00005D5528B405_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `00df17663920b24be29d92ec29cc0bc6` | Factory Binary Firmware Dump |
| `00005D5528B405_original.bin` | **2015–2026** | 8.00 MB | `48159e2bd2f335f0ad844a09fe0969ff` | Factory Binary Firmware Dump |
| `00005D5528BE07.xdf` | **2015–2026** | 1.70 MB | `ef069ae74c531526780999ca4b326e47` | TunerPro Binary Definition Map |
| `00005D5528BE07_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `94e8a84ecb240da9688bdb4803f789e8` | Factory Binary Firmware Dump |
| `00005D5528BE07_original.bin` | **2015–2026** | 8.00 MB | `7a2dd9eb1af5bd2bcbb766204985e11e` | Factory Binary Firmware Dump |
| `00005D5528BE09.xdf` | **2015–2026** | 1.70 MB | `ef069ae74c531526780999ca4b326e47` | TunerPro Binary Definition Map |
| `00005D5528BE09_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `63ad8711bbf76b3baadd7aca492c676b` | Factory Binary Firmware Dump |
| `00005D5528BE09_original.bin` | **2015–2026** | 8.00 MB | `72f163fb317174de4a9db9351c8516c2` | Factory Binary Firmware Dump |
| `00005D55327806.xdf` | **2015–2026** | 1.74 MB | `dd9c005e9b973ce406026904cdb4b489` | TunerPro Binary Definition Map |
| `00005D55327806_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `eb169faacb5e69b0f8efee672c580c77` | Factory Binary Firmware Dump |
| `00005D55327806_original.bin` | **2015–2026** | 8.00 MB | `27cf187aff1c1d10bec4f8a91b2763d3` | Factory Binary Firmware Dump |
| `00005D55328C05.xdf` | **2015–2026** | 1.74 MB | `86d77e3a4b0f4f9135c2969bc2cb242c` | TunerPro Binary Definition Map |
| `00005D55328C05_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `603d1399f3b5685a9fcc6de6dd80e286` | Factory Binary Firmware Dump |
| `00005D55328C05_original.bin` | **2015–2026** | 8.00 MB | `bb03193cd48a25a6eb5013c592347850` | Factory Binary Firmware Dump |
| `00005D55329606.xdf` | **2015–2026** | 1.74 MB | `38b04697ac3b80cf462452cd32533af3` | TunerPro Binary Definition Map |
| `00005D55329606_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `64c4aefd5f1f90a7a03ce17b8a6180e8` | Factory Binary Firmware Dump |
| `00005D55329606_original.bin` | **2015–2026** | 8.00 MB | `d448d38c86fe2a6ad5c84f49834e2af3` | Factory Binary Firmware Dump |
| `00005D5532BE07.xdf` | **2015–2026** | 1.73 MB | `bd266e23c5fe5051788a55010f451d91` | TunerPro Binary Definition Map |
| `00005D5532BE07_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `f0f53b1e0f12d9a37b84640620ba354b` | Factory Binary Firmware Dump |
| `00005D5532BE07_original.bin` | **2015–2026** | 8.00 MB | `4036d39239c36d8efc6ffe447ff70192` | Factory Binary Firmware Dump |
| `00005D5532BE09.xdf` | **2015–2026** | 1.73 MB | `bd266e23c5fe5051788a55010f451d91` | TunerPro Binary Definition Map |
| `00005D5532BE09_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `04bbe85a5ceb658e41e47b6112938e32` | Factory Binary Firmware Dump |
| `00005D5532BE09_original.bin` | **2015–2026** | 8.00 MB | `5c3c0b053b7e63c42cc4b92338663e79` | Factory Binary Firmware Dump |
| `00005D5532C808.xdf` | **2015–2026** | 1.88 MB | `1c057ee57ee29bcf5002115a8e133568` | TunerPro Binary Definition Map |
| `00005D5532C808_original.bin` | **2015–2026** | 8.00 MB | `d8ae396f6acc2b4a348509d01b13de93` | Factory Binary Firmware Dump |
| `00005D5532DC05.xdf` | **2015–2026** | 1.73 MB | `aa596bfa3a9bb8888db0744f2b274eda` | TunerPro Binary Definition Map |
| `00005D5532DC05_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `ed8777cea732f4c6d31a171aa865add2` | Factory Binary Firmware Dump |
| `00005D5532DC05_original.bin` | **2015–2026** | 8.00 MB | `657ad211f3882daeaca844e0a18d381e` | Factory Binary Firmware Dump |
| `00005D5532E605.xdf` | **2015–2026** | 1.58 MB | `e51fe93e536fd585a964ac41dc7c0f0c` | TunerPro Binary Definition Map |
| `00005D553C6405.xdf` | **2015–2026** | 1.74 MB | `0a1997a922d71bdce2b92a255b59ef19` | TunerPro Binary Definition Map |
| `00005D553C6405_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `eedf841ae7fc23119f7e0e9ab3038e7e` | Factory Binary Firmware Dump |
| `00005D553C6405_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `1b54c4c2d68ebb6b0d5aee4d82fbfa33` | Factory Binary Firmware Dump |
| `00005D553C6405_b58o1_original.bin` | **2015–2026** | 8.00 MB | `4c5eb075b823569e0c2c288935f2d03b` | Factory Binary Firmware Dump |
| `00005D553C6405_original.bin` | **2015–2026** | 8.00 MB | `cfa22cddc9644c25785218cd4f02076a` | Factory Binary Firmware Dump |
| `00005D553C6E05.xdf` | **2015–2026** | 1.74 MB | `541630a98964ecdbb6588551fbd830fb` | TunerPro Binary Definition Map |
| `00005D553C6E05_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `c748993b6c1a9683eaaed21a62f467c1` | Factory Binary Firmware Dump |
| `00005D553C6E05_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `d5f692d2fa8e1824b77df5a863058270` | Factory Binary Firmware Dump |
| `00005D553C6E05_b58o1_original.bin` | **2015–2026** | 8.00 MB | `43c994e260447965d2eac6fdb86d09f8` | Factory Binary Firmware Dump |
| `00005D553C6E05_original.bin` | **2015–2026** | 8.00 MB | `3c274b7e7879fcf0937b7263e5f0de2f` | Factory Binary Firmware Dump |
| `00005D553C7805.xdf` | **2015–2026** | 1.74 MB | `2567e02866460b1b0e5d08c992ec91f8` | TunerPro Binary Definition Map |
| `00005D553C7805_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `79c2253d11db20b69fb51961e7adea35` | Factory Binary Firmware Dump |
| `00005D553C7805_original.bin` | **2015–2026** | 8.00 MB | `1d31da5608c10a8a8f4a962cf6675d37` | Factory Binary Firmware Dump |
| `00005D553C7807.xdf` | **2015–2026** | 1.74 MB | `65dc526431f58964ac9e57af5ee8b250` | TunerPro Binary Definition Map |
| `00005D553C7807_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `552d9e3b46e91ca3d66ee58f59564539` | Factory Binary Firmware Dump |
| `00005D553C7807_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `8efbcb2756ea0b8a61eae51789def1cb` | Factory Binary Firmware Dump |
| `00005D553C7807_b58o1_original.bin` | **2015–2026** | 8.00 MB | `f26a599f70ce5c4e23b1c6cbedea5c9b` | Factory Binary Firmware Dump |
| `00005D553C7807_original.bin` | **2015–2026** | 8.00 MB | `986563d4e25e46a6a929cad2b338b768` | Factory Binary Firmware Dump |
| `00005D553C8207.xdf` | **2015–2026** | 1.74 MB | `c7052ea46ccf14bb5ae30d8aa2428839` | TunerPro Binary Definition Map |
| `00005D553C8207_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `dd588795d80d39d6ec267dc32628a29c` | Factory Binary Firmware Dump |
| `00005D553C8207_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `34ae1342a9d2857fbcc83cdc7f9c7d93` | Factory Binary Firmware Dump |
| `00005D553C8207_b58o1_original.bin` | **2015–2026** | 8.00 MB | `35194307097a5d1172953e18af116e2e` | Factory Binary Firmware Dump |
| `00005D553C8207_original.bin` | **2015–2026** | 8.00 MB | `3b9b2fabbec6f09b95b62b7b44aa0099` | Factory Binary Firmware Dump |
| `00005D553C8C05.xdf` | **2015–2026** | 1.74 MB | `4955e6ed9356635f133a514bf7ffc442` | TunerPro Binary Definition Map |
| `00005D553C8C05_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `e519ba35857f066f4b0294062fd65240` | Factory Binary Firmware Dump |
| `00005D553C8C05_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `ae223b9c51898cb3ef71f2a2b9ff4e3c` | Factory Binary Firmware Dump |
| `00005D553C8C05_b58o1_original.bin` | **2015–2026** | 8.00 MB | `6ef607b7e12610cf094d281c6dcb0577` | Factory Binary Firmware Dump |
| `00005D553C8C05_original.bin` | **2015–2026** | 8.00 MB | `6c438db1d2c843cd3a72e52105ec541c` | Factory Binary Firmware Dump |
| `00005D553C9607.xdf` | **2015–2026** | 1.74 MB | `a0cef83fb19ae26bbf039a69556e5cce` | TunerPro Binary Definition Map |
| `00005D553C9607_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `407c477ce2f9605d02eb1a716c5d8405` | Factory Binary Firmware Dump |
| `00005D553C9607_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `73cdea535c3de1e999ee4634f2adcf0a` | Factory Binary Firmware Dump |
| `00005D553C9607_b58o1_original.bin` | **2015–2026** | 8.00 MB | `8eaa71c582ca8b2126c39eb37baae7a3` | Factory Binary Firmware Dump |
| `00005D553C9607_original.bin` | **2015–2026** | 8.00 MB | `b8a852dbd756ab20ee59059f6db1355d` | Factory Binary Firmware Dump |
| `00005D553CA007.xdf` | **2015–2026** | 1.74 MB | `1deadce40cc82b7f93b51194d6d4e502` | TunerPro Binary Definition Map |
| `00005D553CA007_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `b66394f0614b6170e73e233db70d9e50` | Factory Binary Firmware Dump |
| `00005D553CA007_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `6d3cb93245433529d6ef83423d3cfe19` | Factory Binary Firmware Dump |
| `00005D553CA007_b58o1_original.bin` | **2015–2026** | 8.00 MB | `9d833d603fa3806a5ae233c470fe0832` | Factory Binary Firmware Dump |
| `00005D553CA007_original.bin` | **2015–2026** | 8.00 MB | `28278f1d405dcbe458eaa353a26c1c95` | Factory Binary Firmware Dump |
| `00005D553CA009.xdf` | **2015–2026** | 1.73 MB | `0f7b291f828f06067571bcc35e9a9ed0` | TunerPro Binary Definition Map |
| `00005D553CA009_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `5151be22f7e962b443876ac5983f9000` | Factory Binary Firmware Dump |
| `00005D553CA009_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `ceaf836223a87574be32410f0816a1ce` | Factory Binary Firmware Dump |
| `00005D553CA009_b58o1_original.bin` | **2015–2026** | 8.00 MB | `17071e48737b3c4e8231f86f6c8c384e` | Factory Binary Firmware Dump |
| `00005D553CA009_original.bin` | **2015–2026** | 8.00 MB | `a4f42e0ba8b3337256a82877c27bbf38` | Factory Binary Firmware Dump |
| `00005D553CAA08.xdf` | **2015–2026** | 1.74 MB | `fe80923d7a010221b781859fb0de5a7c` | TunerPro Binary Definition Map |
| `00005D553CAA08_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `47aa2b0c4bd952b634711f18157bf87b` | Factory Binary Firmware Dump |
| `00005D553CAA08_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `6e72bdc38724831d93725a51b2a1d8cc` | Factory Binary Firmware Dump |
| `00005D553CAA08_b58o1_original.bin` | **2015–2026** | 8.00 MB | `615fb8acbaaf9170a23cc0f6ac0bceaa` | Factory Binary Firmware Dump |
| `00005D553CAA08_original.bin` | **2015–2026** | 8.00 MB | `08825ebce1c975e0dd04a082ec132620` | Factory Binary Firmware Dump |
| `00005D553CBE05.xdf` | **2015–2026** | 1.74 MB | `a734105c05d4c10ebc98c241d480630e` | TunerPro Binary Definition Map |
| `00005D553CBE05_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `84e6659285087cc6be04b9b7c0b29da7` | Factory Binary Firmware Dump |
| `00005D553CBE05_b58o1_original.bin` | **2015–2026** | 8.00 MB | `7130614befe0d3ec4db767db65f36f92` | Factory Binary Firmware Dump |
| `00005D553CC805.xdf` | **2015–2026** | 1.73 MB | `d096e6febcd66269d55b059d8ce8016e` | TunerPro Binary Definition Map |
| `00005D553CC805_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `d04ca4f190337aa91e6024587a4ce6e8` | Factory Binary Firmware Dump |
| `00005D553CC805_b58o1_original.bin` | **2015–2026** | 8.00 MB | `209474e21c23271e03fa553d18e1b7ac` | Factory Binary Firmware Dump |
| `00005D55461E08.xdf` | **2015–2026** | 1.74 MB | `8c5e755acd721af2617d1853e7437f64` | TunerPro Binary Definition Map |
| `00005D55461E08_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `85838e7af398b6d0a9a80e270c4fa8b1` | Factory Binary Firmware Dump |
| `00005D55461E08_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `e17d573b870fa754b589736ebf8ae6da` | Factory Binary Firmware Dump |
| `00005D55461E08_b58o1_original.bin` | **2015–2026** | 8.00 MB | `a5ee1a1ca6bb64e8a3788bed299c4612` | Factory Binary Firmware Dump |
| `00005D55461E08_original.bin` | **2015–2026** | 8.00 MB | `3783aa2a3ddfdb69fe070d28fc828bc0` | Factory Binary Firmware Dump |
| `00005D55463208.xdf` | **2015–2026** | 1.73 MB | `38e08a07946f243c98dff0186574d591` | TunerPro Binary Definition Map |
| `00005D55463208_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `0104cc078d65ab0d757035ee8c243da5` | Factory Binary Firmware Dump |
| `00005D55463208_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `9b22ed383824cf84d1c57eccec5a632e` | Factory Binary Firmware Dump |
| `00005D55463208_b58o1_original.bin` | **2015–2026** | 8.00 MB | `753ecc208ba78b57a4d1f4a6df3acd1f` | Factory Binary Firmware Dump |
| `00005D55463208_original.bin` | **2015–2026** | 8.00 MB | `f2e187610659079314929c4a9410a25f` | Factory Binary Firmware Dump |
| `00005D55463C07.xdf` | **2015–2026** | 1.73 MB | `06c021888fea8618b1fd5a5174931d02` | TunerPro Binary Definition Map |
| `00005D55463C07_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `1156da5aacd62ced1c9c00333a2e5cea` | Factory Binary Firmware Dump |
| `00005D55463C07_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `63f9d86f6a1d6268258712392ef9777c` | Factory Binary Firmware Dump |
| `00005D55463C07_b58o1_original.bin` | **2015–2026** | 8.00 MB | `4ba1bf9407157bfe8362323a380c1333` | Factory Binary Firmware Dump |
| `00005D55463C07_original.bin` | **2015–2026** | 8.00 MB | `0bc03cc09b8b67750528a29fc6762250` | Factory Binary Firmware Dump |
| `00005D55464605.xdf` | **2015–2026** | 1.73 MB | `a3d80925ab1ecb23f9bb33aad788052e` | TunerPro Binary Definition Map |
| `00005D55464605_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `64742322ee9bbff9ecc8ea906d1c2413` | Factory Binary Firmware Dump |
| `00005D55464605_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `ef26e0f121bdab4eec841b3b69756f2a` | Factory Binary Firmware Dump |
| `00005D55464605_b58o1_original.bin` | **2015–2026** | 8.00 MB | `d639268274f3838851cb3a1459d500ff` | Factory Binary Firmware Dump |
| `00005D55464605_original.bin` | **2015–2026** | 8.00 MB | `e89eca3866b88cfbc03753da9065a80c` | Factory Binary Firmware Dump |
| `00005D55465005.xdf` | **2015–2026** | 1.73 MB | `2e3d325c340c0d47acc93ab4e3a195c1` | TunerPro Binary Definition Map |
| `00005D55465005_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `a7aad45a42b87cbeafb9cf0e88456e85` | Factory Binary Firmware Dump |
| `00005D55465005_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `0d8f727d5f0f9d7749f61e5e3e283ab5` | Factory Binary Firmware Dump |
| `00005D55465005_b58o1_original.bin` | **2015–2026** | 8.00 MB | `e135c32a3f661f39374c28a5892e0b53` | Factory Binary Firmware Dump |
| `00005D55465005_original.bin` | **2015–2026** | 8.00 MB | `50afbc4258e1cee931d3d59446115659` | Factory Binary Firmware Dump |
| `00005D55465A07.xdf` | **2015–2026** | 1.73 MB | `05c61e85761ab01430379502ee777c4b` | TunerPro Binary Definition Map |
| `00005D55465A07_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `37b54f4333d79fe27a9be2ca0fcbef1f` | Factory Binary Firmware Dump |
| `00005D55465A07_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `7961dae3c1df592fa97ce1459261fb11` | Factory Binary Firmware Dump |
| `00005D55465A07_b58o1_original.bin` | **2015–2026** | 8.00 MB | `f0959339fa2e5572265adfce9127b957` | Factory Binary Firmware Dump |
| `00005D55465A07_original.bin` | **2015–2026** | 8.00 MB | `1b05e32a8d18da5f4ca3096063425f8d` | Factory Binary Firmware Dump |
| `00005D55465A09.xdf` | **2015–2026** | 1.73 MB | `05c61e85761ab01430379502ee777c4b` | TunerPro Binary Definition Map |
| `00005D55465A09_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `ce93cfea07134c9c2a03d962d24a1a6d` | Factory Binary Firmware Dump |
| `00005D55465A09_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `69ef92cde1e448446ff7b8162806c0b9` | Factory Binary Firmware Dump |
| `00005D55465A09_b58o1_original.bin` | **2015–2026** | 8.00 MB | `ad196ead00c6f358743c599e1c9389d2` | Factory Binary Firmware Dump |
| `00005D55465A09_original.bin` | **2015–2026** | 8.00 MB | `c82714a45958935329331f7f02db215e` | Factory Binary Firmware Dump |
| `00005D55466408.xdf` | **2015–2026** | 1.73 MB | `5e7caaef74f078a8b5f1b4f326c4417b` | TunerPro Binary Definition Map |
| `00005D55466408_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `dcc156e0d4480f3f70e092409a02c4c9` | Factory Binary Firmware Dump |
| `00005D55466408_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `a54a3d65991c0d6cf23ef6e316622179` | Factory Binary Firmware Dump |
| `00005D55466408_b58o1_original.bin` | **2015–2026** | 8.00 MB | `7bdc27e731e07fc2d1f8e901cd34f0dc` | Factory Binary Firmware Dump |
| `00005D55466408_original.bin` | **2015–2026** | 8.00 MB | `640bad00bdcd8e30166eb37dd1261fe8` | Factory Binary Firmware Dump |
| `00005D55467805.xdf` | **2015–2026** | 1.73 MB | `284eebdafcd236c157ebd2af402481f6` | TunerPro Binary Definition Map |
| `00005D55467805_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `523485ea49e6b9e6f29cdbefc021edd6` | Factory Binary Firmware Dump |
| `00005D55467805_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `84de2cf858fe4bc8574b5c0444e3e9dd` | Factory Binary Firmware Dump |
| `00005D55467805_b58o1_original.bin` | **2015–2026** | 8.00 MB | `94ade113f9eec9bfdbd3a7c369bb0e55` | Factory Binary Firmware Dump |
| `00005D55467805_original.bin` | **2015–2026** | 8.00 MB | `80a8a05927c444074d41cf3a0fd4f511` | Factory Binary Firmware Dump |
| `00005D55468205.xdf` | **2015–2026** | 1.72 MB | `3987c3d97ee7798ab3e9f7096f327d31` | TunerPro Binary Definition Map |
| `00005D55468205_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `1fd35ed044721dc97bc19ddefef59cc2` | Factory Binary Firmware Dump |
| `00005D55468205_b58o1_original.bin` | **2015–2026** | 8.00 MB | `ed34f0b5d988c7e7ffdc4071ca31a1cf` | Factory Binary Firmware Dump |
| `00005D55502807.xdf` | **2015–2026** | 1.75 MB | `89784df46970f2e58809d14acd2f30b9` | TunerPro Binary Definition Map |
| `00005D55502807_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `17eb6e3b53d02ef46fbb3d11b29e05f4` | Factory Binary Firmware Dump |
| `00005D55502807_b58o1_original.bin` | **2015–2026** | 8.00 MB | `7c9b840fae034145edeee89f36ec4c71` | Factory Binary Firmware Dump |
| `00005D55503705.xdf` | **2015–2026** | 1.75 MB | `c4c0fb0166b420cff8a609075cd29cac` | TunerPro Binary Definition Map |
| `00005D55503705_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `1bdee3e13163022a56cb651517996131` | Factory Binary Firmware Dump |
| `00005D55503705_b58o1_original.bin` | **2015–2026** | 8.00 MB | `74a41c32bfb880e4d82eebed744a867b` | Factory Binary Firmware Dump |
| `00005D55503C05.xdf` | **2015–2026** | 1.75 MB | `c74438150e19e8e7764636560a69cf38` | TunerPro Binary Definition Map |
| `00005D55503C05_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `108ca678d654469128755ea82b1e4141` | Factory Binary Firmware Dump |
| `00005D55503C05_b58o1_original.bin` | **2015–2026** | 8.00 MB | `a2fddd30e6d0f8aabd03541bf2d1c059` | Factory Binary Firmware Dump |
| `00005D55504807.xdf` | **2015–2026** | 1.75 MB | `0fb0ff91bfe36623d4f38fb947b4f57c` | TunerPro Binary Definition Map |
| `00005D55504807_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `6d0d685b0aef0ffcda7f27385c952221` | Factory Binary Firmware Dump |
| `00005D55504807_b58o1_original.bin` | **2015–2026** | 8.00 MB | `4ffd27545875cca7ac4c56387b48465b` | Factory Binary Firmware Dump |
| `00005D55504809.xdf` | **2015–2026** | 1.75 MB | `0fb0ff91bfe36623d4f38fb947b4f57c` | TunerPro Binary Definition Map |
| `00005D55504809_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `2dafae850c66d4544e6105c5ec3fcfd5` | Factory Binary Firmware Dump |
| `00005D55504809_b58o1_original.bin` | **2015–2026** | 8.00 MB | `edfdc5665b9bfa080179273eee110544` | Factory Binary Firmware Dump |
| `00005D5550480C.xdf` | **2015–2026** | 1.75 MB | `5f5b12db9b55e5315e32209c35c52480` | TunerPro Binary Definition Map |
| `00005D5550480C_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `ab78b5a56ec136371a540bafce65014c` | Factory Binary Firmware Dump |
| `00005D5550480C_b58o1_original.bin` | **2015–2026** | 8.00 MB | `8dde5a4c9e8af1cf229829c79f6dc834` | Factory Binary Firmware Dump |
| `00005D55505008.xdf` | **2015–2026** | 1.75 MB | `d62a1fe392c03186c269f06f179d9bc0` | TunerPro Binary Definition Map |
| `00005D55505008_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `51b3fcabcd14a69fa2867765693dcd33` | Factory Binary Firmware Dump |
| `00005D55505008_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `f1b02fa73db4d64c5ec90a98ad9d22a6` | Factory Binary Firmware Dump |
| `00005D55505008_b58o1_original.bin` | **2015–2026** | 8.00 MB | `dd3ac2266395e48e551bd134b4353298` | Factory Binary Firmware Dump |
| `00005D55505008_original.bin` | **2015–2026** | 8.00 MB | `5e68c98a974b03b8831b3c5887a76ae7` | Factory Binary Firmware Dump |
| `00005D55506405.xdf` | **2015–2026** | 1.75 MB | `33dbcd18d8976502e73991edaef87399` | TunerPro Binary Definition Map |
| `00005D55506405_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `c33a4dc32af5704253b135bb78c6dacc` | Factory Binary Firmware Dump |
| `00005D55506405_original.bin` | **2015–2026** | 8.00 MB | `35cc73dea4ae494b17bdfa0cc2798f11` | Factory Binary Firmware Dump |
| `00005D55506406.xdf` | **2015–2026** | 1.75 MB | `96faeae26d34eb9b10c011dfa4abbcad` | TunerPro Binary Definition Map |
| `00005D55506406_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `7b4503d5a7c775919da6856865208317` | Factory Binary Firmware Dump |
| `00005D55506406_b58o1_original.bin` | **2015–2026** | 8.00 MB | `3b3ffd1af73b677043f75bf816359710` | Factory Binary Firmware Dump |
| `00005D55508C05.xdf` | **2015–2026** | 1.74 MB | `4d3febd06a0d6c91747d5d5c0a14c43f` | TunerPro Binary Definition Map |
| `00005D55508C05_b58o1_MapSwitchBase.bin` | **2015–2026** | 8.00 MB | `2986bb69bded56d6b4741989deec5aae` | Factory Binary Firmware Dump |
| `00005D55508C05_b58o1_original.bin` | **2015–2026** | 8.00 MB | `6cd968e138fa5809ced11d5b94b1f24e` | Factory Binary Firmware Dump |
| `00007972000505.xdf` | **2015–2026** | 1.46 MB | `c2ffb142d1eafb5b0277aa1c937f04aa` | TunerPro Binary Definition Map |
| `00007972000705.xdf` | **2015–2026** | 1.46 MB | `96f60f893801a8218948135b1affd3a3` | TunerPro Binary Definition Map |
| `00007972000705_original.bin` | **2015–2026** | 7.50 MB | `02e0f6bf5a53cc47169faff717db8054` | Factory Binary Firmware Dump |
| `R0C9J8B2B_3081-080_017_002.a2l` | **2015–2026** | 386.1 KB | `cb43b8aa50cdf25975f5820bf66393ac` | ASAM ASAP2 ECU Description File |
| `R0C9J8B2B_3081-080_017_002_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `7f49b46f45ee23f5c62816e037a05f82` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002.a2l` | **2015–2026** | 386.1 KB | `9d178c10946072783c664e90cff74d63` | ASAM ASAP2 ECU Description File |
| `R0C9J8D2B_3081-080_021_002_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `fd3592c4bae717cebd36c13ad8bd9613` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002.a2l` | **2015–2026** | 386.1 KB | `4fe2768a0520ccb5baccb9cf47db5fa8` | ASAM ASAP2 ECU Description File |
| `R0C9J8I2B_3081-080_029_002_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `82dcbc174bc95291d684aa28b7aa1aa3` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003.a2l` | **2015–2026** | 386.1 KB | `1702c88c998fb647fe3388a101c0dc1e` | ASAM ASAP2 ECU Description File |
| `R0C9J8I3B_3081-080_029_003_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `e598acab19ed437468bb8a190672ba7d` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004.a2l` | **2015–2026** | 386.1 KB | `6dfe004866ed11e3500d8290b95fc25d` | ASAM ASAP2 ECU Description File |
| `R0C9J8I4B_3081-080_029_004_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `e8484d103902c6e0d2989c5abc9b56dd` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002.a2l` | **2015–2026** | 386.1 KB | `497f08e0487cccf4b5bdb0abd388864b` | ASAM ASAP2 ECU Description File |
| `R0C9J962B_3081-090_010_002_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `9f8b12fab0f3f2d32078fc88c52d75d0` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003.a2l` | **2015–2026** | 386.1 KB | `3a84d98af2854b8df9270ccbbc58f21a` | ASAM ASAP2 ECU Description File |
| `R0C9J9E3B_3081-090_020_003_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `3c05377c33fe7d0f216386428d2792ea` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004.a2l` | **2015–2026** | 386.1 KB | `da592a6e9e9f50a54925075f6d34e3e9` | ASAM ASAP2 ECU Description File |
| `R0C9J9E4B_3081-090_020_004_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `47f927379495778ea9b1eea1446bef0e` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005.a2l` | **2015–2026** | 386.1 KB | `aae93b1347aaf3717036db72e318a1dd` | ASAM ASAP2 ECU Description File |
| `R0C9JA05B_3081-090_025_005_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `d2a1488c15499d9bba6b2c0a566e72df` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005.a2l` | **2015–2026** | 386.1 KB | `eeb278610e27e647d7a40bd9c3a55c3b` | ASAM ASAP2 ECU Description File |
| `R0C9JA15B_3081-090_030_005_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `c363e0f6a126971877f8aea05ef4d5dd` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005.a2l` | **2015–2026** | 386.1 KB | `57b4a5d6ea066f9052de58b02e55afd3` | ASAM ASAP2 ECU Description File |
| `R0C9JC05B_3081-090_050_005_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `d5d7f33413fba2c1d206b1b2e8b01976` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006.a2l` | **2015–2026** | 386.1 KB | `9f48f188711b3d0ddc17a94bde0b2e7a` | ASAM ASAP2 ECU Description File |
| `R0C9JD06B_3081-090_060_006_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `06f1e3ec6755d8b341acabf8b839adc9` | ASAM ASAP2 ECU Description File |
| `R0C9JE15B_3081-090_080_005.a2l` | **2015–2026** | 386.1 KB | `19ad03eba45185a7b9868b8b2b1c495e` | ASAM ASAP2 ECU Description File |
| `R0C9JE15B_3081-090_080_005_v7.3.3.a2l` | **2015–2026** | 894.2 KB | `2cb619abdd3ed9b9473aaf86807864ba` | ASAM ASAP2 ECU Description File |
| `R0R96015B_7706-000_007_005.a2l` | **2015–2026** | 386.4 KB | `5f9d06828919697156f028ab47e9c039` | ASAM ASAP2 ECU Description File |
| `R0R96025B_7706-000_008_005.a2l` | **2015–2026** | 386.4 KB | `0f54d1d667bfc6ccd68b8a9bc391a1a9` | ASAM ASAP2 ECU Description File |
| `R0R9A005B_7706-000_011_005.a2l` | **2015–2026** | 386.4 KB | `fa61d3dca9f21df202d33ed4b02c3f12` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002.a2l` | **2015–2026** | 358.4 KB | `0e7c61e00f5fa1d9114911fa3dcb8b14` | ASAM ASAP2 ECU Description File |
| `R1C9I562B_3076-050_006_002_v7.3.3.a2l` | **2015–2026** | 860.1 KB | `d2e0e4274ebc386f5742220676039c4a` | ASAM ASAP2 ECU Description File |
| `R1C9J772B_3076-070_009_002.a2l` | **2015–2026** | 379.5 KB | `92264d4684d71ee891b80285c2803473` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002.a2l` | **2015–2026** | 386.1 KB | `c11f935c694377679990faf7c43f4456` | ASAM ASAP2 ECU Description File |
| `R1C9J8B2B_3076-080_017_002_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `90d75e37bfabe3f41329446d57957f3e` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003.a2l` | **2015–2026** | 386.1 KB | `642a0f1e7d18a5b3a04574494660b3b7` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_3076-080_017_003_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `96e732ad786c4a8bd148e351b1421b1d` | ASAM ASAP2 ECU Description File |
| `R1C9J8B3B_MultiMap_full.ols_CCv6.9_ver1.1.kp` | **2015–2026** | 105.5 KB | `d20813895f40f75554c79369ace0fc3c` | WinOLS Map Definition Pack |
| `R1C9J8B3B_MultiMap_full_CCv6.9_ver1.1.xdf` | **2015–2026** | 223.4 KB | `78516eeb99758de6833a104ef788ace7` | TunerPro Binary Definition Map |
| `R1C9J8B3B_MultiMap_full_stock_data_Winols_project_CCv6.9_ver1.1.ols` | **2015–2026** | 15.81 MB | `83831be9e201c427a22e92a5a3cfc43a` | WinOLS Project Workspace |
| `R1C9J8B3B_original+stock_multimap_data_CC6.9.bin` | **2015–2026** | 7.50 MB | `b424acc799e4c7d9cfef7f5c9c1c76f4` | Factory Binary Firmware Dump |
| `R1C9J8B3B_original.bin` | **2015–2026** | 7.50 MB | `2686b94ac697269dae8d056bfa06ff79` | Factory Binary Firmware Dump |
| `R1C9J8D3B_3076-080_018_003.a2l` | **2015–2026** | 386.1 KB | `8dfcb33efc62ba8ce4f4950eb1f563ec` | ASAM ASAP2 ECU Description File |
| `R1C9J8D3B_3076-080_018_003_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `0d151b52972aad59a89245db9378a5e1` | ASAM ASAP2 ECU Description File |
| `R1C9J8G3B_3428-000_001_001.a2l` | **2015–2026** | 386.1 KB | `ccb14dba32247135cce45d1f92959081` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002.a2l` | **2015–2026** | 386.1 KB | `b53583bd92116cdde3b5cf604562a6f0` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_3076-080_029_002_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `f5b1048fb692f2cf87ecbc613ebd4ddb` | ASAM ASAP2 ECU Description File |
| `R1C9J8I2B_MultiMap_full.ols_CCv6.9_ver1.1.kp` | **2015–2026** | 60.6 KB | `cffe31c8530385f489034f5539cc0978` | WinOLS Map Definition Pack |
| `R1C9J8I2B_MultiMap_full_CCv6.9_ver1.1.xdf` | **2015–2026** | 213.7 KB | `c271ed255281675632f14913420149d6` | TunerPro Binary Definition Map |
| `R1C9J8I2B_MultiMap_full_stock_data_Winols_project_CCv6.9_ver1.1.ols` | **2015–2026** | 15.80 MB | `1074c89f6d1768b23065300c6ef5fea8` | WinOLS Project Workspace |
| `R1C9J8I2B_original+stock_multimap_data_CC6.9.bin` | **2015–2026** | 7.50 MB | `69c1c94870f1abb85ef788a3f69ee855` | Factory Binary Firmware Dump |
| `R1C9J8I2B_original.bin` | **2015–2026** | 7.50 MB | `5d1761e9a8189627f036abb498fb7c33` | Factory Binary Firmware Dump |
| `R1C9J8I7B_3076-080_029_007.a2l` | **2015–2026** | 386.1 KB | `b179e7c592c71791d91de5da5bae510a` | ASAM ASAP2 ECU Description File |
| `R1C9J8I7B_3076-080_029_007_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `63b0ae89d57923be0ded3fa91b456dc6` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002.a2l` | **2015–2026** | 386.1 KB | `1be809321791f90cf3e1c729b016ed0f` | ASAM ASAP2 ECU Description File |
| `R1C9J962B_3076-090_010_002_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `63eddb93aa8d4b2b6e70e448d5b3058e` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003.a2l` | **2015–2026** | 386.1 KB | `c1f3d2bf5268abe391ffac0638f5a922` | ASAM ASAP2 ECU Description File |
| `R1C9J9E3B_3076-090_020_003_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `5245fe362f86c466c9c1cefb65855bec` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005.a2l` | **2015–2026** | 386.1 KB | `41871db55d2ef80e473ed8c9d2a14488` | ASAM ASAP2 ECU Description File |
| `R1C9J9E5B_3076-090_020_005_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `4104fcc835d0322dc074e05f9232f707` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007.a2l` | **2015–2026** | 386.1 KB | `c8da21332073d9bfcbeca83ca13a52e8` | ASAM ASAP2 ECU Description File |
| `R1C9J9E7B_3076-090_020_007_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `d2505fc7c054b9ac4ff2e012fbacd3c6` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005.a2l` | **2015–2026** | 386.1 KB | `d8758065ba6d002ffb2887ec5c09acd9` | ASAM ASAP2 ECU Description File |
| `R1C9JA05B_3076-090_025_005_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `14b4425047f41dcca341acbe6fed3a94` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005.a2l` | **2015–2026** | 386.1 KB | `ba0c6a822d7d6251966132140799d5e0` | ASAM ASAP2 ECU Description File |
| `R1C9JC05B_3076-090_050_005_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `798f44adae732a63bac72df1a31b7bdb` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006.a2l` | **2015–2026** | 386.1 KB | `547dd8687323247792fc7640e19a1179` | ASAM ASAP2 ECU Description File |
| `R1C9JD06B_3076-090_060_006_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `5e1f81e061391dc6fc80ebec9f28c031` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005.a2l` | **2015–2026** | 386.1 KB | `35e191c5f5f850e8c80de63215831ba6` | ASAM ASAP2 ECU Description File |
| `R1C9JE15B_3076-090_080_005_v7.3.3.a2l` | **2015–2026** | 894.7 KB | `0e8689342ce6148cd6c72c8529e91897` | ASAM ASAP2 ECU Description File |
| `R1R95005B_7972-000_005_005.a2l` | **2015–2026** | 386.3 KB | `4d5e94e4432b4110e5d0d5500fcebf42` | ASAM ASAP2 ECU Description File |
| `R1R96015B_7972-000_007_005.a2l` | **2015–2026** | 386.3 KB | `447c5d991d489ead0d1aa61eb1e89ee5` | ASAM ASAP2 ECU Description File |
| `R2C9C277B_3e7d-020_090_007.a2l` | **2015–2026** | 372.6 KB | `a93b6fb627ea6c8ad30beb2521c7ae74` | ASAM ASAP2 ECU Description File |
| `R2C9D392B_3e7d-030_110_002.a2l` | **2015–2026** | 384.6 KB | `f9efcc93f4ceb84fcddc69ebc0cccc39` | ASAM ASAP2 ECU Description File |
| `R2C9D3D6B_3e7d-030_120_006.a2l` | **2015–2026** | 384.4 KB | `437fa422b75425f300d137c46f598188` | ASAM ASAP2 ECU Description File |
| `R2C9D3N5B_3e7d-030_130_005.a2l` | **2015–2026** | 384.4 KB | `d8e35cdf8413176bb38268c3d2c1fe61` | ASAM ASAP2 ECU Description File |
| `R2C9D3P7B_3e7d-030_140_007.a2l` | **2015–2026** | 384.4 KB | `7ecb2a831799eb97258e78afcad5a731` | ASAM ASAP2 ECU Description File |
| `R2C9F493B_3e7d-040_100_003.a2l` | **2015–2026** | 395.4 KB | `d4608a5e73c3e8a3af7a64e17945498f` | ASAM ASAP2 ECU Description File |
| `R2C9F4K6B_3e7d-040_170_006.a2l` | **2015–2026** | 395.2 KB | `ba18e524a189a6519c74b13b2b0583e1` | ASAM ASAP2 ECU Description File |
| `R2C9F4P7B_3e7d-040_190_007.a2l` | **2015–2026** | 395.2 KB | `4d84671f412f4d27acb578dda59bfd9c` | ASAM ASAP2 ECU Description File |
| `R2C9H56AB_3e7d-050_115_010.a2l` | **2015–2026** | 403.7 KB | `ce6173bafeabdfce2be16b56bce3c9e3` | ASAM ASAP2 ECU Description File |
| `R2C9H5E6B_3e7d-050_150_006.a2l` | **2015–2026** | 403.9 KB | `29ea1dace7905487589b974ac48e0a06` | ASAM ASAP2 ECU Description File |
| `R2C9H5I5B_3e7d-050_160_005.a2l` | **2015–2026** | 403.7 KB | `0eb9112c50ac300a5e48555cd5bdfaa1` | ASAM ASAP2 ECU Description File |
| `R2C9H5P7B_3e7d-050_190_007.a2l` | **2015–2026** | 403.7 KB | `c677e6879d371a55aee1d8d914282051` | ASAM ASAP2 ECU Description File |
| `R2C9H695B_3e7d-060_100_005.a2l` | **2015–2026** | 407.0 KB | `cc1fb614012a1a7339af29a5c694671b` | ASAM ASAP2 ECU Description File |
| `R2C9H6D5B_3e7d-060_120_005.a2l` | **2015–2026** | 407.0 KB | `c58e6ef7ca9b7241d8db77539a3e0dcc` | ASAM ASAP2 ECU Description File |
| `R2C9H6H5B_3e7d-060_130_005.a2l` | **2015–2026** | 407.0 KB | `27ee9386a314717ef7118968d17d5972` | ASAM ASAP2 ECU Description File |
| `R2C9H6P7B_3e7d-060_160_007.a2l` | **2015–2026** | 407.1 KB | `b249e7e3f6ad93268fd09a151234752f` | ASAM ASAP2 ECU Description File |
| `R2C9J717B_3e7d-070_030_007.a2l` | **2015–2026** | 411.0 KB | `73e660372e9ec29fae70c22bc97ec1aa` | ASAM ASAP2 ECU Description File |
| `R2C9J756B_3e7d-070_040_006.a2l` | **2015–2026** | 410.7 KB | `c14a5177d2fbe0d41500d03d5cfaab81` | ASAM ASAP2 ECU Description File |
| `R2C9J757B_3e7d-070_040_007.a2l` | **2015–2026** | 410.7 KB | `9f86eebda101cb6ad4567539c867e169` | ASAM ASAP2 ECU Description File |
| `R2C9J795B_3e7d-070_060_005.a2l` | **2015–2026** | 410.7 KB | `1e8ee9f3f4dd1aaea80d3fcfd46df332` | ASAM ASAP2 ECU Description File |
| `R2C9J7N5B_3e7d-070_080_005.a2l` | **2015–2026** | 410.7 KB | `a7094952dda91da356562f9c48350787` | ASAM ASAP2 ECU Description File |
| `R2C9J7P7B_3e7d-070_090_007.a2l` | **2015–2026** | 410.7 KB | `4bb6b7c6787efe0df2e99c18a3657e79` | ASAM ASAP2 ECU Description File |
| `R2C9L856B_3e7d-080_040_006.a2l` | **2015–2026** | 405.5 KB | `a7a2a164c31f3cdd2b39344e934fad6c` | ASAM ASAP2 ECU Description File |
| `R2C9L8N5B_3e7d-080_060_005.a2l` | **2015–2026** | 405.5 KB | `d6fe7d4e074681eb1fced5106a35e2ed` | ASAM ASAP2 ECU Description File |
| `R2C9L8P7B_3e7d-080_072_007.a2l` | **2015–2026** | 405.5 KB | `9ef97db2d8fc3a1282bbfa031529f3a0` | ASAM ASAP2 ECU Description File |
| `R2C9L8PCB_3e7d-080_072_012.a2l` | **2015–2026** | 405.5 KB | `b2a06dba61a62f12f72c747db377312c` | ASAM ASAP2 ECU Description File |
| `R4C9F493B_5d55-040_100_003.a2l` | **2015–2026** | 395.6 KB | `de499f16978c096a06b5684eb4b3ceeb` | ASAM ASAP2 ECU Description File |
| `R4C9F493B_5d55-040_100_003_v7.3.3.a2l` | **2015–2026** | 902.3 KB | `27916a5c0b649e560520e7643be4f36f` | ASAM ASAP2 ECU Description File |
| `R4C9F4C6B_5d55-040_140_006.a2l` | **2015–2026** | 395.3 KB | `2c20fbb67215ede30f58eecd81fa3a7a` | ASAM ASAP2 ECU Description File |
| `R4C9F4C6B_5d55-040_140_006_v7.3.3.a2l` | **2015–2026** | 902.3 KB | `fd699c58a6a78d2b53c938955a961f47` | ASAM ASAP2 ECU Description File |
| `R4C9F4E6B_5d55-040_150_006.a2l` | **2015–2026** | 395.3 KB | `5dad6011f5707ab606da5854bf78595b` | ASAM ASAP2 ECU Description File |
| `R4C9F4E6B_5d55-040_150_006_v7.3.3.a2l` | **2015–2026** | 902.3 KB | `d354776de9ad578e79cf434b16c62a47` | ASAM ASAP2 ECU Description File |
| `R4C9F4G5B_5d55-040_160_005.a2l` | **2015–2026** | 395.3 KB | `f1cd5f4c89b413960150338bb39e50d7` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006.a2l` | **2015–2026** | 395.3 KB | `10b85f2784f329af1cfa909fbc019c2a` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.3.3.a2l` | **2015–2026** | 902.3 KB | `58503bd1d5c6ea56dbf72edc9b3131a5` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005.a2l` | **2015–2026** | 395.4 KB | `476d0e5293b20e405f1823433e7d69d5` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.3.3.a2l` | **2015–2026** | 902.4 KB | `9c802e1540662925b1876d92bbfba769` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007.a2l` | **2015–2026** | 395.4 KB | `ae82828f2279ce1080f2c65b36d1d37d` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.3.3.a2l` | **2015–2026** | 902.4 KB | `42ee80f032929cf807cabf6776c5350d` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009.a2l` | **2015–2026** | 395.4 KB | `a31e616a22219dfdb04ceea3c7f29d9d` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.3.3.a2l` | **2015–2026** | 902.4 KB | `cb7b9578c84afbe5d87959c5aed8e0f4` | ASAM ASAP2 ECU Description File |
| `R4C9H56AB_5d55-050_115_010.a2l` | **2015–2026** | 403.8 KB | `1c8f0517b6387673bfc079d23d8770e5` | ASAM ASAP2 ECU Description File |
| `R4C9H56AB_5d55-050_115_010_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `333ddb8de2f764f2bebd487690db621f` | ASAM ASAP2 ECU Description File |
| `R4C9H596B_5d55-050_120_006.a2l` | **2015–2026** | 403.8 KB | `5ab0aa915f967d1ae8a0a603093e9719` | ASAM ASAP2 ECU Description File |
| `R4C9H596B_5d55-050_120_006_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `a9e5c78ac5b820c4f526c31969dd33f0` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005.a2l` | **2015–2026** | 403.8 KB | `b7955b2f6295b7bc1dd5f5a8de8b58ad` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `86a342a0ea772f0bee38421faa57e421` | ASAM ASAP2 ECU Description File |
| `R4C9H5E5B_5d55-050_150_005.a2l` | **2015–2026** | 403.8 KB | `3b4b30c4533fedfa4c51bfd9bf0e8c1e` | ASAM ASAP2 ECU Description File |
| `R4C9H5E5B_5d55-050_150_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `e425e5bb0870d7960ffd057de1f3051b` | ASAM ASAP2 ECU Description File |
| `R4C9H5E6B_5d55-050_150_006.a2l` | **2015–2026** | 404.1 KB | `838f70c2fa459d676cc6d56c086a4ae1` | ASAM ASAP2 ECU Description File |
| `R4C9H5E6B_5d55-050_150_006_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `cac18da92d12c4fc357c14508156bf7e` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005.a2l` | **2015–2026** | 403.8 KB | `99e6bd3253c367798171b95ba34280ad` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `baeed4272bbde3d034523e6c4119e90f` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005.a2l` | **2015–2026** | 403.8 KB | `141e771cb3c6640045d02afdf4368984` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `a83c3d4140a5907b821cf83ad7e0fdf0` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006.a2l` | **2015–2026** | 403.9 KB | `98bdc135c4e5a3fbc242640b1399fa99` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `d2760a6a1f20f5d67421248d813ed8a6` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007.a2l` | **2015–2026** | 403.9 KB | `3d16133c920c60bd55ea4b42548f510e` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `52b75f03f650ecd76b033ca6099bc7b5` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009.a2l` | **2015–2026** | 403.9 KB | `8d62baee8691e49f1dffad1333e3a0af` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `7292db8e214f35be8e4637f28d523fbf` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008.a2l` | **2015–2026** | 403.9 KB | `dce4a8d0cd9ae40b3ade1c5513fbab78` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `f4aece1193e75d03b34dc905ccd4415e` | ASAM ASAP2 ECU Description File |
| `R4C9H5V5B_5d55-050_220_005.a2l` | **2015–2026** | 403.9 KB | `47c45dcbc815c2b358a7fc031f4584dc` | ASAM ASAP2 ECU Description File |
| `R4C9H5V5B_5d55-050_220_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `f349d17fabdecdd7771291162220cf0f` | ASAM ASAP2 ECU Description File |
| `R4C9H5W5B_5d55-050_230_005.a2l` | **2015–2026** | 403.9 KB | `bc858da539da0bbad7d0e6e61c1e0b27` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005.a2l` | **2015–2026** | 407.2 KB | `f38f407fba7282cb1efda2d632088dff` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `35570e00d9a2b98775dd357bd465a56f` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005.a2l` | **2015–2026** | 407.4 KB | `cfc8b588fea67f88e95142a345cac2e2` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `c386353a15d5253d86aee177a0c73af5` | ASAM ASAP2 ECU Description File |
| `R4C9H6D5B_5d55-060_120_005.a2l` | **2015–2026** | 407.2 KB | `73284b94d4b95639cf937c9681f4b78b` | ASAM ASAP2 ECU Description File |
| `R4C9H6D5B_5d55-060_120_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `b4d92afc9ca3a90e307100cf205ad97a` | ASAM ASAP2 ECU Description File |
| `R4C9H6D6B_5d55-060_120_006.a2l` | **2015–2026** | 407.2 KB | `e87f761f5a368bb5699d00e658c0f21f` | ASAM ASAP2 ECU Description File |
| `R4C9H6D6B_5d55-060_120_006_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `cfd9c3bc3888db2aa34b3d97a4c0aed0` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007.a2l` | **2015–2026** | 407.2 KB | `48a39f766db2c38162084a90201a78ff` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `6f788f6845f6dfffa9f2d8c445d072df` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007.a2l` | **2015–2026** | 407.2 KB | `aa05fe5026fe9cc783ffc44e79e38694` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `738f711b96821a320a58c9bdfafc8cc0` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005.a2l` | **2015–2026** | 407.2 KB | `bf5f0b33b7765d37a42fc9d4dc270a9d` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `5a9beabcea8d255b7f38756de5d05b23` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007.a2l` | **2015–2026** | 407.2 KB | `281579c2ea754eaa292556d061589ceb` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `8c9f15499d0829743781436155c182d9` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007.a2l` | **2015–2026** | 407.2 KB | `d647fad26d8c4981db7ca63dd2b51488` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `dbc922ddf862b29ec4a94d5140304566` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009.a2l` | **2015–2026** | 407.2 KB | `8804494283029d2a6d78618cd1f78f1a` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `5430ebcd01d9e435fa374cb54febecc6` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008.a2l` | **2015–2026** | 407.2 KB | `ddd3d97eb4b9ae08cacff44de25f4fe7` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `9d3b7fe3b8d0a4872bc0bbbb41db1fdc` | ASAM ASAP2 ECU Description File |
| `R4C9H6V5B_5d55-060_190_005.a2l` | **2015–2026** | 407.2 KB | `63c7b8fc8da349e41b2bfacb9df7e5ee` | ASAM ASAP2 ECU Description File |
| `R4C9H6V5B_5d55-060_190_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `95a086ac70cbb960b124f82d9a2c7585` | ASAM ASAP2 ECU Description File |
| `R4C9H6W5B_5d55-060_200_005.a2l` | **2015–2026** | 407.2 KB | `63a9d70fb8ccb73ed216c767a3052e44` | ASAM ASAP2 ECU Description File |
| `R4C9H6W5B_5d55-060_200_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `fd1e8cd6b8fcf85ee1bc0873613c56ce` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008.a2l` | **2015–2026** | 410.9 KB | `fe0603da65759f78c93eb2c1f8c5e4ae` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `6a6fa0e92a931be02c440e5956e274a6` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005.a2l` | **2015–2026** | 410.9 KB | `26c168b18661d1b0849bd69ab4391fb2` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `e39b9721c902e49038a7862c2761a867` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006.a2l` | **2015–2026** | 410.9 KB | `07d1b85bbdb91eb22e90cac045c3efa7` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `21901f91a4cd7a15e719c6eaefde6335` | ASAM ASAP2 ECU Description File |
| `R4C9J757B_5d55-070_050_007.a2l` | **2015–2026** | 410.9 KB | `d77dd3bb44b48a88c8850dce2ea05baa` | ASAM ASAP2 ECU Description File |
| `R4C9J757B_5d55-070_050_007_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `2ea50d7a5eec91db8a237bbbb76db591` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008.a2l` | **2015–2026** | 410.9 KB | `0a93552823f761633df970ab3f86fbd4` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `ce13d4e16c810c6ecd286b1020f103f2` | ASAM ASAP2 ECU Description File |
| `R4C9J795B_5d55-070_060_005.a2l` | **2015–2026** | 411.1 KB | `7788958a43a70352d1cfd4d4c2fb87d7` | ASAM ASAP2 ECU Description File |
| `R4C9J795B_5d55-070_060_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `13d0db58c8aef17a96f7c277a8d813da` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007.a2l` | **2015–2026** | 410.9 KB | `92287b15744bcb7f2479e338e806af42` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `fb436d4b307febbfd0a4882932159ab9` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005.a2l` | **2015–2026** | 410.9 KB | `3508f197159ad7ff37e392fe1cf72f60` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `c594c04d50d458d5d5389502d0768a5f` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005.a2l` | **2015–2026** | 410.9 KB | `f64c3c57ac114086d6af74ed8a4e9644` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `fcc535a52cfc8fd3e0be8aa4a54dcb7f` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007.a2l` | **2015–2026** | 410.9 KB | `5f2c8b2a26408a2a47f45b492824bfe8` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `435b65568bc792f33ba5338fa84011d3` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009.a2l` | **2015–2026** | 410.9 KB | `6bf8f8132d4a7d0dd4e008ee1e89166e` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `921c3275c45e2b1203aa23b97f983b01` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008.a2l` | **2015–2026** | 410.9 KB | `b3e805464bd2b417821aa5179a8848e7` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `3002d32dfac910793514d3b0161b673c` | ASAM ASAP2 ECU Description File |
| `R4C9J7V5B_5d55-070_120_005.a2l` | **2015–2026** | 410.9 KB | `6dc979771426a0ec0b4fbfe7d2ff68b0` | ASAM ASAP2 ECU Description File |
| `R4C9J7V5B_5d55-070_120_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `351244cc25d9c674f94c473b236db825` | ASAM ASAP2 ECU Description File |
| `R4C9J7W5B_5d55-070_130_005.a2l` | **2015–2026** | 410.9 KB | `b86e947b76485ded2b69a3952558dd0a` | ASAM ASAP2 ECU Description File |
| `R4C9J7W5B_5d55-070_130_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `e8f19c4730036ca1027458c4a056d878` | ASAM ASAP2 ECU Description File |
| `R4C9L818B_5d55-080_030_008.a2l` | **2015–2026** | 405.7 KB | `f99994ea97569ef7a9d5901f8db9c75e` | ASAM ASAP2 ECU Description File |
| `R4C9L818B_5d55-080_030_008_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `d5edb77fe3ec48c6e5f9e8f146f00c57` | ASAM ASAP2 ECU Description File |
| `R4C9L856B_5d55-080_040_006.a2l` | **2015–2026** | 405.9 KB | `b3ab8020689635ccbceffd0d60b13286` | ASAM ASAP2 ECU Description File |
| `R4C9L856B_5d55-080_040_006_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `152848a7e2c18756823fb982983b6fed` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007.a2l` | **2015–2026** | 405.7 KB | `70e52a7fe46f777c6a0a5ca505052604` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `e55195609277da00ea0aa7b64344811f` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005.a2l` | **2015–2026** | 405.7 KB | `902e4688ec35da12f3c9d8f5d5aac30f` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `e7acc60de1a9b9ea57c508008cd0407a` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005.a2l` | **2015–2026** | 405.7 KB | `10209499427dafacfff3a90dca1abc6a` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `28c6be476f5207d57148dbfc9f63cf82` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007.a2l` | **2015–2026** | 405.7 KB | `98598c20ccb63c0affe22eae9adb7934` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `b61a530de2117320477ab96fab550dd3` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009.a2l` | **2015–2026** | 405.7 KB | `30394f47f4055c923f54241f82050839` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `0bdbd56178dd9451dd637d720cf8b183` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012.a2l` | **2015–2026** | 405.7 KB | `b07a5d52383f707a03178da2c118b2ee` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `7750e59fd518a82185c3cde1342ec269` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008.a2l` | **2015–2026** | 405.7 KB | `94d23a5f2938bd5253efa95ff7159758` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `307355f7dc6ae3a1fccc33d55f25515e` | ASAM ASAP2 ECU Description File |
| `R4C9L8V5B_5d55-080_100_005.a2l` | **2015–2026** | 405.7 KB | `edc96763371e7a0c7e1479273556601a` | ASAM ASAP2 ECU Description File |
| `R4C9L8V6B_5d55-080_100_006.a2l` | **2015–2026** | 405.7 KB | `010f24b5a4a698d6ec184240c31b2199` | ASAM ASAP2 ECU Description File |
| `R4C9L8V6B_5d55-080_100_006_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `9bfb5355279559eb9467feb60275855a` | ASAM ASAP2 ECU Description File |
| `R4C9L8W9B_5d55-080_140_005.a2l` | **2015–2026** | 405.7 KB | `669a5cd77a20c94f7913a56cb5343ecc` | ASAM ASAP2 ECU Description File |
| `R4C9L8W9B_5d55-080_140_005_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `fcb06a6ad3d2d314a022537bdeae7e3e` | ASAM ASAP2 ECU Description File |
| `V0C9J6J2B_3125-065_027_002.a2l` | **2015–2026** | 348.3 KB | `bceec2dbec6912329e0600d747cc8742` | ASAM ASAP2 ECU Description File |

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
