# OFFICIAL_CALIBRATION_PACKAGES - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/JAZZ_CITY_MOBILIO_BRV_L15/OFFICIAL_CALIBRATION_PACKAGES`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `367 files` (367 binary dumps, 0 definition maps)  

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

* **Rentang Tahun / Model Year**: 2008–2023

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `37805-55A-3050.rwd` | **2008–2023** | 1.94 MB | `5258c2684760d026d2d295f309b887ae` | Factory Binary Firmware Dump |
| `37805-55A-3060.rwd` | **2008–2023** | 1.94 MB | `570425a6d9300ecdeda86869cca2eb1c` | Factory Binary Firmware Dump |
| `37805-55A-3070.rwd` | **2008–2023** | 1.94 MB | `0290e6574043c27f4ff5782fa22f611d` | Factory Binary Firmware Dump |
| `37805-55A-3080.rwd` | **2008–2023** | 1.94 MB | `d6cb90777c0a729e07681bef36a8dfcb` | Factory Binary Firmware Dump |
| `37805-55A-3090.rwd` | **2008–2023** | 1.94 MB | `295cd5c756f95573d91792e3f56bdba3` | Factory Binary Firmware Dump |
| `37805-55A-4050.rwd` | **2008–2023** | 1.94 MB | `9befbcf79c7534046b3d770eadd5132c` | Factory Binary Firmware Dump |
| `37805-55A-4060.rwd` | **2008–2023** | 1.94 MB | `5cae4df399b8c7a08ade651368afd425` | Factory Binary Firmware Dump |
| `37805-55A-4070.rwd` | **2008–2023** | 1.94 MB | `2731763a4650ad34ed93ce772321c779` | Factory Binary Firmware Dump |
| `37805-55A-4080.rwd` | **2008–2023** | 1.94 MB | `0bd4ac54179c525d5aa3dd47dde15f6a` | Factory Binary Firmware Dump |
| `37805-55A-4090.rwd` | **2008–2023** | 1.94 MB | `950922faadce79cc47ef67043896d2c9` | Factory Binary Firmware Dump |
| `37805-55A-5050.rwd` | **2008–2023** | 1.94 MB | `ffaa137e682d7557cb732555dc6bc4bc` | Factory Binary Firmware Dump |
| `37805-55A-5060.rwd` | **2008–2023** | 1.94 MB | `ea7a66f5c9e7b86bd797f9062790f39f` | Factory Binary Firmware Dump |
| `37805-55A-5070.rwd` | **2008–2023** | 1.94 MB | `b36b49d144490b26b587cb309b541d3d` | Factory Binary Firmware Dump |
| `37805-55A-5080.rwd` | **2008–2023** | 1.94 MB | `456adf7a82d9dc21112aa6e3228ebb86` | Factory Binary Firmware Dump |
| `37805-55A-5090.rwd` | **2008–2023** | 1.94 MB | `2fad62c735ac69ba10066685faa8335f` | Factory Binary Firmware Dump |
| `37805-55A-F130-M1.rwd` | **2008–2023** | 1.94 MB | `5cf5df1a33a4503e97bd16a069005cfd` | Factory Binary Firmware Dump |
| `37805-55A-K710-M1.rwd` | **2008–2023** | 1.94 MB | `dd99c4e41b1323e7454800c1dd2cd9ee` | Factory Binary Firmware Dump |
| `37805-55A-Q020-M1.rwd` | **2008–2023** | 1.94 MB | `18fa070eaf05c9fcb9950005341a670e` | Factory Binary Firmware Dump |
| `37805-55A-Z020-M1.rwd` | **2008–2023** | 1.94 MB | `9feab4aa201133ab62f1de1bc0f5204f` | Factory Binary Firmware Dump |
| `37805-55A-Z120-M1.rwd` | **2008–2023** | 1.94 MB | `02c3b1bc6ee418ea548472778282ae82` | Factory Binary Firmware Dump |
| `37805-55D-M050-M8.rwd` | **2008–2023** | 1.00 MB | `37f3035735aefb6e9cef7241d1b61385` | Factory Binary Firmware Dump |
| `37805-55D-M060-M8.rwd` | **2008–2023** | 1.00 MB | `2551d42f1a6a17339ab88d71be1a59f9` | Factory Binary Firmware Dump |
| `37805-55D-M540-M8.rwd` | **2008–2023** | 1.00 MB | `5c33879992bcf4f7fbf143d4e981e131` | Factory Binary Firmware Dump |
| `37805-55D-M550-M8.rwd` | **2008–2023** | 1.00 MB | `b4fe3e98919d0b33e3bf3b37d3773bcc` | Factory Binary Firmware Dump |
| `37805-55F-3050.rwd` | **2008–2023** | 1.94 MB | `183818a14e78c7f0d7f1b7195a747dc1` | Factory Binary Firmware Dump |
| `37805-55F-3060.rwd` | **2008–2023** | 1.94 MB | `0cac786c12624d2d30dc6ddaee11799c` | Factory Binary Firmware Dump |
| `37805-55F-3070.rwd` | **2008–2023** | 1.94 MB | `85fd15f73acaf97ea3f402cd051d6a58` | Factory Binary Firmware Dump |
| `37805-55F-Z030-M1.rwd` | **2008–2023** | 1.94 MB | `d983500d27d095c9a2748c91c7f0f244` | Factory Binary Firmware Dump |
| `37805-58R-T530-M1.rwd` | **2008–2023** | 1.94 MB | `8117b29a6a0ecf6c60b21c4c33cc3687` | Factory Binary Firmware Dump |
| `37805-58R-T730-M1.rwd` | **2008–2023** | 1.94 MB | `056fdba40269486a7c166002f1fb02a9` | Factory Binary Firmware Dump |
| `37805-58R-U550-M1.rwd` | **2008–2023** | 1.94 MB | `b5e1f27210b88e54fbf35de77d2d7ba2` | Factory Binary Firmware Dump |
| `37805-58R-U630-M1.rwd` | **2008–2023** | 1.94 MB | `6fc8c2def2c76bc9dbcb9bb25a0d00a7` | Factory Binary Firmware Dump |
| `37805-58R-Z540-M1.rwd` | **2008–2023** | 1.94 MB | `f7c40857101aee8aabe3072925350ad3` | Factory Binary Firmware Dump |
| `37805-5A4-H540-M1.rwd` | **2008–2023** | 1.94 MB | `94391e92b4cda3691c4fde5645c2a905` | Factory Binary Firmware Dump |
| `37805-5A4-H640-M1.rwd` | **2008–2023** | 1.94 MB | `65a3c97e5259201ce332fdebb63cec6f` | Factory Binary Firmware Dump |
| `37805-5EA-K030-M1.rwd` | **2008–2023** | 1.94 MB | `7aff73e8d7b9aa2a1d6ae9ea25ca5616` | Factory Binary Firmware Dump |
| `37805-5EA-K220-M1.rwd` | **2008–2023** | 1.94 MB | `bc876248c97334d136abeea6e31fc847` | Factory Binary Firmware Dump |
| `37805-5EA-K540-M1.rwd` | **2008–2023** | 1.94 MB | `74381b415b11d41acca69998f9076865` | Factory Binary Firmware Dump |
| `37805-RB0-3050.RWD` | **2008–2023** | 992.2 KB | `92b61af6785d203adb766d246c9a6fae` | Factory Binary Firmware Dump |
| `37805-RB0-4050-M1.RWD` | **2008–2023** | 992.1 KB | `b5ecc031aadd7dc1610aa741d0fd5412` | Factory Binary Firmware Dump |
| `37805-RB0-9630-M1.rwd` | **2008–2023** | 992.1 KB | `e41cbe6cc1166c3b78be0b6ca37a6fdc` | Factory Binary Firmware Dump |
| `37805-RB0-9660-M1.rwd` | **2008–2023** | 992.1 KB | `c000c3e85b0cdabd89bce76ff4ef9893` | Factory Binary Firmware Dump |
| `37805-RB0-E030-M1.rwd` | **2008–2023** | 992.1 KB | `2277c6b49f6c70af3f1a20300c5ff2f9` | Factory Binary Firmware Dump |
| `37805-RB0-E040-M1.rwd` | **2008–2023** | 992.1 KB | `553fdf3b9b38eaed5d1b7adb02638e2a` | Factory Binary Firmware Dump |
| `37805-RB0-E130-M1.rwd` | **2008–2023** | 992.1 KB | `15fa0f126a3f04a360cbbe5d85f33d11` | Factory Binary Firmware Dump |
| `37805-RB0-E140-M1.rwd` | **2008–2023** | 992.1 KB | `359caa74b3b06574036bca1febc61829` | Factory Binary Firmware Dump |
| `37805-RB0-E170-M1.rwd` | **2008–2023** | 992.1 KB | `76cab3dedcb527c0f4553e244f4f57a3` | Factory Binary Firmware Dump |
| `37805-RB0-E340-M1.rwd` | **2008–2023** | 992.1 KB | `c94d90e58b3990ca40acfd7492e0c1b3` | Factory Binary Firmware Dump |
| `37805-RB0-E720-M1.rwd` | **2008–2023** | 992.1 KB | `272df43a82e0b211bc16645e1f297de3` | Factory Binary Firmware Dump |
| `37805-RB0-J030-M1.rwd` | **2008–2023** | 992.1 KB | `bb41ad49db8172b9c637aac8046acbea` | Factory Binary Firmware Dump |
| `37805-RB0-J660-M1.rwd` | **2008–2023** | 992.2 KB | `536aeb00b3a714e243a5e1dcf42a81eb` | Factory Binary Firmware Dump |
| `37805-RB0-J690-M1.rwd` | **2008–2023** | 992.1 KB | `35a9fccb33537dbd4caca9d93027f417` | Factory Binary Firmware Dump |
| `37805-RB0-J760-M1.rwd` | **2008–2023** | 992.2 KB | `cc33814b958c78e8450b233e48a7f366` | Factory Binary Firmware Dump |
| `37805-RB0-J790-M1.rwd` | **2008–2023** | 992.1 KB | `ed694541c633b13c542fae5e9587fa01` | Factory Binary Firmware Dump |
| `37805-RB0-J830-M1.rwd` | **2008–2023** | 992.1 KB | `9fb9e6d352948d7b4dc7b08cfb034301` | Factory Binary Firmware Dump |
| `37805-RB0-T020-M1.rwd` | **2008–2023** | 992.1 KB | `0805640cf1fe570365b2ed243d4147d7` | Factory Binary Firmware Dump |
| `37805-RB0-T520-M1.rwd` | **2008–2023** | 992.1 KB | `f238bd0b0e616d3e37874449dc41b573` | Factory Binary Firmware Dump |
| `3780555D_M070M8__A1710469.rwd` | **2008–2023** | 1.00 MB | `2a814682eeb66909d7633342719a3fd1` | Factory Binary Firmware Dump |
| `3780555D_M560M8__A1710469.rwd` | **2008–2023** | 1.00 MB | `01f66a376b5532efdc984e19dfd1d932` | Factory Binary Firmware Dump |
| `3780558R_E050M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `2ef1fc492583d138fe7139d713142e99` | Factory Binary Firmware Dump |
| `3780558R_E060M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `f99d7fff02e8bb61aed3ce941dfd1fa0` | Factory Binary Firmware Dump |
| `3780558R_E150M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `b707a38d8f89f33b93fbe0fbc5ab47fb` | Factory Binary Firmware Dump |
| `3780558R_E160M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `ff6c385585c53d4b87f15b55d204775f` | Factory Binary Firmware Dump |
| `3780558R_E350M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `82ccc040ee759b875475b238ef91b731` | Factory Binary Firmware Dump |
| `3780558R_E360M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `d53931b1f013bbc85744d7984702ed61` | Factory Binary Firmware Dump |
| `3780558R_E550M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `e6b5299bd7146dfddbc9ecfd2c13500f` | Factory Binary Firmware Dump |
| `3780558R_E560M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `65a632ea4a2ca3824081d1f583d917b7` | Factory Binary Firmware Dump |
| `3780558R_E650M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `20c32ea8d7c65f76e9a0ffcbcd668aaa` | Factory Binary Firmware Dump |
| `3780558R_E660M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `b98f413de6b7009c2a3c825889f97498` | Factory Binary Firmware Dump |
| `3780558R_E730M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `42e21995c7e741f2157d6c54e9c6f6b6` | Factory Binary Firmware Dump |
| `3780558R_E740M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `72b84741827fea885cacbdf26610cb15` | Factory Binary Firmware Dump |
| `3780558R_E850M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `103d67bdc32a2eacb22debe643d46826` | Factory Binary Firmware Dump |
| `3780558R_E860M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `69dbf5c135f5b8095daf95589b9f2209` | Factory Binary Firmware Dump |
| `3780558R_G030M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `7061796192560d61c8cbf3d5af501382` | Factory Binary Firmware Dump |
| `3780558R_G130M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `49cd9e0e1679a5e6c159579ff1a45d6f` | Factory Binary Firmware Dump |
| `3780558R_G330M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `e0ed49b29be5a57f299c75c616115c37` | Factory Binary Firmware Dump |
| `3780558R_G540M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `bc6fdfc9ff6e2bfa44609aafaf3f510b` | Factory Binary Firmware Dump |
| `3780558R_G640M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `8685003083fdf2bfbf0191ea0f42480a` | Factory Binary Firmware Dump |
| `3780558R_G740M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `01499f14f5c9f89be9f73af321d0dfae` | Factory Binary Firmware Dump |
| `3780558R_G840M1__A1901008.rwd` | **2008–2023** | 1.94 MB | `44de0c8a45beec4ba9fb76567c6644cd` | Factory Binary Firmware Dump |
| `3780558R_T540M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `582161cf2bbbd85abcf5c9dfd9bd5298` | Factory Binary Firmware Dump |
| `3780558R_T740M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `c0457240414c093210ad81eea44f908a` | Factory Binary Firmware Dump |
| `3780558R_U560M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `1c0e5cc37086e66c5ce893fe7ee176e2` | Factory Binary Firmware Dump |
| `3780558R_U640M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `6974cbcad1f21ed0d9739fb5d7eea380` | Factory Binary Firmware Dump |
| `3780558R_Z550M1__A1710292.rwd` | **2008–2023** | 1.94 MB | `4db35e1016b8c18ef2c1827b56f266b9` | Factory Binary Firmware Dump |
| `378055A0_A550M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `f86dfba0d8f9c694b07327fe9e8fbf19` | Factory Binary Firmware Dump |
| `378055A0_A650M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `fde587abaa388b6ecbfdce1a81642a9e` | Factory Binary Firmware Dump |
| `378055A0_A750M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `3e36ffe087bf8ecdd4132a009fa0ffa3` | Factory Binary Firmware Dump |
| `378055A0_A850M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `f85458e1221d868ea351cd284252a235` | Factory Binary Firmware Dump |
| `378055A0_B250M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `ad1a779687ab8cc7a13a2b15558e98fa` | Factory Binary Firmware Dump |
| `378055A0_B350M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `d5f95d15eadcd395bbe5424db40208e6` | Factory Binary Firmware Dump |
| `378055A0_B450M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `3c9317a96bb1e95119485021d4d24b0c` | Factory Binary Firmware Dump |
| `378055A0_B550M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `7440ff098a9941481951a087121fb0df` | Factory Binary Firmware Dump |
| `378055A0_B650M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `7fd9fb1a99484296cf01bfdfd75b59ca` | Factory Binary Firmware Dump |
| `378055A0_B750M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `e1f50f2d7db5d7af3daf6d1c2216651a` | Factory Binary Firmware Dump |
| `378055A0_B850M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `112497e5041c8b2eae79bb9017635a26` | Factory Binary Firmware Dump |
| `378055A0_B950M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `0db3dd4d0b8bee5f8bb4143df82558d9` | Factory Binary Firmware Dump |
| `378055A0_C050M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `18dcf5ac1d7e0dc1b8e13fd7efd64451` | Factory Binary Firmware Dump |
| `378055A0_C150M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `872b048e8c854cc97274cbfbedf518ef` | Factory Binary Firmware Dump |
| `378055A0_C560M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `d33be602140ca23b24efccc7e8a80bc1` | Factory Binary Firmware Dump |
| `378055A0_C660M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `3a74b5aeea8d9ce0a20b8d41e38d49e2` | Factory Binary Firmware Dump |
| `378055A0_C760M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `45f383c5291df683e1e1cade8010cea6` | Factory Binary Firmware Dump |
| `378055A0_C860M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `8815bb9696888085df2c20de0c08feb9` | Factory Binary Firmware Dump |
| `378055A0_F540M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `fe5e549f1348823bd36949c176f22fad` | Factory Binary Firmware Dump |
| `378055A0_F630M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `a83f62f54e47537bc0976aac4445d338` | Factory Binary Firmware Dump |
| `378055A0_F730M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `7c7068cf20cec5d80dde5130c57b45ec` | Factory Binary Firmware Dump |
| `378055A0_F840M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `cd5876af79f599bdef48400b613fc49a` | Factory Binary Firmware Dump |
| `378055A0_G250M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `801248a3058224c3c181125ff50d9b21` | Factory Binary Firmware Dump |
| `378055A0_G350M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `be4ead8e9bc150b59943c0414f469dcf` | Factory Binary Firmware Dump |
| `378055A0_G450M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `12ccc186f9488b3c7316f7a555487b91` | Factory Binary Firmware Dump |
| `378055A0_G550M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `102727d5611211dfd18e2f652c26f7ed` | Factory Binary Firmware Dump |
| `378055A0_G650M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `72533722b9d4cb08e14e3dedb87ec21f` | Factory Binary Firmware Dump |
| `378055A0_G750M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `737e835cfdd6869a28e50aa571973a2b` | Factory Binary Firmware Dump |
| `378055A0_G850M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `5d5819237632a1d67a14013d4ed5d06c` | Factory Binary Firmware Dump |
| `378055A0_L050M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `679adf706eef1463e939bf7c1c9b601d` | Factory Binary Firmware Dump |
| `378055A0_L150M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `ea014b5420f34c5a5d4fe2b42082a9a4` | Factory Binary Firmware Dump |
| `378055A0_L240M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `b911bccf1ab7ebc6b2cb75ff6abea1a7` | Factory Binary Firmware Dump |
| `378055A0_L340M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `96719e6712c7ad22abc810166a05bf1f` | Factory Binary Firmware Dump |
| `378055A0_L440M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `b110321fe17c1ba46858fd0eb6ee3796` | Factory Binary Firmware Dump |
| `378055A0_L540M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `d02a4be91cfa4b5aef8030f536bc7cce` | Factory Binary Firmware Dump |
| `378055A0_L640M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `2fff4f6dba0fe0ac2dd8c144b5b9a1cc` | Factory Binary Firmware Dump |
| `378055A0_L740M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `03c646b7afa2da04620dbd313c4eafaf` | Factory Binary Firmware Dump |
| `378055A0_L840M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `01ba5e28c87fe28956ebe3b3c3a0ed87` | Factory Binary Firmware Dump |
| `378055A0_L940M1__A1602465.rwd` | **2008–2023** | 1.94 MB | `fd20e9ef101362efc7305295dd98d28a` | Factory Binary Firmware Dump |
| `378055A0_X740M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `be1ef09865306796dde2f0e58d11cde7` | Factory Binary Firmware Dump |
| `378055A0_X840M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `47c61bddd2b511bfe9cd9b62ed5c45e3` | Factory Binary Firmware Dump |
| `378055A0_X930M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `e281b56bbcaa4d795378cea4003cae71` | Factory Binary Firmware Dump |
| `378055A0_Y640M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `008f5861379b3d124247e5d076072ed4` | Factory Binary Firmware Dump |
| `378055A0_Y650M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `08d1edfcb20e6ea76937796bda103bb6` | Factory Binary Firmware Dump |
| `378055A1_D550M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `6368c350aaf13e83878e0a9df63966af` | Factory Binary Firmware Dump |
| `378055A1_D650M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `80a582844146ddf3de30a972befbac9c` | Factory Binary Firmware Dump |
| `378055A1_D730M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `489840d1e98afaef27ee32eec2baac4b` | Factory Binary Firmware Dump |
| `378055A1_D830M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `e8a00a1bd64c5ddea17e40529e646671` | Factory Binary Firmware Dump |
| `378055A1_L550M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `ba7b701511beeaccc46ef4ca6c5920c1` | Factory Binary Firmware Dump |
| `378055A1_L560M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `c5b2e4939c2946c35fd8f1969fcf56eb` | Factory Binary Firmware Dump |
| `378055A1_L650M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `1b7f7387e753799a7dcf415c73ece669` | Factory Binary Firmware Dump |
| `378055A1_L660M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `388603a41e58a6dc3f51db82cbecf3d5` | Factory Binary Firmware Dump |
| `378055A1_L750M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `83004e6579f277b26979c9003daf49b7` | Factory Binary Firmware Dump |
| `378055A1_L760M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `51ce8cccc69382ad62d0db073171f6fa` | Factory Binary Firmware Dump |
| `378055A1_L850M1__A1602990.rwd` | **2008–2023** | 1.94 MB | `59d931d4fca19d07f70c3ed56733aec4` | Factory Binary Firmware Dump |
| `378055A1_L860M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `2a4af8f264a88a62ec11fa130aba335c` | Factory Binary Firmware Dump |
| `378055A2_3290____A1510099.rwd` | **2008–2023** | 1.94 MB | `2ba6d722e3c4402e94b66248d1d55fe1` | Factory Binary Firmware Dump |
| `378055A2_4250____A1510099.rwd` | **2008–2023** | 1.94 MB | `134a5171d0f45eafb986d6c0076c37b5` | Factory Binary Firmware Dump |
| `378055A2_4260____A1510099.rwd` | **2008–2023** | 1.94 MB | `7343699839cba6c1e5dbefb315f06118` | Factory Binary Firmware Dump |
| `378055A2_4270____A1510099.rwd` | **2008–2023** | 1.94 MB | `1ab75c5185f1813ed22555a9545e6906` | Factory Binary Firmware Dump |
| `378055A2_C070M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `6fc896d21b79312fc11d44968d964e99` | Factory Binary Firmware Dump |
| `378055A2_C170M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `7bacb44a83aa7011fe824205c805acb0` | Factory Binary Firmware Dump |
| `378055A2_G020M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `dfdd296e406a128c20526c7a9d39544f` | Factory Binary Firmware Dump |
| `378055A2_G120M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `9cb61ab66bfb0aeae6a9afc7b751c131` | Factory Binary Firmware Dump |
| `378055A2_G530M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `1845e7bc6936320e72c43ce4066ea9dc` | Factory Binary Firmware Dump |
| `378055A2_G630M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `015e022716656d946492ecdeaa8b50ed` | Factory Binary Firmware Dump |
| `378055A2_G730M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `a1f3fbff5c040f7b9adad8b8d8fefa6f` | Factory Binary Firmware Dump |
| `378055A2_G830M1__A1510099.rwd` | **2008–2023** | 1.94 MB | `03e94de5116ed3546deaa0989907cdcb` | Factory Binary Firmware Dump |
| `378055A2_X230M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `a471fbed34728ef1cfc498d5878c4574` | Factory Binary Firmware Dump |
| `378055A2_X330M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `7d5b9b8d9f53eef6d6dec6748d131491` | Factory Binary Firmware Dump |
| `378055A2_X430M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `5b62c01230275939d1594a15e3f34eb9` | Factory Binary Firmware Dump |
| `378055A2_Y530M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `b6de8d4f6b3d39908dba5d40837ebce1` | Factory Binary Firmware Dump |
| `378055A3_3250____A1803568.rwd` | **2008–2023** | 1.94 MB | `d74df37d68e43f30dafa406a6232d118` | Factory Binary Firmware Dump |
| `378055A3_3260____A1803568.rwd` | **2008–2023** | 1.94 MB | `ab7598001eb22007bd6d95bbd4d55914` | Factory Binary Firmware Dump |
| `378055A3_3270____A1803568.rwd` | **2008–2023** | 1.94 MB | `7e9ba7ed21c143cbbfd8513dfd54f021` | Factory Binary Firmware Dump |
| `378055A3_3280____A1803568.rwd` | **2008–2023** | 1.94 MB | `c0620a5273060c40e740c1be1fa7d44a` | Factory Binary Firmware Dump |
| `378055A3_L130M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `11132fbec8ebce2b91219d0a2354af73` | Factory Binary Firmware Dump |
| `378055A3_L230M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `94e62feb12089990ec871f5938c32123` | Factory Binary Firmware Dump |
| `378055A3_L330M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `f1cbb1d016f99d7f826d795c7f1da48a` | Factory Binary Firmware Dump |
| `378055A3_L430M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `5e503b0f68531df0d39c7fe56fc93920` | Factory Binary Firmware Dump |
| `378055A4_H440M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `19e2f6b1885c8a0d0a2398465cca6638` | Factory Binary Firmware Dump |
| `378055A4_H580M1__A1605541.rwd` | **2008–2023** | 1.94 MB | `6abfbac500d0d99a8aaf0515057ea3a9` | Factory Binary Firmware Dump |
| `378055A4_H680M1__A1605541.rwd` | **2008–2023** | 1.94 MB | `b96dbfbe3f7619c85833e4864922b263` | Factory Binary Firmware Dump |
| `378055A4_H740M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `e9207530beda45b85ff881ebe9dda771` | Factory Binary Firmware Dump |
| `378055A4_H840M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `2a2e554968b2b332d6b4e3e5937dccf8` | Factory Binary Firmware Dump |
| `378055A4_H940M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `d0f11e8245cf234cdbcf879b3c83c54a` | Factory Binary Firmware Dump |
| `378055A4_R840M1__A1505060.rwd` | **2008–2023** | 1.94 MB | `1171f7c8db3cc8b1db1d23dd19e77f07` | Factory Binary Firmware Dump |
| `378055A4_Y540M1__A1505060.rwd` | **2008–2023** | 1.94 MB | `4ca0f62b7887f1cd74be99997ab8fbfd` | Factory Binary Firmware Dump |
| `378055A4_Y550M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `19a1b15a1f9841f1629c24514c4aba0e` | Factory Binary Firmware Dump |
| `378055A4_Y640M1__A1505060.rwd` | **2008–2023** | 1.94 MB | `e7f6af5e1a588189b99e6390a041a147` | Factory Binary Firmware Dump |
| `378055A4_Y650M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `4f7dfa06a9c23944f58e2d36573f9e3e` | Factory Binary Firmware Dump |
| `378055A4_Y740M1__A1505060.rwd` | **2008–2023** | 1.94 MB | `a785a17a3281235f43e646e47c4f39e1` | Factory Binary Firmware Dump |
| `378055A4_Y750M1__A1803568.rwd` | **2008–2023** | 1.94 MB | `a110ebcecef5ef8600404357d23d8c90` | Factory Binary Firmware Dump |
| `378055AA_A070M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `f0b6826efc17a8e1a02dbd4e95570ffe` | Factory Binary Firmware Dump |
| `378055AA_A080M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `f3e0274fe56cb83efff8e68f5df7289a` | Factory Binary Firmware Dump |
| `378055AA_A120M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `6bb51110077fa7c76867c6c440966811` | Factory Binary Firmware Dump |
| `378055AA_A570M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `6a7fb39449d85c27f0fc2b5115e00ad0` | Factory Binary Firmware Dump |
| `378055AA_A580M1__A1807680.rwd` | **2008–2023** | 2.44 MB | `79897fc8a0a21566ae1e0d602a77b3bb` | Factory Binary Firmware Dump |
| `378055AA_A650M1__A1511062.rwd` | **2008–2023** | 2.44 MB | `64d314ba3b8e01fefbcee1e5fce84bb8` | Factory Binary Firmware Dump |
| `378055AA_A670M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `4cecda3ecc361a29cca1ea3d14d6590d` | Factory Binary Firmware Dump |
| `378055AA_A680M1__A1807680.rwd` | **2008–2023** | 2.44 MB | `c9b3025abff054e5f0076b3dbc7facc7` | Factory Binary Firmware Dump |
| `378055AA_A720M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `7ba592b6231907b01afa290f1d5fbfcf` | Factory Binary Firmware Dump |
| `378055AA_A820M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `c781fe6064dfe618a4b758508cb5a8e2` | Factory Binary Firmware Dump |
| `378055AA_A940M1__A1900417.rwd` | **2008–2023** | 2.44 MB | `e8ed47b401e85869909a65aef05836ab` | Factory Binary Firmware Dump |
| `378055AA_A950M1__A1901190.rwd` | **2008–2023** | 2.44 MB | `3a7b9c662102f5aa285e5a042482881b` | Factory Binary Firmware Dump |
| `378055AA_C070M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `c52f611d26f4d3c14185ab99ea402e5f` | Factory Binary Firmware Dump |
| `378055AA_C080M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `57cb5d8383f8291e72ed9a70d748b7e2` | Factory Binary Firmware Dump |
| `378055AA_C120M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `5769aaa4c6873927ffa0f190808e833e` | Factory Binary Firmware Dump |
| `378055AA_C570M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `7aafcb4de3c9f0378a807b4a756c7024` | Factory Binary Firmware Dump |
| `378055AA_C580M1__A1807680.rwd` | **2008–2023** | 2.44 MB | `b9557f2f4f4c45ff715b65077951f555` | Factory Binary Firmware Dump |
| `378055AA_C670M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `4639bd3aefd17e6666435da1374a48bd` | Factory Binary Firmware Dump |
| `378055AA_C680M1__A1807680.rwd` | **2008–2023** | 2.44 MB | `93e1535050c0d36bcc6be8f1e18ecd4d` | Factory Binary Firmware Dump |
| `378055AA_C720M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `5b972831baee7757c003f8a0c63d8211` | Factory Binary Firmware Dump |
| `378055AA_C820M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `44b9eef017fae734fa3640a2ac3367b1` | Factory Binary Firmware Dump |
| `378055AA_C940M1__A1900417.rwd` | **2008–2023** | 2.44 MB | `7743a9146be256a2b7fd19ba451fb66e` | Factory Binary Firmware Dump |
| `378055AA_C950M1__A1901190.rwd` | **2008–2023** | 2.44 MB | `a79face881f38d92e36cce08e83d3a28` | Factory Binary Firmware Dump |
| `378055AA_K060M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `4d7c7997ad1db9ff912a8ad09aa35640` | Factory Binary Firmware Dump |
| `378055AA_K170M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `af50652eae60e712468c485a03d9fa67` | Factory Binary Firmware Dump |
| `378055AA_K270M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `f04fa2223b0d800f25e2530b58965611` | Factory Binary Firmware Dump |
| `378055AA_K560M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `64c521b75a3c4ac86345d54a83962efb` | Factory Binary Firmware Dump |
| `378055AA_K660M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `968d354cc5d3f9abe00bc306e2c2739f` | Factory Binary Firmware Dump |
| `378055AA_K760M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `421c7149ad1b22329580247ca21eb535` | Factory Binary Firmware Dump |
| `378055AA_L580M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `d2a266a4eba6e223aa06f2565738f1a4` | Factory Binary Firmware Dump |
| `378055AA_L590M1__A1807680.rwd` | **2008–2023** | 2.44 MB | `bf995879861d4bba99419fb489247e36` | Factory Binary Firmware Dump |
| `378055AA_L680M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `36b5fa9e35fb78fef1e731462b203367` | Factory Binary Firmware Dump |
| `378055AA_L690M1__A1807680.rwd` | **2008–2023** | 2.44 MB | `2f1dfee61464a3d0e2c5de6ae1215f37` | Factory Binary Firmware Dump |
| `378055AA_L720M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `a16c3a980f48a7fda84b849c3281df62` | Factory Binary Firmware Dump |
| `378055AA_L820M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `7659ee8540f9d473c0bdff013268a2dc` | Factory Binary Firmware Dump |
| `378055AA_L940M1__A1900417.rwd` | **2008–2023** | 2.44 MB | `5892bf75667340d99b8830a6f20e82b8` | Factory Binary Firmware Dump |
| `378055AA_L950M1__A1901190.rwd` | **2008–2023** | 2.44 MB | `a6382955ba353f58fef4d1bd794a333b` | Factory Binary Firmware Dump |
| `378055AA_X060M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `19848c96054c24fcd7fbf4d1b22d84b8` | Factory Binary Firmware Dump |
| `378055AA_X550M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `e2bdfe8e8f782f35e74c6a7a7a6acf54` | Factory Binary Firmware Dump |
| `378055AA_Y530M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `3de5beba72049e250ee37ca02071b0f6` | Factory Binary Firmware Dump |
| `378055AF_B540M1__A1801384.rwd` | **2008–2023** | 2.44 MB | `7671b70c8a24632e822136735af7c17b` | Factory Binary Firmware Dump |
| `378055AF_B550M1__A1803976.rwd` | **2008–2023** | 2.44 MB | `6a0c850db7fda98afabfc17fbb685146` | Factory Binary Firmware Dump |
| `378055AF_H150M1__A1801384.rwd` | **2008–2023** | 2.44 MB | `dd1987f2d99486beeba29580c11a852a` | Factory Binary Firmware Dump |
| `378055AF_H160M1__A1803976.rwd` | **2008–2023** | 2.44 MB | `d5e790e4742ec3e9029778093313b284` | Factory Binary Firmware Dump |
| `378055AF_H840M1__A1801384.rwd` | **2008–2023** | 2.44 MB | `01edba5de6fcb224a938b8ae991567ee` | Factory Binary Firmware Dump |
| `378055AF_H850M1__A1803976.rwd` | **2008–2023** | 2.44 MB | `c4766c09b83ae7dc5fff8a0f82b65770` | Factory Binary Firmware Dump |
| `378055AG_P830M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `e58a89ac7bf3c355f9f71a5196279ef2` | Factory Binary Firmware Dump |
| `378055AG_P920M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `7b25cd9a6c1051ed928b9284265420d3` | Factory Binary Firmware Dump |
| `378055AG_Q830M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `7a159294e14f89adc5058a98f0675b42` | Factory Binary Firmware Dump |
| `378055AG_S830M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `6dc3db4ba9125a42815bdeeda7717a35` | Factory Binary Firmware Dump |
| `378055AG_S930M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `54b62ec611ef7e195c1ff5efeca9f092` | Factory Binary Firmware Dump |
| `378055AG_U620M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `ba9f0b8fad0eb960cccd6cb9c16d8907` | Factory Binary Firmware Dump |
| `378055AG_U720M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `d8dd4406b98ee47dd4ba9ac67c242352` | Factory Binary Firmware Dump |
| `378055AG_U820M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `5dc4d5b6fe758ae31999cbab22800c20` | Factory Binary Firmware Dump |
| `378055AG_U920M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `10a7b0cc677eeb7c0f96af88b6579abc` | Factory Binary Firmware Dump |
| `378055AG_Z530M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `fe2d71e8db5f535e53f96b315d69ff08` | Factory Binary Firmware Dump |
| `378055AG_Z820M1__A1701596.rwd` | **2008–2023** | 2.44 MB | `850836646e184c4c473b7a46f73bebe4` | Factory Binary Firmware Dump |
| `378055AJ_A520M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `07d5fa9a667eaed5aaefde9f30af9438` | Factory Binary Firmware Dump |
| `378055AJ_A620M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `3fb7bf27b6cbf5088c5cd66d5291bd97` | Factory Binary Firmware Dump |
| `378055AJ_A740M1__A1900417.rwd` | **2008–2023** | 2.44 MB | `685dfceae1a420a82c7fa9547653eb28` | Factory Binary Firmware Dump |
| `378055AJ_A750M1__A1901190.rwd` | **2008–2023** | 2.44 MB | `ac74697d76e81899594425ab842e7ea1` | Factory Binary Firmware Dump |
| `378055AJ_L520M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `01665f0224a1aa01b5f6c4427487d868` | Factory Binary Firmware Dump |
| `378055AJ_L620M1__A1807466.rwd` | **2008–2023** | 2.44 MB | `af330ea16e9c18ad67109c4992916f1e` | Factory Binary Firmware Dump |
| `378055AJ_L740M1__A1900417.rwd` | **2008–2023** | 2.44 MB | `dd93262f08e0dd3dee4f1d871641fbb7` | Factory Binary Firmware Dump |
| `378055AJ_L750M1__A1901190.rwd` | **2008–2023** | 2.44 MB | `39a6e092395c0e425570f2a0e208fd40` | Factory Binary Firmware Dump |
| `378055AN_3050____A1808078.rwd` | **2008–2023** | 2.44 MB | `c5e76e1799330c7cca0e1a4f12ff6bec` | Factory Binary Firmware Dump |
| `378055AN_3060____A1808078.rwd` | **2008–2023** | 2.44 MB | `223e2aa591d24ce0febe100eb9aaaa5d` | Factory Binary Firmware Dump |
| `378055AN_3070____A1808078.rwd` | **2008–2023** | 2.44 MB | `cfbbf4dc5f0e5d48f2dabdd9348feb29` | Factory Binary Firmware Dump |
| `378055AN_3080____A1808078.rwd` | **2008–2023** | 2.44 MB | `db408fbc4e132cd0c530c0a2b1d8c470` | Factory Binary Firmware Dump |
| `378055AN_3090____A1808078.rwd` | **2008–2023** | 2.44 MB | `70dfc1eaf83c2e1cc7ce40c256c8e605` | Factory Binary Firmware Dump |
| `378055AN_4050____A1808078.rwd` | **2008–2023** | 2.44 MB | `56891ff1109df52c0dfada58f49ac478` | Factory Binary Firmware Dump |
| `378055AN_4060____A1808078.rwd` | **2008–2023** | 2.44 MB | `9880259572c16d812ad1b1d67c720b4e` | Factory Binary Firmware Dump |
| `378055AN_4070____A1808078.rwd` | **2008–2023** | 2.44 MB | `adbc31d34e5e8df3d4400f7d20b69fb1` | Factory Binary Firmware Dump |
| `378055AN_4080____A1809243.rwd` | **2008–2023** | 2.44 MB | `9fac55feb1b5dda01d264534bb419bff` | Factory Binary Firmware Dump |
| `378055AN_4090____A1809243.rwd` | **2008–2023** | 2.44 MB | `bfc55abcc1336740c332fe507809c6a7` | Factory Binary Firmware Dump |
| `378055AN_5050____A1809243.rwd` | **2008–2023** | 2.44 MB | `6ec4d38a6e16a1e8711aba1b8443221f` | Factory Binary Firmware Dump |
| `378055AN_5060____A1809243.rwd` | **2008–2023** | 2.44 MB | `1716aa8ae743ecc634f870f05835f498` | Factory Binary Firmware Dump |
| `378055AN_5070____A1809243.rwd` | **2008–2023** | 2.44 MB | `b1822c78da6e34abc0faa7694537aa10` | Factory Binary Firmware Dump |
| `378055AN_9540M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `984439ec72fa71ed2c69fed67d10a0c7` | Factory Binary Firmware Dump |
| `378055AN_A050M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `904aab3af9f209742aad0fa9a8c74761` | Factory Binary Firmware Dump |
| `378055AN_A160M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `8a72bc4f7685278b984402db433b31bb` | Factory Binary Firmware Dump |
| `378055AN_A540M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `ebb233b81d01b467365ccc793fba4046` | Factory Binary Firmware Dump |
| `378055AN_A640M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `beb37510710e0d1b7c359353054696e5` | Factory Binary Firmware Dump |
| `378055AN_A750M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `33dac9e61c43037cde9513c74c537404` | Factory Binary Firmware Dump |
| `378055AN_A850M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `1d35a5f725ba9a72b4415a018cfae97b` | Factory Binary Firmware Dump |
| `378055AN_A950M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `4f9f51ae1016354f739b72b567f9b2a2` | Factory Binary Firmware Dump |
| `378055AN_B540M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `ead5cd3d29b4fee11c7352d9ac223433` | Factory Binary Firmware Dump |
| `378055AN_C050M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `edf8772ae7096f3a3e621042300f51f8` | Factory Binary Firmware Dump |
| `378055AN_C160M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `f0355a1d856b828619a61054eeacb838` | Factory Binary Firmware Dump |
| `378055AN_C250M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `b5a9b95ac4bab192deb0bec1ca02b6d4` | Factory Binary Firmware Dump |
| `378055AN_C360M1__A1809243.rwd` | **2008–2023** | 2.44 MB | `698b888a7832bc3ce2169fe83c2cf366` | Factory Binary Firmware Dump |
| `378055AN_C540M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `3448586785cb7c364166f8476437bf6e` | Factory Binary Firmware Dump |
| `378055AN_C650M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `c9bef992aec6a18905178664dc13e44a` | Factory Binary Firmware Dump |
| `378055AN_C750M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `70540b226f835cac2a79fb35a1c1b201` | Factory Binary Firmware Dump |
| `378055AN_C840M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `b5030e00c30901ca40a530a53407a422` | Factory Binary Firmware Dump |
| `378055AN_C950M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `67cc64951df6f6b0c31e471d81569bd5` | Factory Binary Firmware Dump |
| `378055AN_E120M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `ec4aca776e4ac5e175d48235502f6a4e` | Factory Binary Firmware Dump |
| `378055AN_E140M1__A1902579.rwd` | **2008–2023** | 2.44 MB | `4cea61871065e89d61cc2cba745fa1ac` | Factory Binary Firmware Dump |
| `378055AN_E230M1__A1900171.rwd` | **2008–2023** | 2.44 MB | `8782f19d141649f1b9340a95bcf0e15d` | Factory Binary Firmware Dump |
| `378055AN_E330M1__A1900171.rwd` | **2008–2023** | 2.44 MB | `62fc58c8528709541630c026599d1410` | Factory Binary Firmware Dump |
| `378055AN_E620M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `2e047793e8609ac58617998c81ede4f5` | Factory Binary Firmware Dump |
| `378055AN_G220M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `93283f36c551eaec7bd8a9fe61a2da0a` | Factory Binary Firmware Dump |
| `378055AN_G240M1__A1902579.rwd` | **2008–2023** | 2.44 MB | `b09b7247304a87585d6e7d903529804f` | Factory Binary Firmware Dump |
| `378055AN_G520M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `d3a4c6bd2f23cf69e0b044972b514171` | Factory Binary Firmware Dump |
| `378055AN_G720M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `9a6b922dc36d7930745950b8704bb470` | Factory Binary Firmware Dump |
| `378055AN_G920M1__A1610291.rwd` | **2008–2023** | 2.44 MB | `bca40047cd652e3de5ca898d043129c2` | Factory Binary Firmware Dump |
| `378055AN_L540M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `d6a5615a294c1e6cce58bee4aff1f355` | Factory Binary Firmware Dump |
| `378055AN_L640M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `bf8a2550165c1a5a15c580afec3fff96` | Factory Binary Firmware Dump |
| `378055AN_L750M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `95c45f88a0960e608bc52a129ed99849` | Factory Binary Firmware Dump |
| `378055AN_L850M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `9bf8d4d661cf98cdbbc9ae654e3e2596` | Factory Binary Firmware Dump |
| `378055AN_L950M1__A1808078.rwd` | **2008–2023** | 2.44 MB | `a216a23e55bb09237fac61866b828798` | Factory Binary Firmware Dump |
| `378055AW_G030M1__A1900171.rwd` | **2008–2023** | 2.44 MB | `de212054fd985320321274d80c3ed96c` | Factory Binary Firmware Dump |
| `378055AW_G130M1__A1900171.rwd` | **2008–2023** | 2.44 MB | `7184bf03b4f31ce5dd2c9bc7422983f9` | Factory Binary Firmware Dump |
| `378055AW_G330M1__A1902579.rwd` | **2008–2023** | 2.44 MB | `0b2f1a91a600ec082a743b5a6d9408c7` | Factory Binary Firmware Dump |
| `378055AW_G430M1__A1902579.rwd` | **2008–2023** | 2.44 MB | `1d084c96f3bd52d9699931dc0070b4f6` | Factory Binary Firmware Dump |
| `378055AY_H160M6__A1809665.rwd` | **2008–2023** | 2.63 MB | `c3b38562febc0522017dfb86fc75e79a` | Factory Binary Firmware Dump |
| `378055AY_H660M6__A1613477.rwd` | **2008–2023** | 2.63 MB | `3adca94c3b1753602770b89df914008e` | Factory Binary Firmware Dump |
| `378055AY_H680M6__A1809665.rwd` | **2008–2023** | 2.63 MB | `11d6c1ce201533f5b6539e8c9c15fe8c` | Factory Binary Firmware Dump |
| `378055AY_H980M6__A1809665.rwd` | **2008–2023** | 2.63 MB | `ab383d911efefb9a24b0cf95dea610f0` | Factory Binary Firmware Dump |
| `378055AY_S620M6__A1809665.rwd` | **2008–2023** | 2.63 MB | `e06beb32aa8f78e72a34707aeb00d309` | Factory Binary Firmware Dump |
| `378055AY_S820M6__A1809665.rwd` | **2008–2023** | 2.63 MB | `dce63e1f12d757b30b8344d09f6e0b80` | Factory Binary Firmware Dump |
| `378055D2_H720M1__A1604984.rwd` | **2008–2023** | 1.94 MB | `3755f1b5795bd4cdeec2404316c648e0` | Factory Binary Firmware Dump |
| `378055FG_M060M6__A1610583.rwd` | **2008–2023** | 2.38 MB | `6855dc40b1ec66f211dff7789932629b` | Factory Binary Firmware Dump |
| `378055FG_M070M6__A1906747.rwd` | **2008–2023** | 2.38 MB | `36b5e247ae5b6eb503371ba271c0005e` | Factory Binary Firmware Dump |
| `378055FG_M560M6__A1610583.rwd` | **2008–2023** | 2.38 MB | `daecc0145f961f9fa8277346b8c63e05` | Factory Binary Firmware Dump |
| `378055FG_M570M6__A1906747.rwd` | **2008–2023** | 2.38 MB | `8e8bfa6233c6076888fe491fd7a2ae36` | Factory Binary Firmware Dump |
| `37806-RB0-9610-M1.rwd` | **2008–2023** | 480.1 KB | `d29a704d0c1032cd887363b3c60d6f57` | Factory Binary Firmware Dump |
| `37806-RB0-9620-M1.rwd` | **2008–2023** | 480.1 KB | `f1876ad2e705a9b464a10e7b2db2cb1f` | Factory Binary Firmware Dump |
| `37806-RB0-E720-M1.rwd` | **2008–2023** | 480.1 KB | `901117a05ff88e2fbd909069ecbf57d7` | Factory Binary Firmware Dump |
| `37806-RB0-E730-M1.rwd` | **2008–2023** | 480.1 KB | `826d3bbb4d6ad089cf2035f28cdf9ca2` | Factory Binary Firmware Dump |
| `37806-RB0-E820-M1.rwd` | **2008–2023** | 480.1 KB | `5b8f199e96d2e22148c4f2143b2c4f41` | Factory Binary Firmware Dump |
| `37806-RB0-J640-M1.rwd` | **2008–2023** | 480.1 KB | `02296c0a2e0f076dbf1adc20fdcf46ad` | Factory Binary Firmware Dump |
| `37806-RB0-J650-M1.rwd` | **2008–2023** | 480.2 KB | `2263455df460fc44b4714f05a4ab86aa` | Factory Binary Firmware Dump |
| `37806-RB0-J740-M1.rwd` | **2008–2023** | 480.1 KB | `758462f0354f9207c867bbc4b25f408a` | Factory Binary Firmware Dump |
| `37806-RB0-J750-M1.rwd` | **2008–2023** | 480.2 KB | `b9a7ce41eab03dad693d31d94c457bdb` | Factory Binary Firmware Dump |
| `37806-RB0-J820-M1.rwd` | **2008–2023** | 480.1 KB | `7b3ad41e0c2fb905b210c62456370eff` | Factory Binary Firmware Dump |
| `57114-TF0-G120-M1.rwd` | **2008–2023** | 602.6 KB | `2a8bd14181bee0f99b20064dac9fba55` | Factory Binary Firmware Dump |
| `57114-TF0-G220-M1.rwd` | **2008–2023** | 602.6 KB | `153d36dbbc632a2e99a43ca05eee105c` | Factory Binary Firmware Dump |
| `57114-TF0-G820-M1.rwd` | **2008–2023** | 602.6 KB | `eab2dcfc4f426ebe542defc88326df79` | Factory Binary Firmware Dump |
| `57114-TF0-J030-M1.rwd` | **2008–2023** | 499.6 KB | `db448dc02c4e283b2fcc5dda6cb37d09` | Factory Binary Firmware Dump |
| `57114-TF0-J120-M1.rwd` | **2008–2023** | 602.9 KB | `c8991fc5268788783f0172f945cbfc75` | Factory Binary Firmware Dump |
| `57114-TF0-J220-M1.rwd` | **2008–2023** | 602.9 KB | `fb8039ce9cea64df1bb34d76810c49f3` | Factory Binary Firmware Dump |
| `57114-TF0-J530-M1.rwd` | **2008–2023** | 499.6 KB | `e31b093629d654244c93964fd76edc48` | Factory Binary Firmware Dump |
| `57114-TF0-J820-M1.rwd` | **2008–2023** | 602.6 KB | `f00ba5be0361855611cfda37c7a0664b` | Factory Binary Firmware Dump |
| `57114-TF0-Q420-M1.rwd` | **2008–2023** | 602.6 KB | `e330a92f50b3bd59613c0aa72aedaa2d` | Factory Binary Firmware Dump |
| `57114-TF0-Q520-M1.rwd` | **2008–2023** | 602.6 KB | `c736dbdc9937a404eafc44104f41ec00` | Factory Binary Firmware Dump |
| `57114-TF0-Q620-M1.rwd` | **2008–2023** | 602.6 KB | `9f284d05e4682d6f538631a15a1fdc37` | Factory Binary Firmware Dump |
| `57114-TF0-Q720-M1.rwd` | **2008–2023** | 602.6 KB | `04300ea78ef27538eb1faaedc6763133` | Factory Binary Firmware Dump |
| `77959-TF0-E510-M3.rwd` | **2008–2023** | 187.0 KB | `dbaa5942c61ea04c760584d042add5eb` | Factory Binary Firmware Dump |
| `77959-TF0-E830-M3.rwd` | **2008–2023** | 187.0 KB | `9ad931c90742eeaf50691ab7c30d2690` | Factory Binary Firmware Dump |
| `77959-TF0-E840-M3.rwd` | **2008–2023** | 178.9 KB | `f687842e90e2bf3b20220d1b381a56fc` | Factory Binary Firmware Dump |
| `77959-TF0-E870-M3.rwd` | **2008–2023** | 227.6 KB | `4fbc738f5a13d8a6e37f27dcac212909` | Factory Binary Firmware Dump |
| `77959-TF0-G510-M3.rwd` | **2008–2023** | 187.0 KB | `1491ed6f52057c94ea515349da744457` | Factory Binary Firmware Dump |
| `77959-TF0-G830-M3.rwd` | **2008–2023** | 187.0 KB | `0969cc97b189c073b07981c23e2fe72d` | Factory Binary Firmware Dump |
| `77959-TF0-G840-M3.rwd` | **2008–2023** | 178.9 KB | `05258ca3a4fdc3b2a690f6fc76e827b7` | Factory Binary Firmware Dump |
| `77959-TF0-G870-M3.rwd` | **2008–2023** | 227.6 KB | `30a8b2a657b0838f4ecc1281ac9a8c90` | Factory Binary Firmware Dump |
| `77959-TF0-H430-M3.rwd` | **2008–2023** | 187.0 KB | `832ab7cac33cee76843a88f7ac5052f6` | Factory Binary Firmware Dump |
| `77959-TF0-H440-M3.rwd` | **2008–2023** | 187.1 KB | `1376b22b88a09a433ef2bd993237151b` | Factory Binary Firmware Dump |
| `77959-TF0-H470-M3.rwd` | **2008–2023** | 227.6 KB | `245502cebccdb7623093392198e86383` | Factory Binary Firmware Dump |
| `77959-TF0-H630-M3.rwd` | **2008–2023** | 187.0 KB | `e13d4bdb94e68429099b95c3e8bb1379` | Factory Binary Firmware Dump |
| `77959-TF0-H640-M3.rwd` | **2008–2023** | 187.1 KB | `bcbc199c52b6c86713e7014180951d76` | Factory Binary Firmware Dump |
| `77959-TF0-H670-M3.rwd` | **2008–2023** | 227.6 KB | `5249f1919eaacdc3d42a5e8f7555ce4c` | Factory Binary Firmware Dump |
| `77959-TF0-H830-M3.rwd` | **2008–2023** | 187.0 KB | `fe6fb987b9277e340d31b6cc5e66608d` | Factory Binary Firmware Dump |
| `77959-TF0-H840-M3.rwd` | **2008–2023** | 187.1 KB | `e213351048bf62437ac257cc6bfac547` | Factory Binary Firmware Dump |
| `77959-TF0-H870-M3.rwd` | **2008–2023** | 227.6 KB | `a4dfff2ca4815db0d76790115e15ffef` | Factory Binary Firmware Dump |
| `77959-TF0-J450-M3.rwd` | **2008–2023** | 187.1 KB | `ba676598fddcc50ff8ea0076436ff67b` | Factory Binary Firmware Dump |
| `77959-TF0-J460-M3.rwd` | **2008–2023** | 187.1 KB | `dbd9685daa16035216a092efaabb0c5c` | Factory Binary Firmware Dump |
| `77959-TF0-J490-M3.rwd` | **2008–2023** | 227.6 KB | `8d4acbd085b165802a0747e862ceebbf` | Factory Binary Firmware Dump |
| `77959-TF0-J850-M3.rwd` | **2008–2023** | 187.1 KB | `b523ce4f10597364f924258be0df23e9` | Factory Binary Firmware Dump |
| `77959-TF0-J860-M3.rwd` | **2008–2023** | 187.1 KB | `bca5478d6b0bce2670c2547d02d5ff58` | Factory Binary Firmware Dump |
| `77959-TF0-J890-M3.rwd` | **2008–2023** | 227.6 KB | `2c63866469924ad16345e19322f3245c` | Factory Binary Firmware Dump |
| `77959-TF0-Q840-M3.rwd` | **2008–2023** | 187.1 KB | `6066b5d14ff9a5a7c42c7809c92c106f` | Factory Binary Firmware Dump |
| `77959-TF0-Q850-M3.rwd` | **2008–2023** | 187.1 KB | `0b6e0c6e7b3c515b03ae0cfcf49ea7cc` | Factory Binary Firmware Dump |
| `77959-TF0-Q880-M3.rwd` | **2008–2023** | 227.6 KB | `9e2fc07a970b13be4db338e35a703b4d` | Factory Binary Firmware Dump |
| `77959-TF0-U630-M3.rwd` | **2008–2023** | 187.0 KB | `68bac4350075ffaed0cc4a37c7e6a40b` | Factory Binary Firmware Dump |
| `77959-TF0-U640-M3.rwd` | **2008–2023** | 187.1 KB | `222126655bf564cb1612c96321686211` | Factory Binary Firmware Dump |
| `77959-TF0-U670-M3.rwd` | **2008–2023** | 227.6 KB | `898abb3b6b263a01f7b199e5746e5ad1` | Factory Binary Firmware Dump |
| `77959-TF0-Y430-M3.rwd` | **2008–2023** | 187.0 KB | `f9791adb8f8b82009fc184a6ae195d16` | Factory Binary Firmware Dump |
| `77959-TF0-Y440-M3.rwd` | **2008–2023** | 187.1 KB | `81d15ad67fe42b030b54679259df7996` | Factory Binary Firmware Dump |
| `77959-TF0-Y470-M3.rwd` | **2008–2023** | 227.6 KB | `1ddd184e7084a2c52f93e3702d9683a3` | Factory Binary Firmware Dump |
| `77959-TF0-Y630-M3.rwd` | **2008–2023** | 187.0 KB | `188da877f3058d7ac984e4d88fa0d0c7` | Factory Binary Firmware Dump |
| `77959-TF0-Y640-M3.rwd` | **2008–2023** | 187.1 KB | `ae746bf766c489f98519ad75753aba87` | Factory Binary Firmware Dump |
| `77959-TF0-Y670-M3.rwd` | **2008–2023** | 227.6 KB | `4caef727d1ad040903ee15d832d8df35` | Factory Binary Firmware Dump |
| `77959-TF0-Z440-M3.rwd` | **2008–2023** | 187.1 KB | `730fa03115c32c71f9e2db2d65e6ff28` | Factory Binary Firmware Dump |
| `77959-TF0-Z450-M3.rwd` | **2008–2023** | 187.1 KB | `4cf342cecec53a2c7f78f05e7442b932` | Factory Binary Firmware Dump |
| `77959-TF0-Z480-M3.rwd` | **2008–2023** | 227.6 KB | `7584b78dc63e602fd2ce64dc8c1d85c8` | Factory Binary Firmware Dump |
| `77959-TF0-Z840-M3.rwd` | **2008–2023** | 187.1 KB | `e370dedc2389449dd6dd52dba80ec5c5` | Factory Binary Firmware Dump |
| `77959-TF0-Z850-M3.rwd` | **2008–2023** | 187.1 KB | `78a06567e7f76915ba96827351e9b347` | Factory Binary Firmware Dump |
| `77959-TF0-Z880-M3.rwd` | **2008–2023** | 227.6 KB | `02be1616389bbdd8b9c2b33dc913a91e` | Factory Binary Firmware Dump |

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
