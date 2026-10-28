# OFFICIAL_CALIBRATION_PACKAGES - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CIVIC_1_5L_TURBO_L15B/OFFICIAL_CALIBRATION_PACKAGES`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `126 files` (126 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `OFFICIAL_CALIBRATION_PACKAGES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2016–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `37805-5AA-A020-M1.rwd` | **2016–2024** | 2.44 MB | `cd465462b4a55ede7c1ab22f85b42574` | Factory Binary Firmware Dump |
| `37805-5AA-A520-M1.rwd` | **2016–2024** | 2.44 MB | `48348eb09f64dc47b38444edae127b6d` | Factory Binary Firmware Dump |
| `37805-5AA-C020-M1.rwd` | **2016–2024** | 2.44 MB | `1a3e8dc1ab2a3a6465a2cc75342d1cce` | Factory Binary Firmware Dump |
| `37805-5AA-C520-M1.rwd` | **2016–2024** | 2.44 MB | `a22f75e6d14f40d9d81a83d352f0ff26` | Factory Binary Firmware Dump |
| `37805-5AA-C620-M1.rwd` | **2016–2024** | 2.44 MB | `c2aba3c791161709f0e78f37d87697b8` | Factory Binary Firmware Dump |
| `37805-5AA-K070-M1.rwd` | **2016–2024** | 2.44 MB | `d88718a56a10adbb6d20749bd1046213` | Factory Binary Firmware Dump |
| `37805-5AA-K120-M1.rwd` | **2016–2024** | 2.44 MB | `1472549c56cae66543b933064704f838` | Factory Binary Firmware Dump |
| `37805-5AA-K220-M1.rwd` | **2016–2024** | 2.44 MB | `d0b1cec965ccd52fba322be2bb29e23f` | Factory Binary Firmware Dump |
| `37805-5AA-K520-M1.rwd` | **2016–2024** | 2.44 MB | `3ea498935baf8543888924a0239edaca` | Factory Binary Firmware Dump |
| `37805-5AA-K620-M1.rwd` | **2016–2024** | 2.44 MB | `f4cb0b51fcedc4ed9a8660af0644b603` | Factory Binary Firmware Dump |
| `37805-5AA-K720-M1.rwd` | **2016–2024** | 2.44 MB | `c882f10b5f1a02110af2e57f5daf5fcf` | Factory Binary Firmware Dump |
| `37805-5AA-K810-M1.rwd` | **2016–2024** | 2.44 MB | `e520af6fabc090d6d8b6eb5dc3bb5499` | Factory Binary Firmware Dump |
| `37805-5AA-L520-M1.rwd` | **2016–2024** | 2.44 MB | `90e427738fdb376e21edd37d52d9bb5c` | Factory Binary Firmware Dump |
| `37805-5AA-L620-M1.rwd` | **2016–2024** | 2.44 MB | `8b8ce788caf465cc0a2b1d4570fbd056` | Factory Binary Firmware Dump |
| `37805-5AA-M520-M1.rwd` | **2016–2024** | 2.44 MB | `8a2ff83bc1ae10df4311a6933d17c77d` | Factory Binary Firmware Dump |
| `37805-5AA-M610-M1.rwd` | **2016–2024** | 2.44 MB | `266e6fe6420cfb7f48aa2b5c40be2e9f` | Factory Binary Firmware Dump |
| `37805-5AA-M710-M1.rwd` | **2016–2024** | 2.44 MB | `d623d63935653cc587c52ebe97ce93db` | Factory Binary Firmware Dump |
| `37805-5AA-P510-M1.rwd` | **2016–2024** | 2.44 MB | `bef8188adf0fbf12bff83247da59522c` | Factory Binary Firmware Dump |
| `37805-5AA-X610-M1.rwd` | **2016–2024** | 2.44 MB | `bb9b1d86a4ba50ec88ee62eb3592b82e` | Factory Binary Firmware Dump |
| `37805-5AA-X710-M1.rwd` | **2016–2024** | 2.44 MB | `bd3d170358f7e8efe4d92fdff623cf49` | Factory Binary Firmware Dump |
| `37805-5AG-3050-M1.rwd` | **2016–2024** | 2.44 MB | `941e440a34cc77c3f9b88e3355864069` | Factory Binary Firmware Dump |
| `37805-5AG-N510-M1.rwd` | **2016–2024** | 2.44 MB | `ddf473754463aa821f6f789403b5913a` | Factory Binary Firmware Dump |
| `37805-5AG-N710-M1.rwd` | **2016–2024** | 2.44 MB | `43de2833d6f1ef2b969b6441c0d2e1a3` | Factory Binary Firmware Dump |
| `37805-5AG-N810-M1.rwd` | **2016–2024** | 2.44 MB | `463ff02bb1f979255f0ebdc6fab7c912` | Factory Binary Firmware Dump |
| `37805-5AG-P610-M1.rwd` | **2016–2024** | 2.44 MB | `c1258ccd2475c1497fcaa1319c831e80` | Factory Binary Firmware Dump |
| `37805-5AG-P710-M1.rwd` | **2016–2024** | 2.44 MB | `38cbe5f02305ef7fd7f2955c7f7a4ee2` | Factory Binary Firmware Dump |
| `37805-5AG-P830-M1.rwd` | **2016–2024** | 2.44 MB | `13dea46a4654198cd2b5819b9f821d76` | Factory Binary Firmware Dump |
| `37805-5AG-PF10-M1.rwd` | **2016–2024** | 2.44 MB | `3c09282613eb25afa0eec7f4a7df99a1` | Factory Binary Firmware Dump |
| `37805-5AG-PG10-M1.rwd` | **2016–2024** | 2.44 MB | `21858352582393efb250d8a9599a66d0` | Factory Binary Firmware Dump |
| `37805-5AG-Q610-M1.rwd` | **2016–2024** | 2.44 MB | `c631de8a48f00710f3f433ae2e1ea4f6` | Factory Binary Firmware Dump |
| `37805-5AG-Q710-M1.rwd` | **2016–2024** | 2.44 MB | `afe46d8acbc2d9f698a0ca05bfb05742` | Factory Binary Firmware Dump |
| `37805-5AG-Q820-M1.rwd` | **2016–2024** | 2.44 MB | `c11d7822196026af2d9fa88757fb8c88` | Factory Binary Firmware Dump |
| `37805-5AG-QG10-M1.rwd` | **2016–2024** | 2.44 MB | `f86da5e8df3100dfbb76be0cd42e2fb8` | Factory Binary Firmware Dump |
| `37805-5AG-S510-M1.rwd` | **2016–2024** | 2.44 MB | `ae511947ec42f2d95c6667ee2c9f5dc0` | Factory Binary Firmware Dump |
| `37805-5AG-S830-M1.rwd` | **2016–2024** | 2.44 MB | `86b3f90c5cc8de61a4b4aa1320eb786c` | Factory Binary Firmware Dump |
| `37805-5AG-S930-M1.rwd` | **2016–2024** | 2.44 MB | `0f533fde8b5aedf6a2f9c52b475636b5` | Factory Binary Firmware Dump |
| `37805-5AG-SF10-M1.rwd` | **2016–2024** | 2.44 MB | `91134f9d269be0d5d6b2a8c381dcaa1c` | Factory Binary Firmware Dump |
| `37805-5AG-U510-M1.rwd` | **2016–2024** | 2.44 MB | `3eb4440c5d88dce47bd4084779df4775` | Factory Binary Firmware Dump |
| `37805-5AG-U620-M1.rwd` | **2016–2024** | 2.44 MB | `a2d9132df18b717034ecbb81b75088ea` | Factory Binary Firmware Dump |
| `37805-5AG-U710-M1.rwd` | **2016–2024** | 2.44 MB | `a0f1b7ccc024967b1ed232d212ce4902` | Factory Binary Firmware Dump |
| `37805-5AG-U920-M1.rwd` | **2016–2024** | 2.44 MB | `ce2948975eab8b4488412869d6af3da5` | Factory Binary Firmware Dump |
| `37805-5AG-UF10-M1.rwd` | **2016–2024** | 2.44 MB | `2ac40934798a2f97c99f9b8acb3bffaa` | Factory Binary Firmware Dump |
| `37805-5AJ-J620-M1.rwd` | **2016–2024** | 2.44 MB | `ad626e1dbf659fc5b1fd638828546389` | Factory Binary Firmware Dump |
| `37805-5AJ-J820-M1.rwd` | **2016–2024** | 2.44 MB | `688920cf3af8fcf5cd67850f82c9b583` | Factory Binary Firmware Dump |
| `37805-5AM-A050-M1.rwd` | **2016–2024** | 2.44 MB | `2c5e66adc95e5c025603c82135274a82` | Factory Binary Firmware Dump |
| `37805-5AM-A120-M1.rwd` | **2016–2024** | 2.44 MB | `7834da23c28a9b07136ab627e177f48e` | Factory Binary Firmware Dump |
| `37805-5AM-A220-M1.rwd` | **2016–2024** | 2.44 MB | `1df85cb06492ae8cdcdbd8865ee67bab` | Factory Binary Firmware Dump |
| `37805-5AM-C050-M1.rwd` | **2016–2024** | 2.44 MB | `137347f6530ba1750338635c7d26062d` | Factory Binary Firmware Dump |
| `37805-5AM-C120-M1.rwd` | **2016–2024** | 2.44 MB | `586f69b084d3eb463605013b2a988fe1` | Factory Binary Firmware Dump |
| `37805-5AM-C220-M1.rwd` | **2016–2024** | 2.44 MB | `59fb87c9634d1d1848911b268a3faf9b` | Factory Binary Firmware Dump |
| `37805-5AM-K030-M1.rwd` | **2016–2024** | 2.44 MB | `e3e54fff519ec1c1921ceff57afab983` | Factory Binary Firmware Dump |
| `37805-5AM-K130-M1.rwd` | **2016–2024** | 2.44 MB | `5f1d8adfe5512b676b463df4d68b2728` | Factory Binary Firmware Dump |
| `37805-5AM-M030-M1.rwd` | **2016–2024** | 2.44 MB | `5da09eba6c7125e57e3908566f2be206` | Factory Binary Firmware Dump |
| `37805-5AM-M110-M1.rwd` | **2016–2024** | 2.44 MB | `bc03318bc7a7b871ae3ca9e4a3f2292d` | Factory Binary Firmware Dump |
| `37805-5AN-A220-M1.rwd` | **2016–2024** | 2.44 MB | `4d7fc8412145905d4fe45556c0d3126f` | Factory Binary Firmware Dump |
| `37805-5AN-A310-M1.rwd` | **2016–2024** | 2.44 MB | `7a7b6559cd7156e41eca6fe0f060105e` | Factory Binary Firmware Dump |
| `37805-5AN-AF20-M1.rwd` | **2016–2024** | 2.44 MB | `a9338684e1c4ba7a78ab61b22ef4b470` | Factory Binary Firmware Dump |
| `37805-5AN-AG20-M1.rwd` | **2016–2024** | 2.44 MB | `07b882cb38eadbe015532af3b01bbc92` | Factory Binary Firmware Dump |
| `37805-5AN-AH20-M1.rwd` | **2016–2024** | 2.44 MB | `7e96441698bf4e2d195a9ff0d776d5bb` | Factory Binary Firmware Dump |
| `37805-5AN-AJ30-M1.rwd` | **2016–2024** | 2.44 MB | `0a0369848d4cebce0ed21679eacf8cd3` | Factory Binary Firmware Dump |
| `37805-5AN-AK20-M1.rwd` | **2016–2024** | 2.44 MB | `f9c4eb5005254acf152ac9e173c5d0d8` | Factory Binary Firmware Dump |
| `37805-5AN-AL10-M1.rwd` | **2016–2024** | 2.44 MB | `f04cd89de5b8e14a4dec9b21f6f52188` | Factory Binary Firmware Dump |
| `37805-5AN-AR20-M1.rwd` | **2016–2024** | 2.44 MB | `f469ffa872c4120575820f394de6245e` | Factory Binary Firmware Dump |
| `37805-5AN-C420-M1.rwd` | **2016–2024** | 2.44 MB | `632cb9cf45de7975bb81ee26d5d6b4d6` | Factory Binary Firmware Dump |
| `37805-5AN-CA20-M1.rwd` | **2016–2024** | 2.44 MB | `7ff7718c19264cb52554138e8de71da6` | Factory Binary Firmware Dump |
| `37805-5AN-CB10-M1.rwd` | **2016–2024** | 2.44 MB | `45cd1617c04370ee819096dc9c4d3431` | Factory Binary Firmware Dump |
| `37805-5AN-CC10-M1.rwd` | **2016–2024** | 2.44 MB | `536cab12a23dc5dbf8869202890d405f` | Factory Binary Firmware Dump |
| `37805-5AN-CH20-M1.rwd` | **2016–2024** | 2.44 MB | `38652aecc1e5ff462a85d3fa7e84dafd` | Factory Binary Firmware Dump |
| `37805-5AN-CJ10-M1.rwd` | **2016–2024** | 2.44 MB | `fa4689766b3fe98fa4ffd0945099a6ed` | Factory Binary Firmware Dump |
| `37805-5AN-CR10-M1.rwd` | **2016–2024** | 2.44 MB | `a9548563333569ec41e44f3f8db8fb96` | Factory Binary Firmware Dump |
| `37805-5AN-E130-M1.rwd` | **2016–2024** | 2.44 MB | `1dd603e66f0086f992cde4197a5bc3f4` | Factory Binary Firmware Dump |
| `37805-5AN-E220-M1.rwd` | **2016–2024** | 2.44 MB | `709553f3586a9149950b91546aba34e7` | Factory Binary Firmware Dump |
| `37805-5AN-E320-M1.rwd` | **2016–2024** | 2.44 MB | `9d1708c8a7ed31c395b412e41d3d72e9` | Factory Binary Firmware Dump |
| `37805-5AN-E410-M1.rwd` | **2016–2024** | 2.44 MB | `fb29af2e24a5c0e575bab385aefd614e` | Factory Binary Firmware Dump |
| `37805-5AN-E630-M1.rwd` | **2016–2024** | 2.44 MB | `1384be72862f9f44039055549a117e3e` | Factory Binary Firmware Dump |
| `37805-5AN-E720-M1.rwd` | **2016–2024** | 2.44 MB | `f7ce311aee99a8994777cca36b465b21` | Factory Binary Firmware Dump |
| `37805-5AN-E820-M1.rwd` | **2016–2024** | 2.44 MB | `10640f5ae8e29da52b26e700166517a3` | Factory Binary Firmware Dump |
| `37805-5AN-EA10-M1.rwd` | **2016–2024** | 2.44 MB | `cccd8661ddd548e0b4d809c600f5b3a9` | Factory Binary Firmware Dump |
| `37805-5AN-EB30-M1.rwd` | **2016–2024** | 2.44 MB | `392fb4f9f1b67f47605db3eef4dce435` | Factory Binary Firmware Dump |
| `37805-5AN-EC20-M1.rwd` | **2016–2024** | 2.44 MB | `17dada40520dcf50933d04f95f5da0f0` | Factory Binary Firmware Dump |
| `37805-5AN-EK10-M1.rwd` | **2016–2024** | 2.44 MB | `6054af0a70c1cfbe16e8218f1e1ccb50` | Factory Binary Firmware Dump |
| `37805-5AN-G820-M1.rwd` | **2016–2024** | 2.44 MB | `f7861cc2a4e1ac03ea4102eeed0124da` | Factory Binary Firmware Dump |
| `37805-5AN-GJ10-M1.rwd` | **2016–2024** | 2.44 MB | `d168d811a9dec0fda9797c5edc2b38ed` | Factory Binary Firmware Dump |
| `37805-5AN-J120-M1.rwd` | **2016–2024** | 2.44 MB | `f9f3020f91406b37981a22c660054826` | Factory Binary Firmware Dump |
| `37805-5AN-J320-M1.rwd` | **2016–2024** | 2.44 MB | `db4f9328ed25f3875f56056cc8f42339` | Factory Binary Firmware Dump |
| `37805-5AN-J510-M1.rwd` | **2016–2024** | 2.44 MB | `a4e1b3d234c7d93e3d09808e0ef4490c` | Factory Binary Firmware Dump |
| `37805-5AN-J620-M1.rwd` | **2016–2024** | 2.44 MB | `b231630ab3519b6bbd0ba940f97d0d1b` | Factory Binary Firmware Dump |
| `37805-5AN-J820-M1.rwd` | **2016–2024** | 2.44 MB | `8f32401579658bdbe119e9006d3c7c92` | Factory Binary Firmware Dump |
| `37805-5AN-K520-M1.rwd` | **2016–2024** | 2.44 MB | `9b1914f69666b81265e91c80aeb79ca0` | Factory Binary Firmware Dump |
| `378055BA_A140M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `66f6c64908fc8c586fb99ff3467d62c1` | Factory Binary Firmware Dump |
| `378055BA_A160M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `9eb48e15065c3b408454ab7cbf1708c7` | Factory Binary Firmware Dump |
| `378055BA_A640M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `da833a2340fd835ec41976d53e45b243` | Factory Binary Firmware Dump |
| `378055BA_A660M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `8d9e1abad137a89068092c207d593086` | Factory Binary Firmware Dump |
| `378055BA_A740M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `2c3d56c41990584b5d4d8483660c3005` | Factory Binary Firmware Dump |
| `378055BA_A760M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `2d13057e95e72d5b066a36b9b15e4c0b` | Factory Binary Firmware Dump |
| `378055BA_A840M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `1fc9d69819f1f3a40eac9180838cdef6` | Factory Binary Firmware Dump |
| `378055BA_A860M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `1310a44facb09abeee86f0322bda9e60` | Factory Binary Firmware Dump |
| `378055BA_A940M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `3eb84dc53bcfe3610bc3f3eb63c99f77` | Factory Binary Firmware Dump |
| `378055BA_A960M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `7c81558a9a74ec16ffc82c373d1dbec9` | Factory Binary Firmware Dump |
| `378055BA_C140M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `0a007122582a6c96818a60cd5ea6dc4a` | Factory Binary Firmware Dump |
| `378055BA_C160M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `1f30e974379c811073796c9f6f0532b1` | Factory Binary Firmware Dump |
| `378055BA_C240M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `5c1a78d5fb939a86cdcadc530eae0e80` | Factory Binary Firmware Dump |
| `378055BA_C260M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `065d16838ca8650bd858da2768997a82` | Factory Binary Firmware Dump |
| `378055BA_C540M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `440e2d5f47a206b2059874fb990808fd` | Factory Binary Firmware Dump |
| `378055BA_C560M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `b36d687f31372f15d1ced92b2dfaddf6` | Factory Binary Firmware Dump |
| `378055BA_C640M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `101cd6ae64a464919f8ec4fa218bfcd2` | Factory Binary Firmware Dump |
| `378055BA_C660M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `9500cd4d361242a9d12163e252aa96cc` | Factory Binary Firmware Dump |
| `378055BA_C740M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `fd7c6f0f48d30adb2c7f8d8922420f43` | Factory Binary Firmware Dump |
| `378055BA_C760M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `cc5aa2c7a763565f4a405f77eaa01a5d` | Factory Binary Firmware Dump |
| `378055BA_C840M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `623646791a845e302be523905a9c5eff` | Factory Binary Firmware Dump |
| `378055BA_C860M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `6130e030daaea786b91208f68cb56c9d` | Factory Binary Firmware Dump |
| `378055BA_D540M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `d2afa6ece3b9d28e632cd4b53318fcae` | Factory Binary Firmware Dump |
| `378055BA_K040M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `0ac253096a22dd9e9115a186682a5c2a` | Factory Binary Firmware Dump |
| `378055BA_K540M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `c709532d12b126954c54d40688973ea6` | Factory Binary Firmware Dump |
| `378055BA_L640M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `31df5e33fb12096a3c848efbafd6c6d1` | Factory Binary Firmware Dump |
| `378055BA_L660M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `3612e5cc81207aae8cac7d9d0c914f7f` | Factory Binary Firmware Dump |
| `378055BA_L740M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `6b272d7d7d9dfad302267f78399c9aa2` | Factory Binary Firmware Dump |
| `378055BA_L760M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `e3c99afd48d00d89f2b9acb1f2837fe3` | Factory Binary Firmware Dump |
| `378055BA_L840M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `cf77fb5c3313eb83d92defdbf18e0c1a` | Factory Binary Firmware Dump |
| `378055BA_L860M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `abaf4bbdea649000241a486f251c668a` | Factory Binary Firmware Dump |
| `378055BA_L940M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `06f63c407f5406f0097a8ff3f499d963` | Factory Binary Firmware Dump |
| `378055BA_L960M1__A1610291.rwd` | **2016–2024** | 2.44 MB | `d25377ade34b55648acb0fc34fa7bef3` | Factory Binary Firmware Dump |
| `378055BA_X040M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `1ef990ce931ab1588888410b250d1630` | Factory Binary Firmware Dump |
| `378055BA_X540M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `9f8b084c179abd4bbe15d3b361bd47df` | Factory Binary Firmware Dump |
| `378055BA_Y030M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `f575494fcdebb8909466cbb115fca830` | Factory Binary Firmware Dump |
| `378055BA_Y530M1__A1512443.rwd` | **2016–2024** | 2.44 MB | `853a5ab228eb7921617900b43e20bf60` | Factory Binary Firmware Dump |

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
