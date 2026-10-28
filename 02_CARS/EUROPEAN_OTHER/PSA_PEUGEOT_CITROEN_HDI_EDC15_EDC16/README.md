# PSA_PEUGEOT_CITROEN_HDI_EDC15_EDC16 - ECU Calibration Suite

**Repository Path**: `02_CARS/EUROPEAN_OTHER/PSA_PEUGEOT_CITROEN_HDI_EDC15_EDC16`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `190 files` (190 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `PSA_PEUGEOT_CITROEN_HDI_EDC15_EDC16` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `0281001782_1037359041_9634662880.bin` | **2000–2024** | 512.0 KB | `a0f77298798f23d91eb5af9ff4ddd084` | Factory Binary Firmware Dump |
| `0281011634_eep.bin` | **2000–2024** | 8.0 KB | `99e14a1e925a52ae7d80ea3fe9cb74a3` | Factory Binary Firmware Dump |
| `0281011634_flash.bin` | **2000–2024** | 2.00 MB | `80fba83fc038a65ba09d9aa8e9a7dced` | Factory Binary Firmware Dump |
| `213_492.ori` | **2000–2024** | 32.0 KB | `56995d6d95b8f65219d78875f13ee568` | Factory Binary Firmware Dump |
| `306 HDI 0281010163 1037359088 B075WFS.ori` | **2000–2024** | 512.0 KB | `e0835f5debcfa6c664a1e26a403a068a` | Factory Binary Firmware Dump |
| `306.ori` | **2000–2024** | 512.0 KB | `51908c42041c8147874a651fded86c60` | Factory Binary Firmware Dump |
| `5WS40110C-T HW9653447480 SW9648624280.ori` | **2000–2024** | 512.0 KB | `e23255e78d2c606207450649fce9bcbf` | Factory Binary Firmware Dump |
| `5WS40136C-T 380 380.ori` | **2000–2024** | 512.0 KB | `5d173db26166e419cce905689dbb18c0` | Factory Binary Firmware Dump |
| `C5_2_9HZ_0281013872.bin` | **2000–2024** | 2.00 MB | `2747b5050e39db851dde730c55d2be17` | Factory Binary Firmware Dump |
| `CITROEN-ZX-2.0 16V-0261200218-1267357390.ori` | **2000–2024** | 32.0 KB | `71f083253389eb1ea3401ea3fef8cc80` | Factory Binary Firmware Dump |
| `CITROEN-ZX-2.0 16V-0261200218-1267358295.ori` | **2000–2024** | 32.0 KB | `bc60f2bab6d546e26a6c9d53c3537985` | Factory Binary Firmware Dump |
| `CITROEN-ZX-2.0 16V-0261200218-2227355803.ori` | **2000–2024** | 32.0 KB | `51596b7abe45bb862bb4f4057070b5cc` | Factory Binary Firmware Dump |
| `CITROEN_5W40378C-T_HW_9655534080_SW_9663862780_SiD803A.ori` | **2000–2024** | 503.8 KB | `40863a28862530b3c22e13b05022aa56` | Factory Binary Firmware Dump |
| `Citroen AX GTI 1.4 MP31  0261200217-1267357551.ori` | **2000–2024** | 32.0 KB | `bec790964a6b1f023360bf540fcaac0b` | Factory Binary Firmware Dump |
| `Citroen Berlingo 1.6HDI 90HP 1037393468.ori` | **2000–2024** | 2.00 MB | `7b326c996b41883e65246ac6b99ddfe3` | Factory Binary Firmware Dump |
| `Citroen Berlingo 2.0HDI 90HP 5WS40108E-T 9651942080 9647423380.ori` | **2000–2024** | 512.0 KB | `1385de23e22decaf3a5dbf4e7e1f765f` | Factory Binary Firmware Dump |
| `Citroen C2 1.6 VTS 0261208376 369477.ori` | **2000–2024** | 512.0 KB | `54a85d154185a67087ab867d658dba2c` | Factory Binary Firmware Dump |
| `Citroen C3 1.4HDI 68HP 0281012529 1037386117.ori` | **2000–2024** | 2.00 MB | `4754984f683ed9cf8ca5de57c8261969` | Factory Binary Firmware Dump |
| `Citroen C3 1.4HDI 68HP 5WS40285C-T 9660300280 9653451880.ori` | **2000–2024** | 512.0 KB | `36ab6f5a8dd87f45a6aa511aa035e26a` | Factory Binary Firmware Dump |
| `Citroen C3 1.6HDI 90HP 372289 DPF.ori` | **2000–2024** | 2.00 MB | `d24b20805f4f59c37904ada9c012e9a9` | Factory Binary Firmware Dump |
| `Citroen C4 1.6HDI 110HP 0281011629 376755.ori` | **2000–2024** | 2.00 MB | `d389fe7f68a63a69c83cf583d78735f3` | Factory Binary Firmware Dump |
| `Citroen C4 1.6HDI 8v 90HP 376754.ori` | **2000–2024** | 2.00 MB | `2b0abcefa571aabb2d62385d44cbbb93` | Factory Binary Firmware Dump |
| `Citroen C4 2.0HDI 9655534080 5WS40277G-T 9660497480.ori` | **2000–2024** | 2.00 MB | `ad0c4825da2430b66fbfbfab4faf3585` | Factory Binary Firmware Dump |
| `Citroen C5 2.0HDI 0281011524 369508.ori` | **2000–2024** | 512.0 KB | `24d9645b08aaa59288ecd1b6f17dd144` | Factory Binary Firmware Dump |
| `Citroen C5 2.0HDI 110HP  0281010774 353726.ori` | **2000–2024** | 512.0 KB | `3491ee54251a04c258c5b39a97090ce2` | Factory Binary Firmware Dump |
| `Citroen C5 2.0HDI 110HP 0281011340 368212.ori` | **2000–2024** | 512.0 KB | `56e479a23a6c5000b17eb3679b40f30a` | Factory Binary Firmware Dump |
| `Citroen C5 2.0HDI 136HP 5WS40199D-T 9655041480 9656171480.ori` | **2000–2024** | 452.0 KB | `ebbac7a7a1a273d0fe680225f4c9d3d1` | Factory Binary Firmware Dump |
| `Citroen C5 2.2 HDI 133BHP 0281010764 353785.bin` | **2000–2024** | 512.0 KB | `b7489bf827e4a6688b3df0df85a71838` | Factory Binary Firmware Dump |
| `Citroen C5 2.2HDI 128HP 0281011033 364376.ori` | **2000–2024** | 512.0 KB | `dbceced495407f80d24d170aee6ddd59` | Factory Binary Firmware Dump |
| `Citroen C5 2.2HDI 133HP 0281010371 353456.ori` | **2000–2024** | 512.0 KB | `24021e12e73e5e5b8898334f32affd97` | Factory Binary Firmware Dump |
| `Citroen C5 2.2HDI 133HP 0281010641 1037353491.ori` | **2000–2024** | 512.0 KB | `cfa97f18849f9386f0c0720427f42d5b` | Factory Binary Firmware Dump |
| `Citroen C5 2.2HDI 133HP 0281010764 1037353572.ori` | **2000–2024** | 512.0 KB | `126bf0b032e551cab439748d8dd2c908` | Factory Binary Firmware Dump |
| `Citroen C5 2.2HDI 133HP 0281010886 353785.ori` | **2000–2024** | 512.0 KB | `3e1092db8376a5133b667439005fa76c` | Factory Binary Firmware Dump |
| `Citroen C8 2.2HDI 133HP 0281011779 1037375143.ori` | **2000–2024** | 512.0 KB | `d04fa5b79cfdcb4614866f496cbeec43` | Factory Binary Firmware Dump |
| `Citroen C8 2.2HDI 133HP 0281012141 378622.ori` | **2000–2024** | 512.0 KB | `829cf1f86423fb55f0ce84b9d922b771` | Factory Binary Firmware Dump |
| `Citroen Jumper 2.8HDI 127HP 0281010932 363533.ori` | **2000–2024** | 512.0 KB | `289d66afd331cbd42a1a2d89ddea47e1` | Factory Binary Firmware Dump |
| `Citroen Nemo 1.4HDI 1037391713.ori` | **2000–2024** | 2.00 MB | `b9bbe576d8091abfe8b983dd801a7f6b` | Factory Binary Firmware Dump |
| `Citroen Picasso 1.6HDI 90HP 374952.ori` | **2000–2024** | 2.00 MB | `08dfc70bc35e81318c92b6628ea05fd3` | Factory Binary Firmware Dump |
| `Citroen Picasso 2.0HDI 90HP 0281010595 353363.ori` | **2000–2024** | 512.0 KB | `84783c441b5dbc2af8db9296107c3d79` | Factory Binary Firmware Dump |
| `Citroen Xantia 2.0 IAW8P20 162.21.134.ori` | **2000–2024** | 64.0 KB | `b4b0d2f86ccb6cb7d86381afc0774090` | Factory Binary Firmware Dump |
| `Citroen Xhantia 2.0HDI 109HP 0281010029 359131.ori` | **2000–2024** | 512.0 KB | `4f750dd929b31ea5a98bd0fce9ae5c4e` | Factory Binary Firmware Dump |
| `Citroen Xsara 2.0HDI 110HP 0281010550 353310.ori` | **2000–2024** | 512.0 KB | `061604b7d723b8a685d329fe7649f2a1` | Factory Binary Firmware Dump |
| `Citroen Xsara 2.0HDI 90HP 0281010499 353305.ori` | **2000–2024** | 512.0 KB | `5ed6b5b07feb49812fce8329a0ceeaaa` | Factory Binary Firmware Dump |
| `Citroen ZX 1.9 118HP 0261200160 356744.ori` | **2000–2024** | 32.0 KB | `7583681968cbc3b2b4187e1c23c9a5b5` | Factory Binary Firmware Dump |
| `Citroen berlingo 1.6HDI 90HP 96539589 96618137 377715.ori` | **2000–2024** | 2.00 MB | `e0a0361069d4952b0c234d5b03cc41ff` | Factory Binary Firmware Dump |
| `Citroen berlingo 2.0HDI 90HP 5WS40146A-T.ori` | **2000–2024** | 512.0 KB | `910639b1f116eeec3917066f5a98d4ef` | Factory Binary Firmware Dump |
| `Citroen berlingo 2.0HDI 90HP 5WS40146F-T.ori` | **2000–2024** | 512.0 KB | `d328b4d5591344fc374ad05d36ee6969` | Factory Binary Firmware Dump |
| `Citroen berlingo 2.0HDI 90HP HW9647423388 5WS40049C-T SW9659517880.ori` | **2000–2024** | 512.0 KB | `8c64e9243653f5da96f6670c6e713b21` | Factory Binary Firmware Dump |
| `Citroen evasion 2.0HDI 110HP 0281010368 1037353574.ori` | **2000–2024** | 512.0 KB | `f903d1f2a65f3a286d4772274864d3e3` | Factory Binary Firmware Dump |
| `Citroen jumper 2.2HDI 101HP 0281010484 1037363244.ori` | **2000–2024** | 512.0 KB | `abd0bb206b21573ca621fe5bfb5e057a` | Factory Binary Firmware Dump |
| `Citroen picasso 1.6HDI 110HP 377720.ori` | **2000–2024** | 2.00 MB | `c1f1e85881a9f10a0f92174592047d82` | Factory Binary Firmware Dump |
| `Citroen picasso 1.6HDI 90HP 0281011802 371537.ori` | **2000–2024** | 2.00 MB | `74465c2f4c80df6a7259d2739f504c0b` | Factory Binary Firmware Dump |
| `Citroen picasso 2.0HDI 90HP 0281010358 1037353044.ori` | **2000–2024** | 512.0 KB | `5829941631943fecae9e18107c3d1461` | Factory Binary Firmware Dump |
| `Citroen picasso 2.0HDI 90HP 0281011084 364198.ori` | **2000–2024** | 512.0 KB | `4bfb2763daae7ec92963f536335cbfb7` | Factory Binary Firmware Dump |
| `Citroen saxo 1.6 16V 118HP 16225574.ori` | **2000–2024** | 64.0 KB | `037dac1e8eda92f56df318b4a8d7e97e` | Factory Binary Firmware Dump |
| `Citroen saxo 1.6 16v 1AP41 464.ori` | **2000–2024** | 64.0 KB | `a69f51aad0583cda91eb3ef868f48f84` | Factory Binary Firmware Dump |
| `Citroen saxo 1.6i VTS 120HP 0261206214 350812.ori` | **2000–2024** | 256.0 KB | `d9ccacb60dc4390a84c45db2c2f47246` | Factory Binary Firmware Dump |
| `Citroen xanthia 2.0HDI 0281010251 359146.ori` | **2000–2024** | 512.0 KB | `13a7600cd018307cfe85c97522fe8c22` | Factory Binary Firmware Dump |
| `Citroen xantia 2.0HDI 0281010164 359089.ori` | **2000–2024** | 512.0 KB | `fd55ff4834ae59fe57502d2a70627e35` | Factory Binary Firmware Dump |
| `Citroen xantia 2.0HDI 110HP 0281001782 1037359027.ori` | **2000–2024** | 512.0 KB | `74904c41f85df7f2dfaad8d3f6980d43` | Factory Binary Firmware Dump |
| `Citroen xsara 2.0HDI 110HP 0281010499 353305.ori` | **2000–2024** | 512.0 KB | `c2e14437ae4b631e716b1ee9a4854ab8` | Factory Binary Firmware Dump |
| `Citroen xsara 2.0HDI 110HP 0281010962 1037353913.ori` | **2000–2024** | 512.0 KB | `a3f14fcd016306341c9f51fd5151570f` | Factory Binary Firmware Dump |
| `Citroen xsara 2.0HDI 5WS40023D-T.ori` | **2000–2024** | 512.0 KB | `45672f188940f7d8a4a5a4847de71bfd` | Factory Binary Firmware Dump |
| `Citroen xsara 2.0HDI 90HP 0281010595 353363.ori` | **2000–2024** | 512.0 KB | `01cccd9243135313a0e1e9866dbe1d94` | Factory Binary Firmware Dump |
| `Citroen xsara 2.0HDI 90HP 0281010996 353949.ori` | **2000–2024** | 512.0 KB | `8eb6090aa25118e1163e99848bbffd30` | Factory Binary Firmware Dump |
| `Citroen xsara 2.0HDi 90HP 0281010362 353148.ori` | **2000–2024** | 512.0 KB | `79e0e959289ef2f73f73e2659ba19307` | Factory Binary Firmware Dump |
| `Citroen xsara picasso 2.0HDI 90HP 0281010137 1037359162.ori` | **2000–2024** | 512.0 KB | `6ef42b5b5c2497bc290cc05d11734e3f` | Factory Binary Firmware Dump |
| `Citroen xsara picasso 2.0HDI 90HP 0281010750 1037353528.ori` | **2000–2024** | 512.0 KB | `bc88faaa50456e6c875a4899258f8eb9` | Factory Binary Firmware Dump |
| `Flash_bdm.ori` | **2000–2024** | 1.00 MB | `a78043e6e9e5e9bb8cb52d15c5e33e81` | Factory Binary Firmware Dump |
| `JoachimS.ori` | **2000–2024** | 512.0 KB | `8b94f4ad30ddd1f3f6f2dcc11d8a1c96` | Factory Binary Firmware Dump |
| `MPC55x_bdm.ori` | **2000–2024** | 448.2 KB | `15ab190e021102919a3c2712a6de0ab3` | Factory Binary Firmware Dump |
| `P3008_1.6hdi_1037386171 ori.bin` | **2000–2024** | 2.00 MB | `52686d940d7f778aefc3af9c04462768` | Factory Binary Firmware Dump |
| `PEUGEOT 5WS40262B-T HW 9655534080 SW 9660780880 SID803A.ORI` | **2000–2024** | 2.00 MB | `d87e3d14fa3129be8fbec997f10f4aa6` | Factory Binary Firmware Dump |
| `PEUGEOT 5WS40612B-T HW 9661642180 SW 9664626680 SID803A.ORI` | **2000–2024** | 2.00 MB | `2246c745f702d8290208740db62c63bb` | Factory Binary Firmware Dump |
| `PEUGEOT_207_B1600_R4V4T_110kw_xxx_xxx_392034_crc655D7935.ori` | **2000–2024** | 256.0 KB | `b0632461c4ae176fad7415c98d2ad5f0` | Factory Binary Firmware Dump |
| `Pegeot 407 1.6HDI 0281011588 374181.ori` | **2000–2024** | 1.00 MB | `3896b3306d6cd4896eae61c5e7d3d8fe` | Factory Binary Firmware Dump |
| `Peugeot 106 1.4 0261200203 356717.ori` | **2000–2024** | 32.0 KB | `bad93638858d23914d56a4f436cc05d1` | Factory Binary Firmware Dump |
| `Peugeot 106 1.4XSI 0261200203 357243.ori` | **2000–2024** | 32.0 KB | `6654a95fb94446b3afc96a4de19ace35` | Factory Binary Firmware Dump |
| `Peugeot 2.0 HDI 0281010842 353821.ori` | **2000–2024** | 512.0 KB | `7e398a2a1c39d5ca043b020e30769145` | Factory Binary Firmware Dump |
| `Peugeot 205 1.9 GTI 130HP 0261200162 356149.ori` | **2000–2024** | 32.0 KB | `bc630b451cdd1666934d33fe4a46b3dd` | Factory Binary Firmware Dump |
| `Peugeot 206 1.4HDI 68HP 0281010707 363558.ori` | **2000–2024** | 1.00 MB | `03d96f818605b7bafe821ef3cfbb855e` | Factory Binary Firmware Dump |
| `Peugeot 206 1.4HDI 68HP 0281011707 366512.ori` | **2000–2024** | 1.00 MB | `eeeb2061d8097d2e38fd457231bab431` | Factory Binary Firmware Dump |
| `Peugeot 206 1.4HDI 69HP 0080B680 374477.ori` | **2000–2024** | 2.00 MB | `6d8a4dea344678a82d754b7056061284` | Factory Binary Firmware Dump |
| `Peugeot 206 1.4HDI 69HP 0281010707 363160.ori` | **2000–2024** | 1.00 MB | `52f9f84b0e10576315abfc41b20e06f6` | Factory Binary Firmware Dump |
| `Peugeot 206 1.4HDI 90HP 0281011784 371040.ori` | **2000–2024** | 2.00 MB | `445c2c41238b2e1b23c3f05a31617be7` | Factory Binary Firmware Dump |
| `Peugeot 206 1.4i 1AP-81.ori` | **2000–2024** | 64.0 KB | `3e1e3635110cac86429c98297d82215a` | Factory Binary Firmware Dump |
| `Peugeot 206 1.6HDI 110HP 375528.ori` | **2000–2024** | 2.00 MB | `3f9deb7bc4fc36a749a827e855bf6f85` | Factory Binary Firmware Dump |
| `Peugeot 206 1.6i 0261208101 366631.ori` | **2000–2024** | 64.0 KB | `2d29276326ff133ccdf0a4094e885d01` | Factory Binary Firmware Dump |
| `Peugeot 206 1.6i 98HP 0261206942 364124.ori` | **2000–2024** | 64.0 KB | `ddbc562b06dacac62d120487fefdd540` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281001866 359055.ori` | **2000–2024** | 512.0 KB | `9961635b92d5c370f9f4dee4b4241b9c` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281010250 359136.ori` | **2000–2024** | 512.0 KB | `20a317ff20e59cb23eafee50f7f74df2` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281010250 359222.ori` | **2000–2024** | 512.0 KB | `2810a04e4664512b6e39e2cb8f9bdb32` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281010500 353319.ori` | **2000–2024** | 512.0 KB | `2a68384661865c304f1134cc59ff29ee` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281010592 353483.ori` | **2000–2024** | 512.0 KB | `02010d5c8031610052fab3c857848b02` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281010594 353648.ori` | **2000–2024** | 512.0 KB | `d416a281c65502e947efaa61427807f0` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281010594 364196.ori` | **2000–2024** | 512.0 KB | `c688873bef902c4d16964567a05d7b84` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281010767 353735.ori` | **2000–2024** | 512.0 KB | `2cb9059ac88de28654f886e075b805aa` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281011188 364378.ori` | **2000–2024** | 512.0 KB | `b1405d3ef9bc2cb1a86a773f72f37807` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281011525 368453.ori` | **2000–2024** | 512.0 KB | `6ba8b2c8c74887720b3aac103b47456b` | Factory Binary Firmware Dump |
| `Peugeot 206 2.0HDI 90HP 0281011525 374499.ori` | **2000–2024** | 512.0 KB | `800282cd1d868a6ba23d43f52b733b76` | Factory Binary Firmware Dump |
| `Peugeot 207 1.4HDI 68HP SW381875.ori` | **2000–2024** | 2.00 MB | `6eadeccb159549bb7170216b5ffd7ffb` | Factory Binary Firmware Dump |
| `Peugeot 207 1.4HDI 90HP 381875.ori` | **2000–2024** | 2.00 MB | `cb0435581061acaabd77abe634c86f91` | Factory Binary Firmware Dump |
| `Peugeot 207 1.6HDI 110HP 1037379394.ori` | **2000–2024** | 2.00 MB | `99fa150bf748d537d020e7e9a1415736` | Factory Binary Firmware Dump |
| `Peugeot 207 1.6HDI 110HP 1037386112.ori` | **2000–2024** | 2.00 MB | `a2e11a3ba8a7bd74bfca99a1e5e42509` | Factory Binary Firmware Dump |
| `Peugeot 207 RC 1.6 THP 175HP 602 386427.ori` | **2000–2024** | 256.0 KB | `c97e4fe77b1a4932d88df4e5ede3539a` | Factory Binary Firmware Dump |
| `Peugeot 207 THP 1.6 150HP 1037394738.ori` | **2000–2024** | 256.0 KB | `1820821aa9b454f48d3eb9f6cdf78d94` | Factory Binary Firmware Dump |
| `Peugeot 306 0261204495 356916.ori` | **2000–2024** | 256.0 KB | `3e45fdbd0715db5859e3a44b723d49f3` | Factory Binary Firmware Dump |
| `Peugeot 306 1.6 16v 0261204062 355982.ori` | **2000–2024** | 32.0 KB | `d6ec229657fa19564360e1195f1f0e21` | Factory Binary Firmware Dump |
| `Peugeot 306 2.0HDI 90HP 0281010162 359087.ori` | **2000–2024** | 512.0 KB | `e9a4b2a597ca8dc62a46ec6ca426cfa0` | Factory Binary Firmware Dump |
| `Peugeot 306 2.0HDI 90HP 0281010592 353483.ori` | **2000–2024** | 512.0 KB | `bf1312745c274531339e2f1c1884b732` | Factory Binary Firmware Dump |
| `Peugeot 307 1.4HDI 90HP 0281011390 1037363557.ori` | **2000–2024** | 1.00 MB | `fc48906b826701209abcd06f5af5638f` | Factory Binary Firmware Dump |
| `Peugeot 307 1.6HDI 110HP 0281012465 375963.ori` | **2000–2024** | 2.00 MB | `1ab9aacaeec450f893d414e488abce22` | Factory Binary Firmware Dump |
| `Peugeot 307 1.6HDI 110HP 1037381884.ori` | **2000–2024** | 2.00 MB | `9e5c2a3971255d193921bb45e2f64021` | Factory Binary Firmware Dump |
| `Peugeot 307 1.6HDI 110HP 386115.ori` | **2000–2024** | 2.00 MB | `18f8c65057c2990466318b70e61acfeb` | Factory Binary Firmware Dump |
| `Peugeot 307 1.6HDI 90HP 1037375526.ori` | **2000–2024** | 2.00 MB | `1f538bbe23fa9f7f630495b2b8d73dc5` | Factory Binary Firmware Dump |
| `Peugeot 307 1.6HDI 90HP 380727.ori` | **2000–2024** | 2.00 MB | `0642ecc1ea0a3a41642f96536e8aa8ad` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0 HDI 110HP 028101124810 369509.ori` | **2000–2024** | 512.0 KB | `512aeec40e5aca070ace6101af4c282f` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 110HP 0281010779 353725.ori` | **2000–2024** | 512.0 KB | `c66d3ea08f018b429a1bae27d50b69b8` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 110HP 0281010935 364448.ori` | **2000–2024** | 512.0 KB | `2dda2657b30db9d5ef621c4d2c0c7828` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 110HP 0281011081 364193.ori` | **2000–2024** | 512.0 KB | `b29dd475972a5d96faa9f4b64fdc81d3` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 110HP 0281014019 386313.ori` | **2000–2024** | 512.0 KB | `ffa322ebefaaa47479866a4dfd5242d6` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 0281010163 359088.ori` | **2000–2024** | 512.0 KB | `9c33ec85f816a15af6fd033fd88ab37d` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 0281010249 359145.ori` | **2000–2024** | 512.0 KB | `facab0ed8564d38b0773badb128b1343` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 0281010252 359183.ori` | **2000–2024** | 512.0 KB | `446a6ec2cf3459877e45292dc19e71fd` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 0281010935 364309.ori` | **2000–2024** | 512.0 KB | `60d41bafea42a0d2def43e0542d29a87` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 0281011341 371045.ori` | **2000–2024** | 512.0 KB | `ed3e8c958fda4ba74c3c8d01af1e4c0c` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 0281012140 374400.ori` | **2000–2024** | 512.0 KB | `f402dba48b55cf78f0f13f8e492cb6ab` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 5WS40020G-T.ori` | **2000–2024** | 512.0 KB | `36c51820bf4e8b9298cacf5e96fc66be` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 5WS40020GT.ori` | **2000–2024** | 512.0 KB | `e68cf8f5c4941be63e144ec3312463b2` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP 9653205380 5WS40145A-T.ori` | **2000–2024** | 512.0 KB | `9c1c5458d2b48922e3ce760e739fb67d` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI 90HP Siemens 5WS40045B-T.ori` | **2000–2024** | 512.0 KB | `662a396b88e03c02b973a3f3da87cd57` | Factory Binary Firmware Dump |
| `Peugeot 307 2.0HDI-5WS40025D-T.ori` | **2000–2024** | 512.0 KB | `3e92037f33c02337aab0046e5eb1f176` | Factory Binary Firmware Dump |
| `Peugeot 308  1.6HDI 1037393476 .ori` | **2000–2024** | 2.00 MB | `e397b12ea396a5e142f731d976cd2a36` | Factory Binary Firmware Dump |
| `Peugeot 405 1.9 110HP 0261200162 355643.ori` | **2000–2024** | 32.0 KB | `95292111cac38071b43df6b009c7a03c` | Factory Binary Firmware Dump |
| `Peugeot 405 Mi16 19 16V  160bhp 0261200139.bin` | **2000–2024** | 32.0 KB | `a21a0258b15d6af7000b51036fcdf368` | Factory Binary Firmware Dump |
| `Peugeot 405 Mi16 19 16V 148bhp 0261200161.bin` | **2000–2024** | 32.0 KB | `03650196c195a8be47950b9552ef271c` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 0281010033 359065.ori` | **2000–2024** | 512.0 KB | `9745d901a40f981283babd753e46ccfa` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 110HP 0281001977 359082.ori` | **2000–2024** | 512.0 KB | `27e41f1d5577366e201b0e720f8db86a` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 110HP 0281010775 1037353610.ori` | **2000–2024** | 512.0 KB | `b8472717e7b4c770e4ba600b377c4c44` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 110HP 0281011338 1037364408.ori` | **2000–2024** | 512.0 KB | `5bd5d0643751682b305832933c13a84a` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 90HP 0281001978 359083.ori` | **2000–2024** | 512.0 KB | `b1dde5c04a90eab9321fc9ef9e80945f` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 90HP 0281010165 359120.ori` | **2000–2024** | 512.0 KB | `d24b55f8d6bf3b7a826e18576920f145` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 90HP 0281010248 353494.ori` | **2000–2024** | 512.0 KB | `4e29ff3ecdf646fae76189c45981b1d1` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 90HP 0281010248 359169.ori` | **2000–2024** | 512.0 KB | `5b572619e8e8dc7ba25105c338633ad1` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 90HP 0281010361 353047.ori` | **2000–2024** | 512.0 KB | `3972dbc1b5fc47a10b4a53bfea8b0df8` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HDI 90HP 5WS40037D-T.ori` | **2000–2024** | 512.0 KB | `9c4c049b2717caab6c11557f222da3cb` | Factory Binary Firmware Dump |
| `Peugeot 406 2.0HdI 110HP 0281010363 353049.ori` | **2000–2024** | 512.0 KB | `b3f19d82a9daa02e901de0e2e4a75559` | Factory Binary Firmware Dump |
| `Peugeot 406 2.2HDI 133HP 0281010370 353454.ori` | **2000–2024** | 512.0 KB | `c55fe0ca08ad775bca9ae9b63c20f875` | Factory Binary Firmware Dump |
| `Peugeot 406 2.2HDI 133HP 0281010772 353609.ori` | **2000–2024** | 512.0 KB | `9a7123d200fa166ba9664e1fdfeef3c4` | Factory Binary Firmware Dump |
| `Peugeot 406 2.2HDI 133HP 0281010772 353776.ori` | **2000–2024** | 512.0 KB | `a0a5b8b461c2ff6e8da0b0204b1d6e38` | Factory Binary Firmware Dump |
| `Peugeot 406 2.2HDI 133HP 0281011446 368979.ori` | **2000–2024** | 512.0 KB | `bbb2e8afcae4753a9422f5a2df24ace9` | Factory Binary Firmware Dump |
| `Peugeot 406 2.2HDI 136HP 0281010597 1037353968.ori` | **2000–2024** | 512.0 KB | `dabd5ca52103d5b851e72b41f4eb12bc` | Factory Binary Firmware Dump |
| `Peugeot 406 2.2HDI 136HP 0281010773 353575.ori` | **2000–2024** | 512.0 KB | `cec6da6fdca2c15f55131f5abc68d738` | Factory Binary Firmware Dump |
| `Peugeot 406 2.2HDI 136HP 02810187710 353776.ori` | **2000–2024** | 512.0 KB | `2de9c0fb7e703812ec6aa23df6e1720f` | Factory Binary Firmware Dump |
| `Peugeot 406HDI 110HP 0281011520 369507.ori` | **2000–2024** | 512.0 KB | `073a2f587e209d068d6b2b75c6304746` | Factory Binary Firmware Dump |
| `Peugeot 407 1.6 HDI 0281011558 371807.ori` | **2000–2024** | 1.00 MB | `d76ec43d3cad2cdff071dc1771357def` | Factory Binary Firmware Dump |
| `Peugeot 407 1.6HDI 110HP 1037377754.ori` | **2000–2024** | 2.00 MB | `f50289aebd8cc9f1c3b9fcae45d3876a` | Factory Binary Firmware Dump |
| `Peugeot 407 1.6HDI 381872.ori` | **2000–2024** | 2.00 MB | `28bfd8a03a477eb3dfd2689b474b668d` | Factory Binary Firmware Dump |
| `Peugeot 407 2.0HDI  5WS40167H-T SID 803 Mpc555.ori` | **2000–2024** | 452.0 KB | `21698577d5667e17a5f2571bd03bf9bc` | Factory Binary Firmware Dump |
| `Peugeot 407 2.0HDI 136HP 5WS40196E-T 9656413080 965504148.ori` | **2000–2024** | 452.0 KB | `ad193532ade25bb76c0a24fd688265fd` | Factory Binary Firmware Dump |
| `Peugeot 407 2.0HDI 136HP 5WS40204ET 9655041480 9658345280.ori` | **2000–2024** | 448.0 KB | `681c7e581c5faa5ed0b83e550aa9916f` | Factory Binary Firmware Dump |
| `Peugeot 407 2.0HDI 5WS40167G-T SID 803 Mpc555.ori` | **2000–2024** | 452.0 KB | `7b408c606ada857f56c0bc0d0a8744e8` | Factory Binary Firmware Dump |
| `Peugeot 407 2.2HDI 170HP 386058.ori` | **2000–2024** | 2.00 MB | `7c05db360e4ead99b53e46436bbcaa30` | Factory Binary Firmware Dump |
| `Peugeot 607 2.2HDI 133HP 0281010567 353453.ori` | **2000–2024** | 512.0 KB | `66464a791d851280987cd1c7463e253b` | Factory Binary Firmware Dump |
| `Peugeot 607 2.2HDI 136HP 0281010765 1037353571.ori` | **2000–2024** | 512.0 KB | `d5488e04e8ff3c06a7c9302408a98007` | Factory Binary Firmware Dump |
| `Peugeot 607 2.2HDI 136HP 0281010765 353778.ori` | **2000–2024** | 512.0 KB | `133538c9d2ce183d0e99d72cbacbcb47` | Factory Binary Firmware Dump |
| `Peugeot 806 2.0HDI 110HP 028101013 359165.ori` | **2000–2024** | 512.0 KB | `ef0c17318a38db7ac8cfc65c18b3259f` | Factory Binary Firmware Dump |
| `Peugeot 807 2.2HDI 128HP 0281011363 368404.ori` | **2000–2024** | 512.0 KB | `54ef5ef1ff454bd231a541620c9552d1` | Factory Binary Firmware Dump |
| `Peugeot Partner 1.6 HDI 90HP 1037393487.ori` | **2000–2024** | 2.00 MB | `bb7da7647f04437910b11e5605c14f95` | Factory Binary Firmware Dump |
| `Peugeot boxer 2.2HDI 101HP 0281010484 1037369278.ori` | **2000–2024** | 512.0 KB | `f3fa0dd495ca9d88cf56d501453355f9` | Factory Binary Firmware Dump |
| `Peugeot expert 2.0HDI 110HP 0281010359 353497.ori` | **2000–2024** | 512.0 KB | `52b5cfb64ae0bd49224c4e05ba2d8c82` | Factory Binary Firmware Dump |
| `Peugeot partner 1037383736.ori` | **2000–2024** | 632.0 KB | `740fcdbf868887fdf93fcdfefbabc2b3` | Factory Binary Firmware Dump |
| `Peugeot partner 2.0HDI 90HP 0281010360 353444.ori` | **2000–2024** | 512.0 KB | `4c19cceeea4acf6b9daf1fdbd8e9a3bb` | Factory Binary Firmware Dump |
| `Peugeot partner 2.0HDI 90HP 5WS40036D-T 9649063480 9644302380.ori` | **2000–2024** | 512.0 KB | `d3d993a72980465d246e17d0c08cf107` | Factory Binary Firmware Dump |
| `Peugeot partner 2.0HDI 90HP 5ws40155c-t 9653577680 9647423380.ori` | **2000–2024** | 512.0 KB | `f07c3638949b680275a7791ac0af6105` | Factory Binary Firmware Dump |
| `Peugeot_405_B1900_R4V4_108kW_0261200161_96027111_1267356020_crc506232A8.ori` | **2000–2024** | 32.0 KB | `74a3ec717a4bba4f80bca9ea692a25ca` | Factory Binary Firmware Dump |
| `Peugeot_406_B3000_V6V4_140kW_0261204234_9622552780_1037356462_crcDE2363F5.ori` | **2000–2024** | 128.0 KB | `05689c318a392524e1a69baec82a3e92` | Factory Binary Firmware Dump |
| `Peugeot_807_D2200_R4V4T_98kW_0281011363_B075WF2S010287_NZGG38H2_1037368404_crcC4F58194.ori` | **2000–2024** | 512.0 KB | `da046a207a7615f8bcfef703704529de` | Factory Binary Firmware Dump |
| `Pug 206 14HDi 1037368866 Stock.bin` | **2000–2024** | 1.00 MB | `a30ca5da671a76da42452a1b8e888779` | Factory Binary Firmware Dump |
| `eeprom_bdm.ori` | **2000–2024** | 4.0 KB | `9095d0218ffa4e48ab0b30598cba3e0a` | Factory Binary Firmware Dump |
| `my hdi read.bin` | **2000–2024** | 512.0 KB | `030e555f7d7e8b068165bfa41df25d94` | Factory Binary Firmware Dump |
| `original.bin` | **2000–2024** | 64.0 KB | `d9fb72763dc6523c018ebe5af7efc0d7` | Factory Binary Firmware Dump |
| `peugeot 206 1.4HDI 68HP 0281011089 368200.ori` | **2000–2024** | 1.00 MB | `57b4fb9ff658d774d916a9c3a830fc50` | Factory Binary Firmware Dump |
| `peugeot-306-2.0hdi90-0281010249-359145.ori` | **2000–2024** | 512.0 KB | `10be011cea713731298f6c37b1966311` | Factory Binary Firmware Dump |
| `peugeot_306_2.0_hdi_90.0_0281001976_359058.bin` | **2000–2024** | 512.0 KB | `fae48a97aca8161831701eb6c788fe2e` | Factory Binary Firmware Dump |
| `peugeot_306_2.0_hdi_90.0_0281010162_359087.bin` | **2000–2024** | 512.0 KB | `e57ee4770701bc10bfac09ab4a6d8043` | Factory Binary Firmware Dump |
| `peugeot_306_2.0_hdi_90.0_0281010249_359145.bin` | **2000–2024** | 512.0 KB | `a1bd2bd97523cbcbdd3456bc47d54690` | Factory Binary Firmware Dump |
| `peugeot_306_2.0_hdi_90.0_0281010362_353148.bin` | **2000–2024** | 512.0 KB | `120f4c838a3ad73fa204b67e01dc7bcf` | Factory Binary Firmware Dump |
| `peugeot_306_2.0_hdi_90.0_0281010500_353319.bin` | **2000–2024** | 512.0 KB | `b1310fe1474381a0de22220fa30e9343` | Factory Binary Firmware Dump |
| `peugeot_306_2.0_hdi_90.0_0281010592_353483.bin` | **2000–2024** | 512.0 KB | `83232965c0fbccf999bd93ebe3ca0856` | Factory Binary Firmware Dump |

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
