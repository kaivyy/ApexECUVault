# ImperialUnits - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 2/v7.3.3/ImperialUnits`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `114 files` (0 binary dumps, 114 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ImperialUnits` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `R4C9F493B_5d55-040_100_003_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.86 MB | `3605401402e79839a48a77e136c1c771` | TunerPro Binary Definition Map |
| `R4C9F493B_5d55-040_100_003_v7.3.3.a2l` | **2015–2026** | 902.3 KB | `27916a5c0b649e560520e7643be4f36f` | ASAM ASAP2 ECU Description File |
| `R4C9F4C6B_5d55-040_140_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.86 MB | `e656914085dfbd07c8377339a8f5c624` | TunerPro Binary Definition Map |
| `R4C9F4C6B_5d55-040_140_006_v7.3.3.a2l` | **2015–2026** | 902.3 KB | `fd699c58a6a78d2b53c938955a961f47` | ASAM ASAP2 ECU Description File |
| `R4C9F4E6B_5d55-040_150_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.86 MB | `e7615dc0aa22622385cdc45ddfb9e88a` | TunerPro Binary Definition Map |
| `R4C9F4E6B_5d55-040_150_006_v7.3.3.a2l` | **2015–2026** | 902.3 KB | `d354776de9ad578e79cf434b16c62a47` | ASAM ASAP2 ECU Description File |
| `R4C9F4K6B_5d55-040_170_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.86 MB | `d35af4c8a859c9c64c407b41e73d43c6` | TunerPro Binary Definition Map |
| `R4C9F4K6B_5d55-040_170_006_v7.3.3.a2l` | **2015–2026** | 902.3 KB | `58503bd1d5c6ea56dbf72edc9b3131a5` | ASAM ASAP2 ECU Description File |
| `R4C9F4N5B_5d55-040_180_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.86 MB | `aa6426c8db20a1d5a733cfd687b6ad94` | TunerPro Binary Definition Map |
| `R4C9F4N5B_5d55-040_180_005_v7.3.3.a2l` | **2015–2026** | 902.4 KB | `9c802e1540662925b1876d92bbfba769` | ASAM ASAP2 ECU Description File |
| `R4C9F4P7B_5d55-040_190_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.86 MB | `aa6426c8db20a1d5a733cfd687b6ad94` | TunerPro Binary Definition Map |
| `R4C9F4P7B_5d55-040_190_007_v7.3.3.a2l` | **2015–2026** | 902.4 KB | `42ee80f032929cf807cabf6776c5350d` | ASAM ASAP2 ECU Description File |
| `R4C9F4P9B_5d55-040_190_009_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.86 MB | `aa6426c8db20a1d5a733cfd687b6ad94` | TunerPro Binary Definition Map |
| `R4C9F4P9B_5d55-040_190_009_v7.3.3.a2l` | **2015–2026** | 902.4 KB | `cb7b9578c84afbe5d87959c5aed8e0f4` | ASAM ASAP2 ECU Description File |
| `R4C9H56AB_5d55-050_115_010_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `f50b63cc1635c02fa37f362012faf4c0` | TunerPro Binary Definition Map |
| `R4C9H56AB_5d55-050_115_010_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `333ddb8de2f764f2bebd487690db621f` | ASAM ASAP2 ECU Description File |
| `R4C9H596B_5d55-050_120_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `4c3fe33c7296ff496d98e0c6e5c6dd28` | TunerPro Binary Definition Map |
| `R4C9H596B_5d55-050_120_006_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `a9e5c78ac5b820c4f526c31969dd33f0` | ASAM ASAP2 ECU Description File |
| `R4C9H5C5B_5d55-050_140_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `3aa903750572f1ed594769b0e9d8834f` | TunerPro Binary Definition Map |
| `R4C9H5C5B_5d55-050_140_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `86a342a0ea772f0bee38421faa57e421` | ASAM ASAP2 ECU Description File |
| `R4C9H5E5B_5d55-050_150_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `a46ca888cf5dcac168f0ca455b580e75` | TunerPro Binary Definition Map |
| `R4C9H5E5B_5d55-050_150_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `e425e5bb0870d7960ffd057de1f3051b` | ASAM ASAP2 ECU Description File |
| `R4C9H5E6B_5d55-050_150_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `5e1b1d8f0fb0d8070b8b73d6b406c7cb` | TunerPro Binary Definition Map |
| `R4C9H5E6B_5d55-050_150_006_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `cac18da92d12c4fc357c14508156bf7e` | ASAM ASAP2 ECU Description File |
| `R4C9H5I5B_5d55-050_160_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `a680c423df868e0005667eecbed74985` | TunerPro Binary Definition Map |
| `R4C9H5I5B_5d55-050_160_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `baeed4272bbde3d034523e6c4119e90f` | ASAM ASAP2 ECU Description File |
| `R4C9H5K5B_5d55-050_170_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `6c57feac33df150c4ec2b2f9bd990dbe` | TunerPro Binary Definition Map |
| `R4C9H5K5B_5d55-050_170_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `a83c3d4140a5907b821cf83ad7e0fdf0` | ASAM ASAP2 ECU Description File |
| `R4C9H5N6B_5d55-050_180_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `ce5457a0dd4e630b0b6c9bc7d563d357` | TunerPro Binary Definition Map |
| `R4C9H5N6B_5d55-050_180_006_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `d2760a6a1f20f5d67421248d813ed8a6` | ASAM ASAP2 ECU Description File |
| `R4C9H5P7B_5d55-050_190_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `9b71513dd302baf9f470eaa0c11ee634` | TunerPro Binary Definition Map |
| `R4C9H5P7B_5d55-050_190_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `52b75f03f650ecd76b033ca6099bc7b5` | ASAM ASAP2 ECU Description File |
| `R4C9H5P9B_5d55-050_190_009_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `9b71513dd302baf9f470eaa0c11ee634` | TunerPro Binary Definition Map |
| `R4C9H5P9B_5d55-050_190_009_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `7292db8e214f35be8e4637f28d523fbf` | ASAM ASAP2 ECU Description File |
| `R4C9H5S8B_5d55-050_200_008_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `036d19a4022dd1783893108389714041` | TunerPro Binary Definition Map |
| `R4C9H5S8B_5d55-050_200_008_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `f4aece1193e75d03b34dc905ccd4415e` | ASAM ASAP2 ECU Description File |
| `R4C9H5V5B_5d55-050_220_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `02b455992074880f466fc173a3514e18` | TunerPro Binary Definition Map |
| `R4C9H5V5B_5d55-050_220_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `f349d17fabdecdd7771291162220cf0f` | ASAM ASAP2 ECU Description File |
| `R4C9H695B_5d55-060_100_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `673dcd8722b8c08f3e6c57dabdf6dc0d` | TunerPro Binary Definition Map |
| `R4C9H695B_5d55-060_100_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `35570e00d9a2b98775dd357bd465a56f` | ASAM ASAP2 ECU Description File |
| `R4C9H6B5B_5d55-060_110_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `1be800ccc3b0c0f46156c0d4b3900e11` | TunerPro Binary Definition Map |
| `R4C9H6B5B_5d55-060_110_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `c386353a15d5253d86aee177a0c73af5` | ASAM ASAP2 ECU Description File |
| `R4C9H6D5B_5d55-060_120_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `e69c62747fb28dda66c79f4fa084e9ff` | TunerPro Binary Definition Map |
| `R4C9H6D5B_5d55-060_120_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `b4d92afc9ca3a90e307100cf205ad97a` | ASAM ASAP2 ECU Description File |
| `R4C9H6D6B_5d55-060_120_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `b32cd652fa963605241608177c79a999` | TunerPro Binary Definition Map |
| `R4C9H6D6B_5d55-060_120_006_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `cfd9c3bc3888db2aa34b3d97a4c0aed0` | ASAM ASAP2 ECU Description File |
| `R4C9H6D7B_5d55-060_120_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `1b1cbf35a394a08cca8d6a3b3f72083c` | TunerPro Binary Definition Map |
| `R4C9H6D7B_5d55-060_120_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `6f788f6845f6dfffa9f2d8c445d072df` | ASAM ASAP2 ECU Description File |
| `R4C9H6H7B_5d55-060_130_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `d9000d12d26c50b7177078ae4e1a54cf` | TunerPro Binary Definition Map |
| `R4C9H6H7B_5d55-060_130_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `738f711b96821a320a58c9bdfafc8cc0` | ASAM ASAP2 ECU Description File |
| `R4C9H6K5B_5d55-060_140_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `c1da9d01c3ecb6a0642e22aaeea4076e` | TunerPro Binary Definition Map |
| `R4C9H6K5B_5d55-060_140_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `5a9beabcea8d255b7f38756de5d05b23` | ASAM ASAP2 ECU Description File |
| `R4C9H6N7B_5d55-060_150_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `9dd9bc264e442f1dc1ae1b535181365d` | TunerPro Binary Definition Map |
| `R4C9H6N7B_5d55-060_150_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `8c9f15499d0829743781436155c182d9` | ASAM ASAP2 ECU Description File |
| `R4C9H6P7B_5d55-060_160_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `313f21f751480287c99cce2a6eb5e7b4` | TunerPro Binary Definition Map |
| `R4C9H6P7B_5d55-060_160_007_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `dbc922ddf862b29ec4a94d5140304566` | ASAM ASAP2 ECU Description File |
| `R4C9H6P9B_5d55-060_160_009_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `313f21f751480287c99cce2a6eb5e7b4` | TunerPro Binary Definition Map |
| `R4C9H6P9B_5d55-060_160_009_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `5430ebcd01d9e435fa374cb54febecc6` | ASAM ASAP2 ECU Description File |
| `R4C9H6S8B_5d55-060_170_008_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `285b5c646df20359c5ec892d13e57029` | TunerPro Binary Definition Map |
| `R4C9H6S8B_5d55-060_170_008_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `9d3b7fe3b8d0a4872bc0bbbb41db1fdc` | ASAM ASAP2 ECU Description File |
| `R4C9H6V5B_5d55-060_190_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `5d47cc6bd7b860b8c0e9f1bd7137e93f` | TunerPro Binary Definition Map |
| `R4C9H6V5B_5d55-060_190_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `95a086ac70cbb960b124f82d9a2c7585` | ASAM ASAP2 ECU Description File |
| `R4C9H6W5B_5d55-060_200_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.90 MB | `5d47cc6bd7b860b8c0e9f1bd7137e93f` | TunerPro Binary Definition Map |
| `R4C9H6W5B_5d55-060_200_005_v7.3.3.a2l` | **2015–2026** | 917.2 KB | `fd1e8cd6b8fcf85ee1bc0873613c56ce` | ASAM ASAP2 ECU Description File |
| `R4C9J718B_5d55-070_030_008_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `bb56c267d740c002b9b7fdb93b91a977` | TunerPro Binary Definition Map |
| `R4C9J718B_5d55-070_030_008_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `6a6fa0e92a931be02c440e5956e274a6` | ASAM ASAP2 ECU Description File |
| `R4C9J755B_5d55-070_040_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `7f74be34a31626c689fe8bf46d03a3ae` | TunerPro Binary Definition Map |
| `R4C9J755B_5d55-070_040_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `e39b9721c902e49038a7862c2761a867` | ASAM ASAP2 ECU Description File |
| `R4C9J756B_5d55-070_040_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `203315efa061ecd9abcd59626a84eacb` | TunerPro Binary Definition Map |
| `R4C9J756B_5d55-070_040_006_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `21901f91a4cd7a15e719c6eaefde6335` | ASAM ASAP2 ECU Description File |
| `R4C9J757B_5d55-070_050_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `203315efa061ecd9abcd59626a84eacb` | TunerPro Binary Definition Map |
| `R4C9J757B_5d55-070_050_007_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `2ea50d7a5eec91db8a237bbbb76db591` | ASAM ASAP2 ECU Description File |
| `R4C9J758B_5d55-070_050_008_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `339b0b29959bb96a0ea2024bbe93972f` | TunerPro Binary Definition Map |
| `R4C9J758B_5d55-070_050_008_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `ce13d4e16c810c6ecd286b1020f103f2` | ASAM ASAP2 ECU Description File |
| `R4C9J795B_5d55-070_060_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `24d735430776df967b74cd6bb9303a34` | TunerPro Binary Definition Map |
| `R4C9J795B_5d55-070_060_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `13d0db58c8aef17a96f7c277a8d813da` | ASAM ASAP2 ECU Description File |
| `R4C9J797B_5d55-070_060_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `12a6a12f2aa1bfc3b60a092f810c6799` | TunerPro Binary Definition Map |
| `R4C9J797B_5d55-070_060_007_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `fb436d4b307febbfd0a4882932159ab9` | ASAM ASAP2 ECU Description File |
| `R4C9J7A5B_5d55-070_070_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `12a6a12f2aa1bfc3b60a092f810c6799` | TunerPro Binary Definition Map |
| `R4C9J7A5B_5d55-070_070_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `c594c04d50d458d5d5389502d0768a5f` | ASAM ASAP2 ECU Description File |
| `R4C9J7N5B_5d55-070_080_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `0c24f294661dae4271a3f21984a8ba0a` | TunerPro Binary Definition Map |
| `R4C9J7N5B_5d55-070_080_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `fcc535a52cfc8fd3e0be8aa4a54dcb7f` | ASAM ASAP2 ECU Description File |
| `R4C9J7P7B_5d55-070_090_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `5fcc28dc7393c541a9dd066c101c59da` | TunerPro Binary Definition Map |
| `R4C9J7P7B_5d55-070_090_007_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `435b65568bc792f33ba5338fa84011d3` | ASAM ASAP2 ECU Description File |
| `R4C9J7P9B_5d55-070_090_009_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `5fcc28dc7393c541a9dd066c101c59da` | TunerPro Binary Definition Map |
| `R4C9J7P9B_5d55-070_090_009_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `921c3275c45e2b1203aa23b97f983b01` | ASAM ASAP2 ECU Description File |
| `R4C9J7S8B_5d55-070_100_008_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `c723afd78deec1f78bddcaf13cff05de` | TunerPro Binary Definition Map |
| `R4C9J7S8B_5d55-070_100_008_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `3002d32dfac910793514d3b0161b673c` | ASAM ASAP2 ECU Description File |
| `R4C9J7V5B_5d55-070_120_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `a9c2f874d49467cd878efd7663f903f1` | TunerPro Binary Definition Map |
| `R4C9J7V5B_5d55-070_120_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `351244cc25d9c674f94c473b236db825` | ASAM ASAP2 ECU Description File |
| `R4C9J7W5B_5d55-070_130_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.93 MB | `a9c2f874d49467cd878efd7663f903f1` | TunerPro Binary Definition Map |
| `R4C9J7W5B_5d55-070_130_005_v7.3.3.a2l` | **2015–2026** | 925.1 KB | `e8f19c4730036ca1027458c4a056d878` | ASAM ASAP2 ECU Description File |
| `R4C9L818B_5d55-080_030_008_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `aecb520d56a1bc41a70609e8bd409be7` | TunerPro Binary Definition Map |
| `R4C9L818B_5d55-080_030_008_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `d5edb77fe3ec48c6e5f9e8f146f00c57` | ASAM ASAP2 ECU Description File |
| `R4C9L856B_5d55-080_040_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `62e5e43bfa1fc21799f6a7399c122c73` | TunerPro Binary Definition Map |
| `R4C9L856B_5d55-080_040_006_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `152848a7e2c18756823fb982983b6fed` | ASAM ASAP2 ECU Description File |
| `R4C9L857B_5d55-080_040_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `0bb3433bd9a6573f52f0b9ce71ff5447` | TunerPro Binary Definition Map |
| `R4C9L857B_5d55-080_040_007_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `e55195609277da00ea0aa7b64344811f` | ASAM ASAP2 ECU Description File |
| `R4C9L875B_5d55-080_055_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `5ad4a6b062c68258d3aeb7d87d632f98` | TunerPro Binary Definition Map |
| `R4C9L875B_5d55-080_055_005_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `e7acc60de1a9b9ea57c508008cd0407a` | ASAM ASAP2 ECU Description File |
| `R4C9L8N5B_5d55-080_060_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `f44956dd0008cf621b97d03d47565ed8` | TunerPro Binary Definition Map |
| `R4C9L8N5B_5d55-080_060_005_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `28c6be476f5207d57148dbfc9f63cf82` | ASAM ASAP2 ECU Description File |
| `R4C9L8P7B_5d55-080_072_007_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `2ca8020f646295912bcd5965016c9c26` | TunerPro Binary Definition Map |
| `R4C9L8P7B_5d55-080_072_007_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `b61a530de2117320477ab96fab550dd3` | ASAM ASAP2 ECU Description File |
| `R4C9L8P9B_5d55-080_072_009_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `2ca8020f646295912bcd5965016c9c26` | TunerPro Binary Definition Map |
| `R4C9L8P9B_5d55-080_072_009_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `0bdbd56178dd9451dd637d720cf8b183` | ASAM ASAP2 ECU Description File |
| `R4C9L8PCB_5d55-080_072_012_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `fbe19fe18134553fc4852c3219f531fb` | TunerPro Binary Definition Map |
| `R4C9L8PCB_5d55-080_072_012_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `7750e59fd518a82185c3cde1342ec269` | ASAM ASAP2 ECU Description File |
| `R4C9L8S8B_5d55-080_080_008_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `22b72de42e69f854e041c06a936d1c12` | TunerPro Binary Definition Map |
| `R4C9L8S8B_5d55-080_080_008_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `307355f7dc6ae3a1fccc33d55f25515e` | ASAM ASAP2 ECU Description File |
| `R4C9L8V6B_5d55-080_100_006_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `65fd71ad7d75ea441176473361a93183` | TunerPro Binary Definition Map |
| `R4C9L8V6B_5d55-080_100_006_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `9bfb5355279559eb9467feb60275855a` | ASAM ASAP2 ECU Description File |
| `R4C9L8W9B_5d55-080_140_005_v7.3.3.ImperialUnits.xdf` | **2015–2026** | 2.92 MB | `0ecd3c954bcf6b530cbf1c19df9788fc` | TunerPro Binary Definition Map |
| `R4C9L8W9B_5d55-080_140_005_v7.3.3.a2l` | **2015–2026** | 920.5 KB | `fcb06a6ad3d2d314a022537bdeae7e3e` | ASAM ASAP2 ECU Description File |

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
