# v7.3 - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/Deprecated/v7.3`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `92 files` (0 binary dumps, 92 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `v7.3` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R4C9F493B_5d55-040_100_003_v7.3.a2l` | **2015–2026** | 837.3 KB | `db6226fe53ab39617411de3357c09454` | ASAM ASAP2 ECU Description File |
| `R4C9F493B_5d55-040_100_003_v7.3.xdf` | **2015–2026** | 2.73 MB | `30ed693fc2d28c699f9cdf9f6a61c2dd` | TunerPro Binary Definition Map |
| `R4C9F4E6B_5d55-040_150_006_v7.3.a2l` | **2015–2026** | 837.3 KB | `b89963489f517157f3a0c9572247f785` | ASAM ASAP2 ECU Description File |
| `R4C9F4E6B_5d55-040_150_006_v7.3.xdf` | **2015–2026** | 2.73 MB | `a46b6f66fb903f7dc74a04b1ea9181fd` | TunerPro Binary Definition Map |
| `R4C9F4K6B_5d55-040_170_006_v7.3.a2l` | **2015–2026** | 837.3 KB | `74e5584d248e1f1d2da19868bb80bcfe` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.3.xdf` | **2015–2026** | 2.73 MB | `12daf2322150a283caf7a2f4e8d203d7` | TunerPro Binary Definition Map |
| `R4C9F4N5B_5d55-040_180_005_v7.3.a2l` | **2015–2026** | 837.3 KB | `1706aa7da47e0c3b38c028585e3db41d` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.3.xdf` | **2015–2026** | 2.73 MB | `21a9f8d47a54f4e81dfec408150ae4e6` | TunerPro Binary Definition Map |
| `R4C9F4P7B_5d55-040_190_007_v7.3.a2l` | **2015–2026** | 837.3 KB | `9088efcf392241171af3f7cdca6fb369` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.3.xdf` | **2015–2026** | 2.73 MB | `21a9f8d47a54f4e81dfec408150ae4e6` | TunerPro Binary Definition Map |
| `R4C9F4P9B_5d55-040_190_009_v7.3.a2l` | **2015–2026** | 837.3 KB | `017678ca0c0e228288391089f34f1d03` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.3.xdf` | **2015–2026** | 2.73 MB | `21a9f8d47a54f4e81dfec408150ae4e6` | TunerPro Binary Definition Map |
| `R4C9H5C5B_5d55-050_140_005_v7.3.a2l` | **2015–2026** | 844.3 KB | `a1559507b6f187fd871b4472bed6812f` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `069c3b6fef84b718a54ba6b8580992a0` | TunerPro Binary Definition Map |
| `R4C9H5I5B_5d55-050_160_005_v7.3.a2l` | **2015–2026** | 844.3 KB | `4cca686632ce0d0212fe28dce83ac049` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `7df8f1332ab862c2fe35d0f4af7cc9b3` | TunerPro Binary Definition Map |
| `R4C9H5K5B_5d55-050_170_005_v7.3.a2l` | **2015–2026** | 844.3 KB | `9f2e1146785e4f9268abce4379e01d9e` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `5a9112c36ef7a498544ecab7ab183bbc` | TunerPro Binary Definition Map |
| `R4C9H5N6B_5d55-050_180_006_v7.3.a2l` | **2015–2026** | 844.3 KB | `1d8890c9b64a1943c5516c9a8d973296` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.3.xdf` | **2015–2026** | 2.75 MB | `254f3d3965d80521ded8481b800b073d` | TunerPro Binary Definition Map |
| `R4C9H5P7B_5d55-050_190_007_v7.3.a2l` | **2015–2026** | 844.3 KB | `387deee0e82478f2f9ce08ad192a44d1` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `621351823f77d1ac33ee0d71cef53ab3` | TunerPro Binary Definition Map |
| `R4C9H5P9B_5d55-050_190_009_v7.3.a2l` | **2015–2026** | 844.3 KB | `0675335e167f1b750c585fe710bde0c0` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.3.xdf` | **2015–2026** | 2.75 MB | `621351823f77d1ac33ee0d71cef53ab3` | TunerPro Binary Definition Map |
| `R4C9H5S8B_5d55-050_200_008_v7.3.a2l` | **2015–2026** | 844.3 KB | `5deacdb47e4f00b7e8986efc205b8202` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.3.xdf` | **2015–2026** | 2.75 MB | `2c777a9466942072210d205985c4d73f` | TunerPro Binary Definition Map |
| `R4C9H5V5B_5d55-050_220_005_v7.3.a2l` | **2015–2026** | 844.3 KB | `20beb8dc481c419c11da507e346397f6` | ASAM ASAP2 ECU Description File |
| `R4C9H5V5B_5d55-050_220_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `3528783d615339dc5b701009c2c451ba` | TunerPro Binary Definition Map |
| `R4C9H695B_5d55-060_100_005_v7.3.a2l` | **2015–2026** | 844.3 KB | `295b4f6d04f8e5f49535595939d1b819` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `9b60e3494a8effd7c0ee101c888b2913` | TunerPro Binary Definition Map |
| `R4C9H6B5B_5d55-060_110_005_v7.3.a2l` | **2015–2026** | 844.3 KB | `bf24fa41836afb490255a9b4aeed5a20` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `e0c32d7abc9550d79f9017a9d916d5e4` | TunerPro Binary Definition Map |
| `R4C9H6D6B_5d55-060_120_006_v7.3.a2l` | **2015–2026** | 844.3 KB | `f7e4600cd4932282abbcb495372644b5` | ASAM ASAP2 ECU Description File |
| `R4C9H6D6B_5d55-060_120_006_v7.3.xdf` | **2015–2026** | 2.75 MB | `2644d1d45be66f06abf3929fc9249938` | TunerPro Binary Definition Map |
| `R4C9H6D7B_5d55-060_120_007_v7.3.a2l` | **2015–2026** | 844.3 KB | `72767ea7dc9b1d674dbec3720af6aa4e` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `ef33330129971a02475de0334be7f7c6` | TunerPro Binary Definition Map |
| `R4C9H6H7B_5d55-060_130_007_v7.3.a2l` | **2015–2026** | 844.3 KB | `ce488df58951a410e9de2aeaf5208dba` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `f294f4e2537c61fd795901e5f81d6b11` | TunerPro Binary Definition Map |
| `R4C9H6K5B_5d55-060_140_005_v7.3.a2l` | **2015–2026** | 844.3 KB | `ff4f3d2d426e8d77b4cf662bf379c423` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `a3968c1c08b936eed0384830b4ce4ffe` | TunerPro Binary Definition Map |
| `R4C9H6N7B_5d55-060_150_007_v7.3.a2l` | **2015–2026** | 844.3 KB | `2257eceaac32beeb5a2da4aae5246be8` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `7e14af622324980e9bc1082accf34cf9` | TunerPro Binary Definition Map |
| `R4C9H6P7B_5d55-060_160_007_v7.3.a2l` | **2015–2026** | 844.3 KB | `31fe688c49cc5086175deab6c253a7fd` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `b5b042fe7a3ae947672714b834c8c6d2` | TunerPro Binary Definition Map |
| `R4C9H6P9B_5d55-060_160_009_v7.3.a2l` | **2015–2026** | 844.3 KB | `f2cf6c65951d85075f855f0ce81a1d69` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.3.xdf` | **2015–2026** | 2.75 MB | `b5b042fe7a3ae947672714b834c8c6d2` | TunerPro Binary Definition Map |
| `R4C9H6S8B_5d55-060_170_008_v7.3.a2l` | **2015–2026** | 844.3 KB | `7cb5cdd159827b376a255a69f6449777` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.3.xdf` | **2015–2026** | 2.75 MB | `292c411c486af37b5a49d0197b83b69f` | TunerPro Binary Definition Map |
| `R4C9H6V5B_5d55-060_190_005_v7.3.a2l` | **2015–2026** | 844.3 KB | `df3d26856a19ef6fb025bc56b68d1d59` | ASAM ASAP2 ECU Description File |
| `R4C9H6V5B_5d55-060_190_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `0ec901c95df19a7b107d1061249acb75` | TunerPro Binary Definition Map |
| `R4C9J718B_5d55-070_030_008_v7.3.a2l` | **2015–2026** | 849.2 KB | `b2ed24ec3500e5f764eb38954c36ffe0` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.3.xdf` | **2015–2026** | 2.76 MB | `6ddaae807302b50dd133fd0bedd559f3` | TunerPro Binary Definition Map |
| `R4C9J755B_5d55-070_040_005_v7.3.a2l` | **2015–2026** | 849.2 KB | `62d8b80d3a3167fc9959dfdde92983b8` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `fdb8ade083c959f290fe68065596b407` | TunerPro Binary Definition Map |
| `R4C9J756B_5d55-070_040_006_v7.3.a2l` | **2015–2026** | 849.2 KB | `5ef476df5f275950357f79094e7c9ce1` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.3.xdf` | **2015–2026** | 2.76 MB | `3f24f40a4cd69ee304449b6e91324c8e` | TunerPro Binary Definition Map |
| `R4C9J758B_5d55-070_050_008_v7.3.a2l` | **2015–2026** | 849.2 KB | `0fce90743571f203bf0c0ba1f3e0e02e` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.3.xdf` | **2015–2026** | 2.76 MB | `d922171c6849b66e830447b649d7bad8` | TunerPro Binary Definition Map |
| `R4C9J797B_5d55-070_060_007_v7.3.a2l` | **2015–2026** | 849.2 KB | `ef750c0ee4360584e1190755f6fc56f9` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.3.xdf` | **2015–2026** | 2.76 MB | `7e6d86c42863bcdae899c7d80bbba3c8` | TunerPro Binary Definition Map |
| `R4C9J7A5B_5d55-070_070_005_v7.3.a2l` | **2015–2026** | 849.2 KB | `dfcc7dee4a099a0472a04eb514ab4b9f` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `7e6d86c42863bcdae899c7d80bbba3c8` | TunerPro Binary Definition Map |
| `R4C9J7N5B_5d55-070_080_005_v7.3.a2l` | **2015–2026** | 849.2 KB | `cd1eafa1adb6fba915b3f029dcf5b2d7` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `368faf5b44adf85680306bb85bbb3f35` | TunerPro Binary Definition Map |
| `R4C9J7P7B_5d55-070_090_007_v7.3.a2l` | **2015–2026** | 849.2 KB | `3cc7f965b4d0a5b4a8ee3391f61d06fc` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.3.xdf` | **2015–2026** | 2.76 MB | `a6be730a013139a2eb24829a4e208ecc` | TunerPro Binary Definition Map |
| `R4C9J7P9B_5d55-070_090_009_v7.3.a2l` | **2015–2026** | 849.2 KB | `9eae9b5ec406622c3527c5e67540c767` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.3.xdf` | **2015–2026** | 2.76 MB | `a6be730a013139a2eb24829a4e208ecc` | TunerPro Binary Definition Map |
| `R4C9J7S8B_5d55-070_100_008_v7.3.a2l` | **2015–2026** | 849.2 KB | `ceef586ad9e8c872219ad7fb5fcc1708` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.3.xdf` | **2015–2026** | 2.76 MB | `8773c6a60a4c8615bcd932d99020d00b` | TunerPro Binary Definition Map |
| `R4C9J7V5B_5d55-070_120_005_v7.3.a2l` | **2015–2026** | 849.2 KB | `4a7979a622d1d6c43dbbdb426219477c` | ASAM ASAP2 ECU Description File |
| `R4C9J7V5B_5d55-070_120_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `3f8346157e512c77bbe3b92518db4021` | TunerPro Binary Definition Map |
| `R4C9J7W5B_5d55-070_130_005_v7.3.a2l` | **2015–2026** | 849.2 KB | `198704bc3959b5385179cfa538f1dd67` | ASAM ASAP2 ECU Description File |
| `R4C9J7W5B_5d55-070_130_005_v7.3.xdf` | **2015–2026** | 2.76 MB | `3f8346157e512c77bbe3b92518db4021` | TunerPro Binary Definition Map |
| `R4C9L857B_5d55-080_040_007_v7.3.a2l` | **2015–2026** | 844.5 KB | `8b0f3ecb7daf5cd30cab1758c8a950eb` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `c984171bc7c2fa09736c9343ee0256bf` | TunerPro Binary Definition Map |
| `R4C9L875B_5d55-080_055_005_v7.3.a2l` | **2015–2026** | 844.5 KB | `ff03ff1aca50de3670e66947c778fb2d` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `0c2f813c1da671fbbb58ca100b8b3157` | TunerPro Binary Definition Map |
| `R4C9L8N5B_5d55-080_060_005_v7.3.a2l` | **2015–2026** | 844.5 KB | `90c931bd4d5b3a64612815e96458e0ad` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `6cb9d84a74ada8a70ecc9ebde883fce3` | TunerPro Binary Definition Map |
| `R4C9L8P7B_5d55-080_072_007_v7.3.a2l` | **2015–2026** | 844.5 KB | `7c6f836698065dbed759a70c33c92f35` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.3.xdf` | **2015–2026** | 2.75 MB | `7916ce9d67ac3dd6cbb4677c278b593e` | TunerPro Binary Definition Map |
| `R4C9L8P9B_5d55-080_072_009_v7.3.a2l` | **2015–2026** | 844.5 KB | `64b8468b9a3308724c73d60e12da238f` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.3.xdf` | **2015–2026** | 2.75 MB | `7916ce9d67ac3dd6cbb4677c278b593e` | TunerPro Binary Definition Map |
| `R4C9L8PCB_5d55-080_072_012_v7.3.a2l` | **2015–2026** | 844.5 KB | `4ac235bcc84ef97714290468a0f7a968` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.3.xdf` | **2015–2026** | 2.75 MB | `6c6a34030f07b9a0e4b115925b1129ef` | TunerPro Binary Definition Map |
| `R4C9L8S8B_5d55-080_080_008_v7.3.a2l` | **2015–2026** | 844.5 KB | `98e43d7a96635b7ac667c2afd9b0db47` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.3.xdf` | **2015–2026** | 2.75 MB | `51110599a05e1f72f5dc9cb2c80ab087` | TunerPro Binary Definition Map |
| `R4C9L8V6B_5d55-080_100_006_v7.3.a2l` | **2015–2026** | 844.5 KB | `9ca63cdd53561e9b5f2155d82c59554b` | ASAM ASAP2 ECU Description File |
| `R4C9L8V6B_5d55-080_100_006_v7.3.xdf` | **2015–2026** | 2.75 MB | `c030c3c11adfa3eb7d2da186517bd735` | TunerPro Binary Definition Map |
| `R4C9L8W9B_5d55-080_140_005_v7.3.a2l` | **2015–2026** | 844.5 KB | `773d58dd9f1407023e04a8fd8d89c129` | ASAM ASAP2 ECU Description File |
| `R4C9L8W9B_5d55-080_140_005_v7.3.xdf` | **2015–2026** | 2.75 MB | `d952c72a6bda18dd2a394b9398f6d229` | TunerPro Binary Definition Map |

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
