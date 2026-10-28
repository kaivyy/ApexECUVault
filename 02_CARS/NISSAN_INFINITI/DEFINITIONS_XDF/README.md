# DEFINITIONS_XDF - ECU Calibration Suite

**Repository Path**: `02_CARS/NISSAN_INFINITI/DEFINITIONS_XDF`  
**Classification**: `ECU Definition & Map Pack Suite (ASAP2 / WinOLS / TunerPro)`  
**Total Managed Assets**: `190 files` (0 binary dumps, 190 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `DEFINITIONS_XDF` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

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
| `1KA6A.xml` | **2000–2024** | 762 B | `eec0b9eb25966eb8fafeaa78df90df2a` | ECU / XML Calibration Map Definition |
| `1KE6C.xml` | **2000–2024** | 763 B | `64a691601da962b7f51da5881afbd799` | ECU / XML Calibration Map Definition |
| `1KE9C.xml` | **2000–2024** | 763 B | `ebb7f7492d92dbf889cbd7143fbbc0ee` | ECU / XML Calibration Map Definition |
| `1KN0B.xml` | **2000–2024** | 762 B | `c64b7b166c4b8303c92910296faac124` | ECU / XML Calibration Map Definition |
| `4ME6B.xml` | **2000–2024** | 762 B | `84fe123785d4b42b40f06a791375d573` | ECU / XML Calibration Map Definition |
| `5W502.xml` | **2000–2024** | 631 B | `f94eb68a09f005e65cfc34f1eb033f21` | ECU / XML Calibration Map Definition |
| `5Y005.xml` | **2000–2024** | 712 B | `36458145e9c64d3384e85950e2cfd066` | ECU / XML Calibration Map Definition |
| `5Y700.xml` | **2000–2024** | 714 B | `2d2ba9d8e3c44bd40f7eb298fe2894f6` | ECU / XML Calibration Map Definition |
| `5Y701.xml` | **2000–2024** | 420 B | `e8766bd08c99dd9e969064966620ce7e` | ECU / XML Calibration Map Definition |
| `5Y702.xml` | **2000–2024** | 398 B | `0f1f14633ddf862a7f3cad1915e45182` | ECU / XML Calibration Map Definition |
| `5Y703.xml` | **2000–2024** | 395 B | `293baa98b8acfbf02975cd2fd42d3a44` | ECU / XML Calibration Map Definition |
| `5Y711.xml` | **2000–2024** | 493 B | `d99f48b3088d33dba5a8d56ec55cc1de` | ECU / XML Calibration Map Definition |
| `5Y712.xml` | **2000–2024** | 421 B | `5b2a8eb2aa8d14120a151e97e78a7d60` | ECU / XML Calibration Map Definition |
| `5Y713.xml` | **2000–2024** | 395 B | `1a38569665457078717b744063c42512` | ECU / XML Calibration Map Definition |
| `5Y724.xml` | **2000–2024** | 7.9 KB | `058faa3192efcd08bde424c797868c21` | ECU / XML Calibration Map Definition |
| `6W505.xml` | **2000–2024** | 3.7 KB | `9aa197f7723452acd177738da697b104` | ECU / XML Calibration Map Definition |
| `6W570.xml` | **2000–2024** | 714 B | `1833e6cab4a4246e38d1242f44e313e2` | ECU / XML Calibration Map Definition |
| `6Y300.xml` | **2000–2024** | 791 B | `e073907cc69599f7d69a1c6a5ca68ead` | ECU / XML Calibration Map Definition |
| `6Y303.xml` | **2000–2024** | 395 B | `25c41cbee081265ebf2f0e7efbb229c3` | ECU / XML Calibration Map Definition |
| `6Y310.xml` | **2000–2024** | 710 B | `5f203e243130f390f8a6b6cef74d5204` | ECU / XML Calibration Map Definition |
| `6Y314.xml` | **2000–2024** | 395 B | `a23d4cae44576ee05743d651f5dd1d07` | ECU / XML Calibration Map Definition |
| `6Y321.xml` | **2000–2024** | 598 B | `5c89a3f6c2a63a48b3b921d9345fb556` | ECU / XML Calibration Map Definition |
| `6Y324.xml` | **2000–2024** | 4.7 KB | `652452b991ea710a2a264308b15aeb15` | ECU / XML Calibration Map Definition |
| `6Z55A.xml` | **2000–2024** | 7.6 KB | `843a83fefd02008cd30d8291bddf7706` | ECU / XML Calibration Map Definition |
| `6Z68A.xml` | **2000–2024** | 796 B | `65c2416e7f42ca44be4bcb4018b9bfc0` | ECU / XML Calibration Map Definition |
| `7S875.xml` | **2000–2024** | 7.8 KB | `685aac9042b19ea361f337da2d3f926b` | ECU / XML Calibration Map Definition |
| `7Y001.xml` | **2000–2024** | 711 B | `dc7847ab748d28a9e004ab4056a4ed35` | ECU / XML Calibration Map Definition |
| `7Y006.xml` | **2000–2024** | 396 B | `ee93c3458ca9f19845afce43cdb71b2e` | ECU / XML Calibration Map Definition |
| `7Y210.xml` | **2000–2024** | 3.1 KB | `ef2bc873ea43eacded4a31d5f61e2383` | ECU / XML Calibration Map Definition |
| `8J160.xml` | **2000–2024** | 367 B | `91b698d3c9de588b599354dea445b533` | ECU / XML Calibration Map Definition |
| `8J164.xml` | **2000–2024** | 7.1 KB | `baaafaaf393e487ddac773a8f53771dd` | ECU / XML Calibration Map Definition |
| `8U023.xml` | **2000–2024** | 397 B | `38ddd65cb0d4fec53fa56d4fe0d0d33d` | ECU / XML Calibration Map Definition |
| `8U073.xml` | **2000–2024** | 397 B | `87fe3966344722ae640e794e0ba4587d` | ECU / XML Calibration Map Definition |
| `8U07A.xml` | **2000–2024** | 3.1 KB | `01e1282e6975b04a977ff46a9b0c3b30` | ECU / XML Calibration Map Definition |
| `8U07B.xml` | **2000–2024** | 395 B | `00fb1f35ea49b6eb0524b9eeef70b6d5` | ECU / XML Calibration Map Definition |
| `8U320.xml` | **2000–2024** | 707 B | `7cba59eb1d2484b1c5e2d77dff7b9bad` | ECU / XML Calibration Map Definition |
| `8U42D.xml` | **2000–2024** | 2.6 KB | `6c81569a177e05dfd29b3bcb60153be6` | ECU / XML Calibration Map Definition |
| `8U50B.xml` | **2000–2024** | 395 B | `53ad6fe042b8024a9e03918e10820ac5` | ECU / XML Calibration Map Definition |
| `8U51B.xml` | **2000–2024** | 397 B | `904ea3e0e28162b3aabe0aa3a9a3dc51` | ECU / XML Calibration Map Definition |
| `8U523.xml` | **2000–2024** | 397 B | `a870e2a394f6530d8ac3c6a02cb4dee8` | ECU / XML Calibration Map Definition |
| `8U52B.xml` | **2000–2024** | 4.7 KB | `f5f8c149c97bf47dcfa35fe1a381e6bf` | ECU / XML Calibration Map Definition |
| `8U901.xml` | **2000–2024** | 394 B | `afbed86d17eda12f6324d8c09be3d965` | ECU / XML Calibration Map Definition |
| `8U906.xml` | **2000–2024** | 3.8 KB | `905d85941463feffb65d5e1829aa08ff` | ECU / XML Calibration Map Definition |
| `8U92A.xml` | **2000–2024** | 3.5 KB | `5c542a743b800986bbd813d2fc226e8d` | ECU / XML Calibration Map Definition |
| `8Y004.xml` | **2000–2024** | 715 B | `aad17a65c48fff7d60600f0c590dae5b` | ECU / XML Calibration Map Definition |
| `8Y106.xml` | **2000–2024** | 2.6 KB | `ac0249e0535307836ed74ff59c408dd6` | ECU / XML Calibration Map Definition |
| `9DA0D.xml` | **2000–2024** | 623 B | `3cf263a0a76e01fa87276a9a25a1d1fd` | ECU / XML Calibration Map Definition |
| `9J003.xml` | **2000–2024** | 5.9 KB | `63bd4c63cbffa31d170890b2aa8a6ad0` | ECU / XML Calibration Map Definition |
| `9J074.xml` | **2000–2024** | 5.0 KB | `010a3bce6816c386a20c43f32143b082` | ECU / XML Calibration Map Definition |
| `9J081.xml` | **2000–2024** | 395 B | `22270a40894281f6801cc3731615eec6` | ECU / XML Calibration Map Definition |
| `9W400.xml` | **2000–2024** | 709 B | `a5a14ca424e9520a502fc7c5ba3ee71a` | ECU / XML Calibration Map Definition |
| `9W73B.xml` | **2000–2024** | 627 B | `7a1f42b0dbbbc98d955cc1ed497daecc` | ECU / XML Calibration Map Definition |
| `9W84A.xml` | **2000–2024** | 8.7 KB | `840d6cefc02e15af65a9771a50921997` | ECU / XML Calibration Map Definition |
| `9Y410.xml` | **2000–2024** | 709 B | `d5140605eda8063a1860d55336d72d8f` | ECU / XML Calibration Map Definition |
| `9Y412.xml` | **2000–2024** | 709 B | `b0aa8c6b07ebd33e8dfb6727eb867f77` | ECU / XML Calibration Map Definition |
| `9Y510.xml` | **2000–2024** | 714 B | `354c6924ab3d0d2ab141db88999883ef` | ECU / XML Calibration Map Definition |
| `A2L.xml` | **2000–2024** | 134.9 KB | `2e335cc9d485b3dd751009cea54d70c7` | ECU / XML Calibration Map Definition |
| `AC011.xml` | **2000–2024** | 8.1 KB | `7e1ea640610a1511f210771412386c73` | ECU / XML Calibration Map Definition |
| `AC012.xml` | **2000–2024** | 8.4 KB | `ca67de1faec2b46bf9c50e25c33a389a` | ECU / XML Calibration Map Definition |
| `AC200.xml` | **2000–2024** | 470 B | `4d71edacb390c4dc5e00fa4b73655ec1` | ECU / XML Calibration Map Definition |
| `AC300.xml` | **2000–2024** | 390 B | `4cf1f67d2149e8a97be002fb4d5da394` | ECU / XML Calibration Map Definition |
| `AC301.xml` | **2000–2024** | 390 B | `5ae64ee32bfe08115722d57ba7fd1759` | ECU / XML Calibration Map Definition |
| `AC305.xml` | **2000–2024** | 390 B | `0522dc815baac93429dbbc6c7e90295b` | ECU / XML Calibration Map Definition |
| `AC306.xml` | **2000–2024** | 390 B | `80a89cb21c6efddafb7d903ad496c760` | ECU / XML Calibration Map Definition |
| `AC30A.xml` | **2000–2024** | 390 B | `40739a2d76a8312200fa3a1100fbecac` | ECU / XML Calibration Map Definition |
| `AC31A.xml` | **2000–2024** | 9.3 KB | `5710636752b88eb409ddb0c22b20cc75` | ECU / XML Calibration Map Definition |
| `AC400.xml` | **2000–2024** | 388 B | `13bb2637122767a8eaa49c619f425742` | ECU / XML Calibration Map Definition |
| `AC401.xml` | **2000–2024** | 395 B | `cf8530fc9b2660f7bdae5caf21ba33db` | ECU / XML Calibration Map Definition |
| `AC405.xml` | **2000–2024** | 388 B | `a25df64b62e7bcfb040a078e7631521c` | ECU / XML Calibration Map Definition |
| `AC406.xml` | **2000–2024** | 395 B | `cccc7fd8b53a8e9011b665a215574a71` | ECU / XML Calibration Map Definition |
| `AC40A.xml` | **2000–2024** | 388 B | `587b757c5d0c2756d09a49adac987596` | ECU / XML Calibration Map Definition |
| `AC510.xml` | **2000–2024** | 402 B | `0573311c214a46e19393ee37df8acb78` | ECU / XML Calibration Map Definition |
| `AC610.xml` | **2000–2024** | 601 B | `5238890d38a04b7c6aea8a9640052b6b` | ECU / XML Calibration Map Definition |
| `AC700.xml` | **2000–2024** | 386 B | `7cb258adc2be2807ae556e38b9e7e656` | ECU / XML Calibration Map Definition |
| `AC705.xml` | **2000–2024** | 389 B | `fe4bbc8114c9dcd2d2fced58321422d9` | ECU / XML Calibration Map Definition |
| `AC810.xml` | **2000–2024** | 394 B | `421499a83b481a40e3e24adc58b58d9f` | ECU / XML Calibration Map Definition |
| `AC81A.xml` | **2000–2024** | 9.4 KB | `571660d3b2922997f2da214925f51c8e` | ECU / XML Calibration Map Definition |
| `AL902.xml` | **2000–2024** | 711 B | `5dd2b61f522c73e223e20f6030dcb318` | ECU / XML Calibration Map Definition |
| `AM603.xml` | **2000–2024** | 8.0 KB | `cb49b074c8ddf5657f4d63bf7b5749b5` | ECU / XML Calibration Map Definition |
| `AM604.xml` | **2000–2024** | 7.7 KB | `6ffb6637b104ee2f8542be147f53b0f4` | ECU / XML Calibration Map Definition |
| `AM607.xml` | **2000–2024** | 395 B | `aac6bea62ab4c0b49057a2bcb1876541` | ECU / XML Calibration Map Definition |
| `AM900.xml` | **2000–2024** | 393 B | `fe5b0a8d2713e1016c28e2a8bffe4254` | ECU / XML Calibration Map Definition |
| `AM905.xml` | **2000–2024** | 6.1 KB | `54f52f011beb4fb445e3fd50203a8a7a` | ECU / XML Calibration Map Definition |
| `AM90A.xml` | **2000–2024** | 401 B | `4a0004869ce0103961c3e6c24c0d2b76` | ECU / XML Calibration Map Definition |
| `AM91A.xml` | **2000–2024** | 3.2 KB | `b7b72e4e4c8a9a7e99ba1c5c11134f27` | ECU / XML Calibration Map Definition |
| `AQ001.xml` | **2000–2024** | 708 B | `8a946860e5ac3ef6c507371e4376cf9e` | ECU / XML Calibration Map Definition |
| `AQ806.xml` | **2000–2024** | 798 B | `ea88ca571d46009707c77067ea1d0d8f` | ECU / XML Calibration Map Definition |
| `AQ860.xml` | **2000–2024** | 2.6 KB | `6a52a10c590837b5b9c116c4c9ef10c4` | ECU / XML Calibration Map Definition |
| `AZ01A.xml` | **2000–2024** | 581 B | `3926499759c050f50c13b6c7a054ca49` | ECU / XML Calibration Map Definition |
| `CC00A.xml` | **2000–2024** | 715 B | `8351f68edeed2c8d4b2634fc0f9bf0d4` | ECU / XML Calibration Map Definition |
| `CC00B.xml` | **2000–2024** | 715 B | `73515d60cb5c7032bab05cd94d832092` | ECU / XML Calibration Map Definition |
| `CC020.xml` | **2000–2024** | 715 B | `70bf43561c4c4a3da2920dca36d16704` | ECU / XML Calibration Map Definition |
| `CC02A.xml` | **2000–2024** | 715 B | `2e441c4edf214130953ce677a08e43da` | ECU / XML Calibration Map Definition |
| `CC06A.xml` | **2000–2024** | 715 B | `00700f0824f8f412be3c45c035f47acd` | ECU / XML Calibration Map Definition |
| `CD000.xml` | **2000–2024** | 740 B | `4994d1737d85f0f326d2c333a89d6e01` | ECU / XML Calibration Map Definition |
| `CD001.xml` | **2000–2024** | 571 B | `a51cc414c6ed3f7f83db1f7f98a43557` | ECU / XML Calibration Map Definition |
| `CD002.xml` | **2000–2024** | 571 B | `9bed0b2457c7704619f062f3f430745d` | ECU / XML Calibration Map Definition |
| `CD003.xml` | **2000–2024** | 571 B | `946ab83f7feba77fe848f2f795e7f556` | ECU / XML Calibration Map Definition |
| `CD006.xml` | **2000–2024** | 565 B | `be9141a7db593d5d1998a1dfed0e11ae` | ECU / XML Calibration Map Definition |
| `CD007.xml` | **2000–2024** | 565 B | `2e0fddf911d3c9375065464f06f14e56` | ECU / XML Calibration Map Definition |
| `CD008.xml` | **2000–2024** | 567 B | `30bf31d2570987eed8b8a2ce22905f97` | ECU / XML Calibration Map Definition |
| `CD100.xml` | **2000–2024** | 391 B | `bfc90dfb48285fb5d23566c662e31043` | ECU / XML Calibration Map Definition |
| `CD101.xml` | **2000–2024** | 391 B | `2d83ce25869391c08cb231a267bf90ef` | ECU / XML Calibration Map Definition |
| `CD102.xml` | **2000–2024** | 8.3 KB | `3c1e49804ad47c04c0863a5c22bb7562` | ECU / XML Calibration Map Definition |
| `CD405.xml` | **2000–2024** | 389 B | `ce0e711be6bad95929899ac3e82bf68c` | ECU / XML Calibration Map Definition |
| `CD406.xml` | **2000–2024** | 391 B | `78f728f087db3971d44ac2363589333e` | ECU / XML Calibration Map Definition |
| `CD415.xml` | **2000–2024** | 7.1 KB | `9e605303a2fd356a79d7b9e3c74502c6` | ECU / XML Calibration Map Definition |
| `CD416.xml` | **2000–2024** | 4.4 KB | `5ed5c2e6e73fc47ff5520d897313ffb9` | ECU / XML Calibration Map Definition |
| `CD515.xml` | **2000–2024** | 8.6 KB | `77e820743b6180d6bdae1fdb59e8b911` | ECU / XML Calibration Map Definition |
| `CD700.xml` | **2000–2024** | 393 B | `caceeade17c0349554ecd407e6134647` | ECU / XML Calibration Map Definition |
| `CD800.xml` | **2000–2024** | 436 B | `ba453ad242fa1353c1d0a4466b8c0e73` | ECU / XML Calibration Map Definition |
| `CE405.xml` | **2000–2024** | 10.1 KB | `08a1ab5d9a8f6ffca34ff1cf4192327c` | ECU / XML Calibration Map Definition |
| `CE406.xml` | **2000–2024** | 1.1 KB | `05472e9e2a8a2d4a1e1b4ef9a240015f` | ECU / XML Calibration Map Definition |
| `CE805.xml` | **2000–2024** | 390 B | `439a0c15481b8ac743bfec2dc79ddb21` | ECU / XML Calibration Map Definition |
| `CE806.xml` | **2000–2024** | 8.9 KB | `3843878bb08210bc7f537a697bf71af4` | ECU / XML Calibration Map Definition |
| `CE810.xml` | **2000–2024** | 8.9 KB | `205e6075321c10f1e8474d96b5709f13` | ECU / XML Calibration Map Definition |
| `CE811.xml` | **2000–2024** | 9.6 KB | `f3d9ca5e5d2bce89ed0e6d523036b95d` | ECU / XML Calibration Map Definition |
| `CE860.xml` | **2000–2024** | 5.3 KB | `c5bd45679006168df10dba4de437370f` | ECU / XML Calibration Map Definition |
| `CF000.xml` | **2000–2024** | 9.1 KB | `f24b7949729f390623dc32e685b758d8` | ECU / XML Calibration Map Definition |
| `CF010.xml` | **2000–2024** | 397 B | `20fd12ce0db0f370010f3f2e85dab9fc` | ECU / XML Calibration Map Definition |
| `CF020.xml` | **2000–2024** | 520 B | `8eef73c7907ccfd0b27520fb4c59fb56` | ECU / XML Calibration Map Definition |
| `CF065.xml` | **2000–2024** | 12.9 KB | `aba49000729865725b37d62c2c69f15c` | ECU / XML Calibration Map Definition |
| `CF115.xml` | **2000–2024** | 14.4 KB | `6f74c5bf1ad382c27ea5f0b9b114e67b` | ECU / XML Calibration Map Definition |
| `CF170.xml` | **2000–2024** | 8.6 KB | `8228a9edef1c69228ccbe324f9fb9ff2` | ECU / XML Calibration Map Definition |
| `CF40A.xml` | **2000–2024** | 617 B | `962b0f685561aedfd4f30753e53ce212` | ECU / XML Calibration Map Definition |
| `CF40C.xml` | **2000–2024** | 390 B | `82bebd90bd2a943462bdbd8be245d8c7` | ECU / XML Calibration Map Definition |
| `CF40D.xml` | **2000–2024** | 12.7 KB | `b6b2c170475494fe263af881e587cdaa` | ECU / XML Calibration Map Definition |
| `CF40E.xml` | **2000–2024** | 793 B | `9a3488e43d7bcc2ef2d935a0304b2ec5` | ECU / XML Calibration Map Definition |
| `CF41A.xml` | **2000–2024** | 613 B | `00a83bbe80c5294417e2ef6f48d3ad16` | ECU / XML Calibration Map Definition |
| `CF41B.xml` | **2000–2024** | 613 B | `a906480fee96b268b22f7de36c0fb65e` | ECU / XML Calibration Map Definition |
| `CF41D.xml` | **2000–2024** | 613 B | `589b3d199e76d533726130c7ca80b0e5` | ECU / XML Calibration Map Definition |
| `CF41E.xml` | **2000–2024** | 5.0 KB | `7142695ef357e84241e1c620e2d0bcc4` | ECU / XML Calibration Map Definition |
| `CF42A.xml` | **2000–2024** | 394 B | `7d15ed1feb9c98a106bd97202db42efe` | ECU / XML Calibration Map Definition |
| `CF42C.xml` | **2000–2024** | 10.6 KB | `bd613ca7ce79b918127e6cc1534e0d28` | ECU / XML Calibration Map Definition |
| `CF43A.xml` | **2000–2024** | 569 B | `d1d29aa04aa503b25364d7ce0c794caa` | ECU / XML Calibration Map Definition |
| `CF43D.xml` | **2000–2024** | 14.9 KB | `71a5e22e1570ba8700708111abb3d954` | ECU / XML Calibration Map Definition |
| `CF44A.xml` | **2000–2024** | 402 B | `5c21bc1a1601ed446a00c12c96e975e6` | ECU / XML Calibration Map Definition |
| `CF44B.xml` | **2000–2024** | 636 B | `cc8e4a7f0014b03633d5bf5419f99fa2` | ECU / XML Calibration Map Definition |
| `CF44C.xml` | **2000–2024** | 636 B | `93ce64d78ac3621366d677ada184979f` | ECU / XML Calibration Map Definition |
| `CF44D.xml` | **2000–2024** | 608 B | `61da2875bbdeeb78b7357c81b23746f4` | ECU / XML Calibration Map Definition |
| `CF48D.xml` | **2000–2024** | 17.4 KB | `9829f2bda69c23ddfc6b3e1d4c6da7f2` | ECU / XML Calibration Map Definition |
| `CF49A.xml` | **2000–2024** | 17.7 KB | `2901370e500add5ebeedbfd0c3e7672b` | ECU / XML Calibration Map Definition |
| `CF50A.xml` | **2000–2024** | 687 B | `4d363f8bccdf00a7865896f5e34bc083` | ECU / XML Calibration Map Definition |
| `CF90A.xml` | **2000–2024** | 570 B | `573a6cd20a8253f5d3f49d7d417d5c16` | ECU / XML Calibration Map Definition |
| `CF92A.xml` | **2000–2024** | 10.3 KB | `7eff4f423c339c073eccb1250269a1f0` | ECU / XML Calibration Map Definition |
| `CL110.xml` | **2000–2024** | 9.3 KB | `068072795d9fc200f0c6a2bd6110dfd5` | ECU / XML Calibration Map Definition |
| `CL72A.xml` | **2000–2024** | 537 B | `a2900d0fb0a32dbe53dfd8f18fd4364a` | ECU / XML Calibration Map Definition |
| `CM30A.xml` | **2000–2024** | 392 B | `d28abef0408a23ce8f7e65b50008bbe8` | ECU / XML Calibration Map Definition |
| `CM30B.xml` | **2000–2024** | 398 B | `a92f428286a379bfa4ec2bd782677866` | ECU / XML Calibration Map Definition |
| `CM30C.xml` | **2000–2024** | 670 B | `5c2641d76f43b61101e1bee4474fcd4b` | ECU / XML Calibration Map Definition |
| `CM31C.xml` | **2000–2024** | 390 B | `595277d2ba30ed2830e99407b227d806` | ECU / XML Calibration Map Definition |
| `CM32B.xml` | **2000–2024** | 394 B | `30de24f2eef44237b5db4eb96c4563f2` | ECU / XML Calibration Map Definition |
| `CM32C.xml` | **2000–2024** | 662 B | `be5422cf49d78778fc6b6bc37898cb41` | ECU / XML Calibration Map Definition |
| `CM37A.xml` | **2000–2024** | 396 B | `106d3b2632285e79fad21dc98528fdc8` | ECU / XML Calibration Map Definition |
| `CM40A.xml` | **2000–2024** | 392 B | `01effb72cb0340b4ab7302563052c1ab` | ECU / XML Calibration Map Definition |
| `CM40B.xml` | **2000–2024** | 392 B | `366e1bdec7dbbce861341281c4e39986` | ECU / XML Calibration Map Definition |
| `CM40C.xml` | **2000–2024** | 392 B | `b42ddfc7f045ab6a5a8666db720ce715` | ECU / XML Calibration Map Definition |
| `CM41A.xml` | **2000–2024** | 390 B | `992435bc7dbfaed30b2c01762a97fbbb` | ECU / XML Calibration Map Definition |
| `CM41B.xml` | **2000–2024** | 390 B | `ae16c4399b1e977677aa4d94e5fa60cc` | ECU / XML Calibration Map Definition |
| `CM41C.xml` | **2000–2024** | 390 B | `dc4129edc9020b0cc09da0d2ac243af0` | ECU / XML Calibration Map Definition |
| `EC80A.xml` | **2000–2024** | 642 B | `dd0fe6d5eb732e6df90d2df8468f88df` | ECU / XML Calibration Map Definition |
| `EC82A.xml` | **2000–2024** | 720 B | `cf7b69d55824e42c2ea964919bbea056` | ECU / XML Calibration Map Definition |
| `EC87A.xml` | **2000–2024** | 720 B | `b9b5b89a7e6656183c5683a86f9a6c4e` | ECU / XML Calibration Map Definition |
| `EM62B.xml` | **2000–2024** | 769 B | `244d91bbae41cb2bdb312e19a7a5dea0` | ECU / XML Calibration Map Definition |
| `EM63A.xml` | **2000–2024** | 720 B | `66850a14c21bd08ad0b4be5c528c310d` | ECU / XML Calibration Map Definition |
| `EV13B.xml` | **2000–2024** | 389 B | `394a781162aca0e74e7b7e5f5fc71228` | ECU / XML Calibration Map Definition |
| `EV15A.xml` | **2000–2024** | 2.6 KB | `33560b8c78d29a98b90457cb796eee6e` | ECU / XML Calibration Map Definition |
| `EV16A.xml` | **2000–2024** | 393 B | `b069a8731d7bba57ef537bde98a40da4` | ECU / XML Calibration Map Definition |
| `EV18A.xml` | **2000–2024** | 12.5 KB | `cf30c426e12f339dce67059933d7c2fb` | ECU / XML Calibration Map Definition |
| `EV19B.xml` | **2000–2024** | 828 B | `ac503cb8513fa72e3fb1ba996d5149a7` | ECU / XML Calibration Map Definition |
| `JK03A.xml` | **2000–2024** | 759 B | `ede92fd8a67ec35a35f2fdd52fd51933` | ECU / XML Calibration Map Definition |
| `M5113.xml` | **2000–2024** | 12.0 KB | `117b9a5b0c80c9c2ac522b33f0092001` | ECU / XML Calibration Map Definition |
| `ScalingData.xml` | **2000–2024** | 57.7 KB | `4bfa888d3c1826e1601053ae0c6dd353` | ECU / XML Calibration Map Definition |
| `ZB010.xml` | **2000–2024** | 791 B | `114765ccab59efd3ddac33c5c6774de6` | ECU / XML Calibration Map Definition |
| `ZB070.xml` | **2000–2024** | 14.6 KB | `09ffb5ff3db08f75d60a7b771c83eae3` | ECU / XML Calibration Map Definition |
| `ZB075.xml` | **2000–2024** | 537 B | `0575bca18b227041b4fe8d5d7720ba2d` | ECU / XML Calibration Map Definition |
| `ZC060.xml` | **2000–2024** | 705 B | `9eb05798bfe3c9a7f4683d318463d0a1` | ECU / XML Calibration Map Definition |
| `ZC070.xml` | **2000–2024** | 618 B | `842557193fbf01fb85cf2685b6fb278b` | ECU / XML Calibration Map Definition |
| `ZD85E.xml` | **2000–2024** | 716 B | `371b030ebdf84522021fb192f393f389` | ECU / XML Calibration Map Definition |
| `ZD89A.xml` | **2000–2024** | 397 B | `cfbc57aa57a02b8f881b9c6d80d7de20` | ECU / XML Calibration Map Definition |
| `ZG59B.xml` | **2000–2024** | 12.5 KB | `364712f3d72e86c7d7283a76960ddcc8` | ECU / XML Calibration Map Definition |
| `ZH98A.xml` | **2000–2024** | 392 B | `81fb8e4f50c039c9629eb6cb91c6fb0e` | ECU / XML Calibration Map Definition |
| `ZH98C.xml` | **2000–2024** | 392 B | `11d8e3c3852d122c662999ad24fbe2a1` | ECU / XML Calibration Map Definition |
| `ZH99A.xml` | **2000–2024** | 391 B | `655617e43521faff979f856100c11ea4` | ECU / XML Calibration Map Definition |
| `ZJ05B.xml` | **2000–2024** | 7.2 KB | `2d0c975ab07b770a33d9018d35a85da0` | ECU / XML Calibration Map Definition |
| `ZK01B.xml` | **2000–2024** | 393 B | `07365df3ff5aad5c7c6816e46e2a0416` | ECU / XML Calibration Map Definition |
| `ZK03A.xml` | **2000–2024** | 712 B | `e80c815efaf99de3b5faf5067f2c5114` | ECU / XML Calibration Map Definition |
| `ZR35B.xml` | **2000–2024** | 3.0 KB | `6f4585626d08e1168ea91b29e343fde7` | ECU / XML Calibration Map Definition |
| `ZX10B.xml` | **2000–2024** | 821 B | `7da979eb090f8c714bffb85be4fa95ab` | ECU / XML Calibration Map Definition |
| `ZY70A.xml` | **2000–2024** | 758 B | `c608831259bc54dbea9958bcf9088f6c` | ECU / XML Calibration Map Definition |

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
