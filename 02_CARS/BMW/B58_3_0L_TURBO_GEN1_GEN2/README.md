# BMW & Toyota GR Supra B58 3.0L Turbo Master Calibration Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi biner OEM original dan file definisi TunerPro XDF komprehensif untuk mesin modular 3.0L turbocharged inline-6 B58 Generation 1 dan Generation 2 (B58B30M0 / B58B30O1). Platform ini menggerakkan Toyota GR Supra MK5 (A90/A91), BMW M340i, M240i, 440i, 540i, 740i, X3 M40i, X5 xDrive40i, dan Z4 M40i dengan ECU Bosch MG1CS003 dan MG1CS024 (TriCore TC298TP / Aurix 32-bit MCU, 8MB Flash memory).

* **Hardware / ECU**: Bosch MG1CS003 / MG1CS024 (Infineon Aurix TriCore TC298TP, 8MB Flash ROM)
* **Metode Flashing & Antarmuka**: Bench Boot Mode / OBD Unlock via MG Flasher, Bootmod3, MHD Flasher, atau WinOLS. Perhatikan ECU lock manufaktur post-06/2020 memerlukan bench unlock khusus (Femto unlock).
* **Rentang Tahun / Model Year**: 2015–2026
* **Total File Terdaftar**: 190 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `00003076501103.xdf` | **2015–2019 (Gen 1)** | 1.44 MB | `00217d4176a16d454d25229812820efa` | TunerPro Binary Definition Map |
| `00003076501103_MapSwitchBase.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `76f8861793f099c08644bb01631034da` | Factory Binary Firmware Dump |
| `00003076501103_original.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `8b9573bf5009b1e4d65ee3391848b28b` | Factory Binary Firmware Dump |
| `00003076501D02.xdf` | **2015–2019 (Gen 1)** | 1.44 MB | `e8d52842acbb00f1a4f6dbb05173e287` | TunerPro Binary Definition Map |
| `00003076501D02_MapSwitchBase.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `c759b8a34de0f24a5dddaed493f8851a` | Factory Binary Firmware Dump |
| `00003076501D02_original.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `707e5620335e88155cf16fb11924b354` | Factory Binary Firmware Dump |
| `000030765A3205.xdf` | **2015–2019 (Gen 1)** | 1.42 MB | `9045002b8d2935ea3ca96319c86b24e7` | TunerPro Binary Definition Map |
| `000030765A3C06.xdf` | **2015–2019 (Gen 1)** | 1.43 MB | `18b7bdbda2628b943b0950d03064e022` | TunerPro Binary Definition Map |
| `000030765A3C06_MapSwitchBase.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `e6ccbc87ad6bfc132e6d7e40529dd83f` | Factory Binary Firmware Dump |
| `000030765A3C06_original.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `337685cc630cd3b2170fdace8d3eea80` | Factory Binary Firmware Dump |
| `000030765A5005.xdf` | **2015–2019 (Gen 1)** | 1.50 MB | `37e94e15a37afe7d6b693eb2743ce0a2` | TunerPro Binary Definition Map |
| `00003081501102.xdf` | **2015–2019 (Gen 1)** | 1.42 MB | `3110580438b22b045162e30175492b0f` | TunerPro Binary Definition Map |
| `00003081501102_MapSwitchBase.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `d361517f6421e448f0213c4a09805db7` | Factory Binary Firmware Dump |
| `00003081501102_original.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `bcb970a18d374f84ba2233b8a1778892` | Factory Binary Firmware Dump |
| `00003081501D04.xdf` | **2015–2019 (Gen 1)** | 1.42 MB | `f517518bb78c841b01ff9bc14cb445d0` | TunerPro Binary Definition Map |
| `00003081501D04_MapSwitchBase.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `3d124aaa145b1bb8dda7c04d9b8a4421` | Factory Binary Firmware Dump |
| `00003081501D04_original.bin` | **2015–2019 (Gen 1)** | 7.50 MB | `dad0c5753740123a16ebe8e1014082bd` | Factory Binary Firmware Dump |
| `00005D55289606.xdf` | **2019–2026 (Gen 2)** | 1.70 MB | `2606c69f1a2dc6580809f3950d40e517` | TunerPro Binary Definition Map |
| `00005D55289606_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `bcae1f9b2c9ce546f68a5b1405f8e0a0` | Factory Binary Firmware Dump |
| `00005D55289606_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `e443aa6005f91b68731985e3e8c572f1` | Factory Binary Firmware Dump |
| `00005D5528AA06.xdf` | **2019–2026 (Gen 2)** | 1.71 MB | `1db2be013ffd670a067a0e3dd4d0b337` | TunerPro Binary Definition Map |
| `00005D5528AA06_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `da41f76f2f36257fc58b3e02c0b0d818` | Factory Binary Firmware Dump |
| `00005D5528AA06_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `3b901ecad128789e7a6cff0042ca9ead` | Factory Binary Firmware Dump |
| `00005D5528B405.xdf` | **2019–2026 (Gen 2)** | 1.70 MB | `ef069ae74c531526780999ca4b326e47` | TunerPro Binary Definition Map |
| `00005D5528B405_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `00df17663920b24be29d92ec29cc0bc6` | Factory Binary Firmware Dump |
| `00005D5528B405_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `48159e2bd2f335f0ad844a09fe0969ff` | Factory Binary Firmware Dump |
| `00005D5528BE07.xdf` | **2019–2026 (Gen 2)** | 1.70 MB | `ef069ae74c531526780999ca4b326e47` | TunerPro Binary Definition Map |
| `00005D5528BE07_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `94e8a84ecb240da9688bdb4803f789e8` | Factory Binary Firmware Dump |
| `00005D5528BE07_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `7a2dd9eb1af5bd2bcbb766204985e11e` | Factory Binary Firmware Dump |
| `00005D5528BE09.xdf` | **2019–2026 (Gen 2)** | 1.70 MB | `ef069ae74c531526780999ca4b326e47` | TunerPro Binary Definition Map |
| `00005D5528BE09_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `63ad8711bbf76b3baadd7aca492c676b` | Factory Binary Firmware Dump |
| `00005D5528BE09_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `72f163fb317174de4a9db9351c8516c2` | Factory Binary Firmware Dump |
| `00005D55327806.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `dd9c005e9b973ce406026904cdb4b489` | TunerPro Binary Definition Map |
| `00005D55327806_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `eb169faacb5e69b0f8efee672c580c77` | Factory Binary Firmware Dump |
| `00005D55327806_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `27cf187aff1c1d10bec4f8a91b2763d3` | Factory Binary Firmware Dump |
| `00005D55328C05.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `86d77e3a4b0f4f9135c2969bc2cb242c` | TunerPro Binary Definition Map |
| `00005D55328C05_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `603d1399f3b5685a9fcc6de6dd80e286` | Factory Binary Firmware Dump |
| `00005D55328C05_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `bb03193cd48a25a6eb5013c592347850` | Factory Binary Firmware Dump |
| `00005D55329606.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `38b04697ac3b80cf462452cd32533af3` | TunerPro Binary Definition Map |
| `00005D55329606_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `64c4aefd5f1f90a7a03ce17b8a6180e8` | Factory Binary Firmware Dump |
| `00005D55329606_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `d448d38c86fe2a6ad5c84f49834e2af3` | Factory Binary Firmware Dump |
| `00005D5532BE07.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `bd266e23c5fe5051788a55010f451d91` | TunerPro Binary Definition Map |
| `00005D5532BE07_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `f0f53b1e0f12d9a37b84640620ba354b` | Factory Binary Firmware Dump |
| `00005D5532BE07_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `4036d39239c36d8efc6ffe447ff70192` | Factory Binary Firmware Dump |
| `00005D5532BE09.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `bd266e23c5fe5051788a55010f451d91` | TunerPro Binary Definition Map |
| `00005D5532BE09_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `04bbe85a5ceb658e41e47b6112938e32` | Factory Binary Firmware Dump |
| `00005D5532BE09_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `5c3c0b053b7e63c42cc4b92338663e79` | Factory Binary Firmware Dump |
| `00005D5532C808.xdf` | **2019–2026 (Gen 2)** | 1.88 MB | `1c057ee57ee29bcf5002115a8e133568` | TunerPro Binary Definition Map |
| `00005D5532C808_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `d8ae396f6acc2b4a348509d01b13de93` | Factory Binary Firmware Dump |
| `00005D5532DC05.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `aa596bfa3a9bb8888db0744f2b274eda` | TunerPro Binary Definition Map |
| `00005D5532DC05_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `ed8777cea732f4c6d31a171aa865add2` | Factory Binary Firmware Dump |
| `00005D5532DC05_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `657ad211f3882daeaca844e0a18d381e` | Factory Binary Firmware Dump |
| `00005D5532E605.xdf` | **2019–2026 (Gen 2)** | 1.58 MB | `e51fe93e536fd585a964ac41dc7c0f0c` | TunerPro Binary Definition Map |
| `00005D553C6405.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `0a1997a922d71bdce2b92a255b59ef19` | TunerPro Binary Definition Map |
| `00005D553C6405_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `eedf841ae7fc23119f7e0e9ab3038e7e` | Factory Binary Firmware Dump |
| `00005D553C6405_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `1b54c4c2d68ebb6b0d5aee4d82fbfa33` | Factory Binary Firmware Dump |
| `00005D553C6405_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `4c5eb075b823569e0c2c288935f2d03b` | Factory Binary Firmware Dump |
| `00005D553C6405_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `cfa22cddc9644c25785218cd4f02076a` | Factory Binary Firmware Dump |
| `00005D553C6E05.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `541630a98964ecdbb6588551fbd830fb` | TunerPro Binary Definition Map |
| `00005D553C6E05_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `c748993b6c1a9683eaaed21a62f467c1` | Factory Binary Firmware Dump |
| `00005D553C6E05_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `d5f692d2fa8e1824b77df5a863058270` | Factory Binary Firmware Dump |
| `00005D553C6E05_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `43c994e260447965d2eac6fdb86d09f8` | Factory Binary Firmware Dump |
| `00005D553C6E05_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `3c274b7e7879fcf0937b7263e5f0de2f` | Factory Binary Firmware Dump |
| `00005D553C7805.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `2567e02866460b1b0e5d08c992ec91f8` | TunerPro Binary Definition Map |
| `00005D553C7805_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `79c2253d11db20b69fb51961e7adea35` | Factory Binary Firmware Dump |
| `00005D553C7805_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `1d31da5608c10a8a8f4a962cf6675d37` | Factory Binary Firmware Dump |
| `00005D553C7807.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `65dc526431f58964ac9e57af5ee8b250` | TunerPro Binary Definition Map |
| `00005D553C7807_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `552d9e3b46e91ca3d66ee58f59564539` | Factory Binary Firmware Dump |
| `00005D553C7807_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `8efbcb2756ea0b8a61eae51789def1cb` | Factory Binary Firmware Dump |
| `00005D553C7807_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `f26a599f70ce5c4e23b1c6cbedea5c9b` | Factory Binary Firmware Dump |
| `00005D553C7807_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `986563d4e25e46a6a929cad2b338b768` | Factory Binary Firmware Dump |
| `00005D553C8207.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `c7052ea46ccf14bb5ae30d8aa2428839` | TunerPro Binary Definition Map |
| `00005D553C8207_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `dd588795d80d39d6ec267dc32628a29c` | Factory Binary Firmware Dump |
| `00005D553C8207_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `34ae1342a9d2857fbcc83cdc7f9c7d93` | Factory Binary Firmware Dump |
| `00005D553C8207_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `35194307097a5d1172953e18af116e2e` | Factory Binary Firmware Dump |
| `00005D553C8207_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `3b9b2fabbec6f09b95b62b7b44aa0099` | Factory Binary Firmware Dump |
| `00005D553C8C05.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `4955e6ed9356635f133a514bf7ffc442` | TunerPro Binary Definition Map |
| `00005D553C8C05_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `e519ba35857f066f4b0294062fd65240` | Factory Binary Firmware Dump |
| `00005D553C8C05_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `ae223b9c51898cb3ef71f2a2b9ff4e3c` | Factory Binary Firmware Dump |
| `00005D553C8C05_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `6ef607b7e12610cf094d281c6dcb0577` | Factory Binary Firmware Dump |
| `00005D553C8C05_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `6c438db1d2c843cd3a72e52105ec541c` | Factory Binary Firmware Dump |
| `00005D553C9607.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `a0cef83fb19ae26bbf039a69556e5cce` | TunerPro Binary Definition Map |
| `00005D553C9607_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `407c477ce2f9605d02eb1a716c5d8405` | Factory Binary Firmware Dump |
| `00005D553C9607_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `73cdea535c3de1e999ee4634f2adcf0a` | Factory Binary Firmware Dump |
| `00005D553C9607_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `8eaa71c582ca8b2126c39eb37baae7a3` | Factory Binary Firmware Dump |
| `00005D553C9607_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `b8a852dbd756ab20ee59059f6db1355d` | Factory Binary Firmware Dump |
| `00005D553CA007.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `1deadce40cc82b7f93b51194d6d4e502` | TunerPro Binary Definition Map |
| `00005D553CA007_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `b66394f0614b6170e73e233db70d9e50` | Factory Binary Firmware Dump |
| `00005D553CA007_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `6d3cb93245433529d6ef83423d3cfe19` | Factory Binary Firmware Dump |
| `00005D553CA007_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `9d833d603fa3806a5ae233c470fe0832` | Factory Binary Firmware Dump |
| `00005D553CA007_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `28278f1d405dcbe458eaa353a26c1c95` | Factory Binary Firmware Dump |
| `00005D553CA009.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `0f7b291f828f06067571bcc35e9a9ed0` | TunerPro Binary Definition Map |
| `00005D553CA009_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `5151be22f7e962b443876ac5983f9000` | Factory Binary Firmware Dump |
| `00005D553CA009_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `ceaf836223a87574be32410f0816a1ce` | Factory Binary Firmware Dump |
| `00005D553CA009_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `17071e48737b3c4e8231f86f6c8c384e` | Factory Binary Firmware Dump |
| `00005D553CA009_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `a4f42e0ba8b3337256a82877c27bbf38` | Factory Binary Firmware Dump |
| `00005D553CAA08.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `fe80923d7a010221b781859fb0de5a7c` | TunerPro Binary Definition Map |
| `00005D553CAA08_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `47aa2b0c4bd952b634711f18157bf87b` | Factory Binary Firmware Dump |
| `00005D553CAA08_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `6e72bdc38724831d93725a51b2a1d8cc` | Factory Binary Firmware Dump |
| `00005D553CAA08_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `615fb8acbaaf9170a23cc0f6ac0bceaa` | Factory Binary Firmware Dump |
| `00005D553CAA08_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `08825ebce1c975e0dd04a082ec132620` | Factory Binary Firmware Dump |
| `00005D553CBE05.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `a734105c05d4c10ebc98c241d480630e` | TunerPro Binary Definition Map |
| `00005D553CBE05_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `84e6659285087cc6be04b9b7c0b29da7` | Factory Binary Firmware Dump |
| `00005D553CBE05_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `7130614befe0d3ec4db767db65f36f92` | Factory Binary Firmware Dump |
| `00005D553CC805.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `d096e6febcd66269d55b059d8ce8016e` | TunerPro Binary Definition Map |
| `00005D553CC805_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `d04ca4f190337aa91e6024587a4ce6e8` | Factory Binary Firmware Dump |
| `00005D553CC805_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `209474e21c23271e03fa553d18e1b7ac` | Factory Binary Firmware Dump |
| `00005D55461E08.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `8c5e755acd721af2617d1853e7437f64` | TunerPro Binary Definition Map |
| `00005D55461E08_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `85838e7af398b6d0a9a80e270c4fa8b1` | Factory Binary Firmware Dump |
| `00005D55461E08_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `e17d573b870fa754b589736ebf8ae6da` | Factory Binary Firmware Dump |
| `00005D55461E08_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `a5ee1a1ca6bb64e8a3788bed299c4612` | Factory Binary Firmware Dump |
| `00005D55461E08_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `3783aa2a3ddfdb69fe070d28fc828bc0` | Factory Binary Firmware Dump |
| `00005D55463208.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `38e08a07946f243c98dff0186574d591` | TunerPro Binary Definition Map |
| `00005D55463208_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `0104cc078d65ab0d757035ee8c243da5` | Factory Binary Firmware Dump |
| `00005D55463208_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `9b22ed383824cf84d1c57eccec5a632e` | Factory Binary Firmware Dump |
| `00005D55463208_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `753ecc208ba78b57a4d1f4a6df3acd1f` | Factory Binary Firmware Dump |
| `00005D55463208_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `f2e187610659079314929c4a9410a25f` | Factory Binary Firmware Dump |
| `00005D55463C07.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `06c021888fea8618b1fd5a5174931d02` | TunerPro Binary Definition Map |
| `00005D55463C07_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `1156da5aacd62ced1c9c00333a2e5cea` | Factory Binary Firmware Dump |
| `00005D55463C07_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `63f9d86f6a1d6268258712392ef9777c` | Factory Binary Firmware Dump |
| `00005D55463C07_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `4ba1bf9407157bfe8362323a380c1333` | Factory Binary Firmware Dump |
| `00005D55463C07_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `0bc03cc09b8b67750528a29fc6762250` | Factory Binary Firmware Dump |
| `00005D55464605.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `a3d80925ab1ecb23f9bb33aad788052e` | TunerPro Binary Definition Map |
| `00005D55464605_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `64742322ee9bbff9ecc8ea906d1c2413` | Factory Binary Firmware Dump |
| `00005D55464605_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `ef26e0f121bdab4eec841b3b69756f2a` | Factory Binary Firmware Dump |
| `00005D55464605_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `d639268274f3838851cb3a1459d500ff` | Factory Binary Firmware Dump |
| `00005D55464605_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `e89eca3866b88cfbc03753da9065a80c` | Factory Binary Firmware Dump |
| `00005D55465005.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `2e3d325c340c0d47acc93ab4e3a195c1` | TunerPro Binary Definition Map |
| `00005D55465005_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `a7aad45a42b87cbeafb9cf0e88456e85` | Factory Binary Firmware Dump |
| `00005D55465005_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `0d8f727d5f0f9d7749f61e5e3e283ab5` | Factory Binary Firmware Dump |
| `00005D55465005_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `e135c32a3f661f39374c28a5892e0b53` | Factory Binary Firmware Dump |
| `00005D55465005_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `50afbc4258e1cee931d3d59446115659` | Factory Binary Firmware Dump |
| `00005D55465A07.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `05c61e85761ab01430379502ee777c4b` | TunerPro Binary Definition Map |
| `00005D55465A07_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `37b54f4333d79fe27a9be2ca0fcbef1f` | Factory Binary Firmware Dump |
| `00005D55465A07_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `7961dae3c1df592fa97ce1459261fb11` | Factory Binary Firmware Dump |
| `00005D55465A07_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `f0959339fa2e5572265adfce9127b957` | Factory Binary Firmware Dump |
| `00005D55465A07_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `1b05e32a8d18da5f4ca3096063425f8d` | Factory Binary Firmware Dump |
| `00005D55465A09.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `05c61e85761ab01430379502ee777c4b` | TunerPro Binary Definition Map |
| `00005D55465A09_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `ce93cfea07134c9c2a03d962d24a1a6d` | Factory Binary Firmware Dump |
| `00005D55465A09_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `69ef92cde1e448446ff7b8162806c0b9` | Factory Binary Firmware Dump |
| `00005D55465A09_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `ad196ead00c6f358743c599e1c9389d2` | Factory Binary Firmware Dump |
| `00005D55465A09_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `c82714a45958935329331f7f02db215e` | Factory Binary Firmware Dump |
| `00005D55466408.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `5e7caaef74f078a8b5f1b4f326c4417b` | TunerPro Binary Definition Map |
| `00005D55466408_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `dcc156e0d4480f3f70e092409a02c4c9` | Factory Binary Firmware Dump |
| `00005D55466408_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `a54a3d65991c0d6cf23ef6e316622179` | Factory Binary Firmware Dump |
| `00005D55466408_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `7bdc27e731e07fc2d1f8e901cd34f0dc` | Factory Binary Firmware Dump |
| `00005D55466408_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `640bad00bdcd8e30166eb37dd1261fe8` | Factory Binary Firmware Dump |
| `00005D55467805.xdf` | **2019–2026 (Gen 2)** | 1.73 MB | `284eebdafcd236c157ebd2af402481f6` | TunerPro Binary Definition Map |
| `00005D55467805_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `523485ea49e6b9e6f29cdbefc021edd6` | Factory Binary Firmware Dump |
| `00005D55467805_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `84de2cf858fe4bc8574b5c0444e3e9dd` | Factory Binary Firmware Dump |
| `00005D55467805_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `94ade113f9eec9bfdbd3a7c369bb0e55` | Factory Binary Firmware Dump |
| `00005D55467805_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `80a8a05927c444074d41cf3a0fd4f511` | Factory Binary Firmware Dump |
| `00005D55468205.xdf` | **2019–2026 (Gen 2)** | 1.72 MB | `3987c3d97ee7798ab3e9f7096f327d31` | TunerPro Binary Definition Map |
| `00005D55468205_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `1fd35ed044721dc97bc19ddefef59cc2` | Factory Binary Firmware Dump |
| `00005D55468205_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `ed34f0b5d988c7e7ffdc4071ca31a1cf` | Factory Binary Firmware Dump |
| `00005D55502807.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `89784df46970f2e58809d14acd2f30b9` | TunerPro Binary Definition Map |
| `00005D55502807_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `17eb6e3b53d02ef46fbb3d11b29e05f4` | Factory Binary Firmware Dump |
| `00005D55502807_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `7c9b840fae034145edeee89f36ec4c71` | Factory Binary Firmware Dump |
| `00005D55503705.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `c4c0fb0166b420cff8a609075cd29cac` | TunerPro Binary Definition Map |
| `00005D55503705_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `1bdee3e13163022a56cb651517996131` | Factory Binary Firmware Dump |
| `00005D55503705_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `74a41c32bfb880e4d82eebed744a867b` | Factory Binary Firmware Dump |
| `00005D55503C05.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `c74438150e19e8e7764636560a69cf38` | TunerPro Binary Definition Map |
| `00005D55503C05_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `108ca678d654469128755ea82b1e4141` | Factory Binary Firmware Dump |
| `00005D55503C05_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `a2fddd30e6d0f8aabd03541bf2d1c059` | Factory Binary Firmware Dump |
| `00005D55504807.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `0fb0ff91bfe36623d4f38fb947b4f57c` | TunerPro Binary Definition Map |
| `00005D55504807_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `6d0d685b0aef0ffcda7f27385c952221` | Factory Binary Firmware Dump |
| `00005D55504807_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `4ffd27545875cca7ac4c56387b48465b` | Factory Binary Firmware Dump |
| `00005D55504809.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `0fb0ff91bfe36623d4f38fb947b4f57c` | TunerPro Binary Definition Map |
| `00005D55504809_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `2dafae850c66d4544e6105c5ec3fcfd5` | Factory Binary Firmware Dump |
| `00005D55504809_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `edfdc5665b9bfa080179273eee110544` | Factory Binary Firmware Dump |
| `00005D5550480C.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `5f5b12db9b55e5315e32209c35c52480` | TunerPro Binary Definition Map |
| `00005D5550480C_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `ab78b5a56ec136371a540bafce65014c` | Factory Binary Firmware Dump |
| `00005D5550480C_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `8dde5a4c9e8af1cf229829c79f6dc834` | Factory Binary Firmware Dump |
| `00005D55505008.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `d62a1fe392c03186c269f06f179d9bc0` | TunerPro Binary Definition Map |
| `00005D55505008_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `51b3fcabcd14a69fa2867765693dcd33` | Factory Binary Firmware Dump |
| `00005D55505008_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `f1b02fa73db4d64c5ec90a98ad9d22a6` | Factory Binary Firmware Dump |
| `00005D55505008_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `dd3ac2266395e48e551bd134b4353298` | Factory Binary Firmware Dump |
| `00005D55505008_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `5e68c98a974b03b8831b3c5887a76ae7` | Factory Binary Firmware Dump |
| `00005D55506405.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `33dbcd18d8976502e73991edaef87399` | TunerPro Binary Definition Map |
| `00005D55506405_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `c33a4dc32af5704253b135bb78c6dacc` | Factory Binary Firmware Dump |
| `00005D55506405_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `35cc73dea4ae494b17bdfa0cc2798f11` | Factory Binary Firmware Dump |
| `00005D55506406.xdf` | **2019–2026 (Gen 2)** | 1.75 MB | `96faeae26d34eb9b10c011dfa4abbcad` | TunerPro Binary Definition Map |
| `00005D55506406_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `7b4503d5a7c775919da6856865208317` | Factory Binary Firmware Dump |
| `00005D55506406_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `3b3ffd1af73b677043f75bf816359710` | Factory Binary Firmware Dump |
| `00005D55508C05.xdf` | **2019–2026 (Gen 2)** | 1.74 MB | `4d3febd06a0d6c91747d5d5c0a14c43f` | TunerPro Binary Definition Map |
| `00005D55508C05_b58o1_MapSwitchBase.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `2986bb69bded56d6b4741989deec5aae` | Factory Binary Firmware Dump |
| `00005D55508C05_b58o1_original.bin` | **2019–2026 (Gen 2)** | 8.00 MB | `6cd968e138fa5809ced11d5b94b1f24e` | Factory Binary Firmware Dump |
| `00007972000505.xdf` | **2015–2026** | 1.46 MB | `c2ffb142d1eafb5b0277aa1c937f04aa` | TunerPro Binary Definition Map |
| `00007972000705.xdf` | **2015–2026** | 1.46 MB | `96f60f893801a8218948135b1affd3a3` | TunerPro Binary Definition Map |
| `00007972000705_original.bin` | **2015–2026** | 7.50 MB | `02e0f6bf5a53cc47169faff717db8054` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
