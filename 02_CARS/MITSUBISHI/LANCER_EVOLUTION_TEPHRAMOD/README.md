# LANCER EVOLUTION TEPHRAMOD - ECU Calibration Suite

**Repository Path**: `02_CARS/MITSUBISHI/LANCER_EVOLUTION_TEPHRAMOD`  
**Classification**: `TunerPro Definition Map Suite (XDF Only)`  
**Total Managed Assets**: `142 files` (0 binary dumps, 142 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `LANCER_EVOLUTION_TEPHRAMOD` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2001–2007

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `22580006 1998 JDM Lancer Evo 5 GSR.xml` | **1998** | 15.4 KB | `30f31ddf7a6124181082f56334758003` | ECU / ASAP2 Calibration Map Definition |
| `22580007 1998 JDM Lancer Evo 5 GSR.xml` | **1998** | 17.1 KB | `e5e07ca6aae17740b9193923bd2cbc69` | ECU / ASAP2 Calibration Map Definition |
| `23490006 1998-1999 JDM Lancer Evo 5-6.xml` | **1998–1999** | 17.1 KB | `7c592959a93d842b9cb301d22f66c968` | ECU / ASAP2 Calibration Map Definition |
| `23490007 1998 JDM Lanver Evo 5.xml` | **1998** | 15.0 KB | `d5264166994a9826a1bc0adcbd8b6925` | ECU / ASAP2 Calibration Map Definition |
| `24430002 1999 JDM Lancer Evo 6 RS.xml` | **1999** | 17.4 KB | `15db82d82bad330ed47934d850382f78` | ECU / ASAP2 Calibration Map Definition |
| `24440002 1999 JDM Lancer Evo 6 GSR.xml` | **1999** | 17.0 KB | `358c641f7613c422fb7547f4c37b44a7` | ECU / ASAP2 Calibration Map Definition |
| `25570000 1998-1999 JDM Lanver Evo 5-6 Ralliart MT.xml` | **1998–1999** | 16.6 KB | `3bc8f594004bd5cdd44ba759b9acc0f6` | ECU / ASAP2 Calibration Map Definition |
| `25580000 1999 JDM Lancer Evo 6 RSII MT.xml` | **1999** | 15.4 KB | `c0084d9504f2401fa6b7f003b335aa3a` | ECU / ASAP2 Calibration Map Definition |
| `25770000 1998-1999 JDM Lancer Evo 5-6.xml` | **1998–1999** | 17.9 KB | `147236de2219e140da70ce9157ac5043` | ECU / ASAP2 Calibration Map Definition |
| `27370001 2000 JDM Lancer Evo TME GSR.xml` | **2000** | 17.6 KB | `9a0b8497ec9afdb0fbdc28b0322b6ac2` | ECU / ASAP2 Calibration Map Definition |
| `27380001 2000 JDM Lancer Evo TME RS.xml` | **2000** | 16.3 KB | `2927818ddd7ecbfc33167864254417fb` | ECU / ASAP2 Calibration Map Definition |
| `50845084 2014 EDM Lancer Evolution X 5MT.xml` | **2014** | 13.8 KB | `7175d1530d7b98005eaa5a521b55a642` | ECU / ASAP2 Calibration Map Definition |
| `52350012 2008 JDM Lancer Evolution X 5MT.xml` | **2008** | 12.3 KB | `d0741e44f49f343169705416523bf712` | ECU / ASAP2 Calibration Map Definition |
| `52350018 2008 JDM Lancer Evolution X 5MT.xml` | **2008** | 20.2 KB | `2647019b82226ab567667e86f8ef5db3` | ECU / ASAP2 Calibration Map Definition |
| `52360016 2008 JDM Lancer Evolution X 5MT.xml` | **2008** | 12.3 KB | `aed336b408a2eadbe52dabb728e7cac2` | ECU / ASAP2 Calibration Map Definition |
| `52360018 2008 JDM Lancer Evolution X 5MT.xml` | **2008** | 22.8 KB | `1cf1080a753febbb9bc6e36fa248f5c3` | ECU / ASAP2 Calibration Map Definition |
| `52370023 2008 JDM Lancer Evolution X SST.xml` | **2008** | 15.0 KB | `eee9b6085feb8762dd36c148f89b4f4d` | ECU / ASAP2 Calibration Map Definition |
| `52370024 2008 JDM Lancer Evolution X SST.xml` | **2008** | 27.1 KB | `65009ba39ea670a28285d38f1f91cea3` | ECU / ASAP2 Calibration Map Definition |
| `52550003 2008 EDM Lancer Evolution X 5MT.xml` | **2008** | 12.5 KB | `af01de18c983006b8dc09cb4dd546111` | ECU / ASAP2 Calibration Map Definition |
| `52680015 2008 USDM Lancer Evolution X 5MT.xml` | **2008** | 29.3 KB | `adf4b4d45d83adfa63dabe41c469c788` | ECU / ASAP2 Calibration Map Definition |
| `52680016 2008 USDM Lancer Evolution X 5MT.xml` | **2008** | 918 B | `73d35f1cf93b34b25cfac41add4e2154` | ECU / ASAP2 Calibration Map Definition |
| `52680017 2008 USDM Lancer Evolution X 5MT.xml` | **2008** | 918 B | `c6ef328700f42dd8132dbdea6aae02db` | ECU / ASAP2 Calibration Map Definition |
| `52680018 2008 USDM Lancer Evolution X 5MT.xml` | **2008** | 918 B | `f5b160ab8680c144e7a575b230c26ae3` | ECU / ASAP2 Calibration Map Definition |
| `52680019 2008 USDM Lancer Evolution X 5MT.xml` | **2008** | 918 B | `5755180351bfd780030955ab8a9e7b56` | ECU / ASAP2 Calibration Map Definition |
| `52680020 2008 USDM Lancer Evolution X 5MT.xml` | **2008** | 918 B | `089bbe5719f9aa96f6b1d483c8d30816` | ECU / ASAP2 Calibration Map Definition |
| `52680022 2008 USDM Lancer Evolution X 5MT.xml` | **2008** | 918 B | `432b96609cb28e285fb14ec8433cb1d2` | ECU / ASAP2 Calibration Map Definition |
| `52680024 2008 USDM Lancer Evolution X 5MT.xml` | **2008** | 23.1 KB | `d8383068f9041654718986360e7b730b` | ECU / ASAP2 Calibration Map Definition |
| `52690019 2008 USDM Lancer Evolution X SST.xml` | **2008** | 33.3 KB | `5d3bdce6675d6057ca996885f83d11a2` | ECU / ASAP2 Calibration Map Definition |
| `52690021 2008 USDM Lancer Evolution X SST.xml` | **2008** | 918 B | `f4280cf31f32f590ec87f3bf7f14d0ec` | ECU / ASAP2 Calibration Map Definition |
| `52690022 2008 USDM Lancer Evolution X SST.xml` | **2008** | 918 B | `0e07e4a413bef41155b8d0b0c97a12de` | ECU / ASAP2 Calibration Map Definition |
| `52690024 2008 USDM Lancer Evolution X SST.xml` | **2008** | 22.3 KB | `114a6f3fa82c2e0c9d98f0ae79902ba4` | ECU / ASAP2 Calibration Map Definition |
| `53040007 2008 EDM Lancer Evolution X 5MT.xml` | **2008** | 14.0 KB | `47830c5368dcdbbf1cdb06c7f81a48d3` | ECU / ASAP2 Calibration Map Definition |
| `53040008 2008 EDM Lancer Evolution X 5MT.xml` | **2008** | 917 B | `d2f9a7cc0b59495fa1b0664e2a6b5afd` | ECU / ASAP2 Calibration Map Definition |
| `53040010 2008 EDM Lancer Evolution X 5MT.xml` | **2008** | 23.6 KB | `f587af8079dc41e1ca4d2f98ce44a765` | ECU / ASAP2 Calibration Map Definition |
| `53050006 2008 EDM Lancer Evolution X SST.xml` | **2008** | 13.5 KB | `ec36ce1395d2a4ad107493e84f97029a` | ECU / ASAP2 Calibration Map Definition |
| `53050007 2008 EDM Lancer Evolution X SST.xml` | **2008** | 917 B | `b4c20b4cf9d07d728e0a0bf53e7711c4` | ECU / ASAP2 Calibration Map Definition |
| `53050009 2008 EDM Lancer Evolution X SST.xml` | **2008** | 28.5 KB | `c6eb94ea09a332bb953098a5fb02ceed` | ECU / ASAP2 Calibration Map Definition |
| `53050011 2008 EDM Lancer Evolution X SST.xml` | **2008** | 20.8 KB | `aab16de3134c3a12ae104974963a65cc` | ECU / ASAP2 Calibration Map Definition |
| `53050012 2008 EDM Lancer Evolution X SST.xml` | **2008** | 917 B | `c9c9f97754fbbc4336b6fc5ab0f85a9c` | ECU / ASAP2 Calibration Map Definition |
| `53600008 2009 USDM Lancer Ralliart SST.xml` | **2009** | 26.1 KB | `9a81bdf831e38bd7cd067ad72324c1b8` | ECU / ASAP2 Calibration Map Definition |
| `53600009 2009 USDM Lancer Ralliart SST.xml` | **2009** | 915 B | `6ee7937fb0ed45fd232f333c4a7b2d40` | ECU / ASAP2 Calibration Map Definition |
| `53600010 2009 USDM Lancer Ralliart SST.xml` | **2009** | 915 B | `c6077781f23b6825e867f04e9a93e317` | ECU / ASAP2 Calibration Map Definition |
| `53610009 2009 EDM Lancer Ralliart SST.xml` | **2009** | 23.9 KB | `8ecaa1308d16563f07187e67fc4e59a6` | ECU / ASAP2 Calibration Map Definition |
| `53610010 2009 EDM Lancer Ralliart SST.xml` | **2009** | 914 B | `255f1202ec1152dfdf4d9008412f6320` | ECU / ASAP2 Calibration Map Definition |
| `53610012 2009 EDM Lancer Ralliart SST.xml` | **2009** | 25.7 KB | `c66e05ce9b57a12b12e65ae97d89a7e5` | ECU / ASAP2 Calibration Map Definition |
| `53610013 2009 EDM Lancer Ralliart SST.xml` | **2009** | 914 B | `e1c23db71342dfb6e93887bcc2c45099` | ECU / ASAP2 Calibration Map Definition |
| `54060007 2009 EDM Lancer Evolution X 5MT.xml` | **2009** | 13.3 KB | `c2b6238a73ef76b06e6e615b661e9648` | ECU / ASAP2 Calibration Map Definition |
| `54060008 2009 EDM Lancer Evolution X 5MT.xml` | **2009** | 917 B | `96050335afadfbf6bdc9d5be7edb209a` | ECU / ASAP2 Calibration Map Definition |
| `54070006  2009 EDM Lancer Evolution X SST.xml` | **2009** | 20.2 KB | `9366abd054f1f508d1e745d45ce622d4` | ECU / ASAP2 Calibration Map Definition |
| `54070007 2009 EDM Lancer Evolution X SST.xml` | **2009** | 917 B | `06120ec853e54bb5a13c1c90156726ab` | ECU / ASAP2 Calibration Map Definition |
| `54550003 2009 JDM Lancer Evolution X SST.xml` | **2009** | 11.9 KB | `3e8cff8529b10359a91eac95415d82a1` | ECU / ASAP2 Calibration Map Definition |
| `54560003 2009 JDM Lancer Evolution X 5MT.xml` | **2009** | 12.1 KB | `f0be51c63993b449adea32988855a1d4` | ECU / ASAP2 Calibration Map Definition |
| `55570005 2010 USDM Lancer Evolution X 5MT.xml` | **2010** | 25.8 KB | `7ffe0c90733cf9806d63c7a76bd6a5b2` | ECU / ASAP2 Calibration Map Definition |
| `55570006 2010 USDM Lancer Evolution X 5MT.xml` | **2010** | 918 B | `de785b12642f8ddf4d4e6cc1efe6af19` | ECU / ASAP2 Calibration Map Definition |
| `55580005 2010 USDM Lancer Evolution X SST.xml` | **2010** | 34.2 KB | `81690cc37c4684dd60d4c1d9088a84e0` | ECU / ASAP2 Calibration Map Definition |
| `55580006 2010 USDM Lancer Evolution X SST.xml` | **2010** | 918 B | `7f51a7679f71033536888229e6dc163a` | ECU / ASAP2 Calibration Map Definition |
| `55590006 2010 USDM Lancer Ralliart SST.xml` | **2010** | 32.8 KB | `345b509fd861a5f7a73073fa11708bb4` | ECU / ASAP2 Calibration Map Definition |
| `55590007 2010 USDM Lancer Ralliart SST.xml` | **2010** | 915 B | `0cce19c9619bfe4ed30b3ec36c812948` | ECU / ASAP2 Calibration Map Definition |
| `56180001 2010 JDM Lancer Evolution X 5MT.xml` | **2010** | 20.1 KB | `f467820c14197702d37fe246ad21586c` | ECU / ASAP2 Calibration Map Definition |
| `56180002 2010 JDM Lancer Evolution X 5MT.xml` | **2010** | 917 B | `a186c7ee0e2f4eb8f5971841dbdf46e3` | ECU / ASAP2 Calibration Map Definition |
| `56190002 2010 JDM Lancer Evolution X SST.xml` | **2010** | 18.4 KB | `ba5f1da2844fe859c9c5bf5402dfde27` | ECU / ASAP2 Calibration Map Definition |
| `56870008 2011 JDM Lancer Evolution X 5MT.xml` | **2011** | 21.7 KB | `c49c7870c4d591c28be88d4da9a6a2c6` | ECU / ASAP2 Calibration Map Definition |
| `56880005 2011 JDM Lancer Evolution X SST.xml` | **2011** | 20.4 KB | `89b93d1101799441c72759a532b2a056` | ECU / ASAP2 Calibration Map Definition |
| `56880009 2011 JDM Lancer Evolution X SST.xml` | **2011** | 21.7 KB | `3bcddf86c6ad8947a405abfde7e17040` | ECU / ASAP2 Calibration Map Definition |
| `56890007 2011 USDM Lancer Evolution X 5MT.xml` | **2011** | 24.7 KB | `9286390363362d081d636635f87f6dcf` | ECU / ASAP2 Calibration Map Definition |
| `56890009 2011 USDM Lancer Evolution X 5MT.xml` | **2011** | 27.8 KB | `b1bfbbc65b1012abf25b8e9454e95d6c` | ECU / ASAP2 Calibration Map Definition |
| `56890010 2011 USDM Lancer Evolution X 5MT.xml` | **2011** | 918 B | `9f2bf7e0b12e8445774a6cae0c54b1df` | ECU / ASAP2 Calibration Map Definition |
| `56890013 2011 USDM Lancer Evolution X 5MT.xml` | **2011** | 22.4 KB | `a1c9de8d88f0b3e4d26349e6e936f943` | ECU / ASAP2 Calibration Map Definition |
| `56890109 2011 USDM Lancer Evolution X 5MT.xml` | **2011** | 733 B | `482e03bb3d769c345871421c929381bf` | ECU / ASAP2 Calibration Map Definition |
| `56900007 2011 USDM Lancer Evolution X SST.xml` | **2011** | 13.0 KB | `6e3eef9d2a6fd4f4e46c6b4887bc753c` | ECU / ASAP2 Calibration Map Definition |
| `56900009 2011 USDM Lancer Evolution X SST.xml` | **2011** | 27.1 KB | `939ff010f255629ac603d054386d12ec` | ECU / ASAP2 Calibration Map Definition |
| `56900010 2011 USDM Lancer Evolution X SST.xml` | **2011** | 918 B | `1b3fe60cc11f96b8960395b4838aa47f` | ECU / ASAP2 Calibration Map Definition |
| `56910007 2011 EDM Lancer Evolution X 5MT.xml` | **2011** | 24.6 KB | `8bffd2e32c83b8880025446774d2056f` | ECU / ASAP2 Calibration Map Definition |
| `56910009 2011 EDM Lancer Evolution X 5MT.xml` | **2011** | 20.7 KB | `bf012768519c78658aa5fcc004fc9a97` | ECU / ASAP2 Calibration Map Definition |
| `56920006 2011 EDM Lancer Evolution X SST.xml` | **2011** | 28.0 KB | `e02e9f52e375f829cbcb97e5b532d7c1` | ECU / ASAP2 Calibration Map Definition |
| `56920008 2011 EDM Lancer Evolution X SST.xml` | **2011** | 27.7 KB | `0c2f3b88bac50325307fd5d74198d601` | ECU / ASAP2 Calibration Map Definition |
| `56940007 2011 USDM Lancer Ralliart SST.xml` | **2011** | 21.9 KB | `f15c9b7e33eb813e35a9012f897f5ac5` | ECU / ASAP2 Calibration Map Definition |
| `56940009 2011 USDM Lancer Ralliart SST.xml` | **2011** | 10.1 KB | `d2cf50c879fd24ec7792b48bd011a896` | ECU / ASAP2 Calibration Map Definition |
| `56940010 2011 USDM Lancer Ralliart SST.xml` | **2011** | 915 B | `ec654bb60d55f6ac6f2648a86b3243bb` | ECU / ASAP2 Calibration Map Definition |
| `56950006 2011 EDM Lancer Ralliart SST.xml` | **2011** | 17.7 KB | `8269f0c12c1f5e82ab3630104fb4c689` | ECU / ASAP2 Calibration Map Definition |
| `57140001 2011 EDM Lancer Evolution X SST.xml` | **2011** | 33.6 KB | `fb99b896b0e1eecd6c2e7306ae0e5944` | ECU / ASAP2 Calibration Map Definition |
| `57140003 2011 EDM Lancer Evolution X SST.xml` | **2011** | 27.1 KB | `9f652361999d3b5b310797ed167393f0` | ECU / ASAP2 Calibration Map Definition |
| `58010005 2012 USDM Lancer Evolution X 5MT.xml` | **2012** | 22.9 KB | `2b585464ecc427bf0c8dcd9a15c7e2e6` | ECU / ASAP2 Calibration Map Definition |
| `58020005 2012 USDM Lancer Evolution X SST.xml` | **2012** | 28.2 KB | `d0e3e0547f8cd32702ec2e1070fcc66e` | ECU / ASAP2 Calibration Map Definition |
| `58030005 2012 USDM Lancer Ralliart SST.xml` | **2012** | 24.6 KB | `ba78ec48d029cabfb4faef82bce86eff` | ECU / ASAP2 Calibration Map Definition |
| `58030006 2012 USDM Lancer Ralliart SST.xml` | **2012** | 655 B | `8360b7ab23f5b19dea6e42ea48efb57b` | ECU / ASAP2 Calibration Map Definition |
| `58045804 2014 EDM Lancer Evolution X 5MT.xml` | **2014** | 10.6 KB | `8580ffa076b70b23c2c7b04d724a0bb2` | ECU / ASAP2 Calibration Map Definition |
| `58640002 2012 EDM Lancer Ralliart SST.xml` | **2012** | 24.6 KB | `da54272678b6d79c93e8dcfd49693e0c` | ECU / ASAP2 Calibration Map Definition |
| `59570004 2013 USDM Lancer Ralliart SST.xml` | **2013** | 28.6 KB | `eb2bcd839b4872b5bf5e6422a461bd94` | ECU / ASAP2 Calibration Map Definition |
| `59580004 2013 USDM Lancer Evolution X 5MT.xml` | **2013** | 28.7 KB | `a28b6174a90c6837841b7ce9010c7092` | ECU / ASAP2 Calibration Map Definition |
| `59580005 2013 USDM Lancer Evolution X 5MT.xml` | **2013** | 923 B | `a387f0d2755853466dcf0fb88b751456` | ECU / ASAP2 Calibration Map Definition |
| `59590004 2013 USDM Lancer Evolution X SST.xml` | **2013** | 30.1 KB | `90cd28cd764118671d7f226398cc6a7a` | ECU / ASAP2 Calibration Map Definition |
| `59590005 2013 USDM Lancer Evolution X SST.xml` | **2013** | 923 B | `034e04ad5194c9b32fc13c6e8ff1a88a` | ECU / ASAP2 Calibration Map Definition |
| `80700010 2002 JDM Lancer Evo 7 AT.xml` | **2002** | 23.7 KB | `1c9024fc158c2442abe49a1250cb80ba` | ECU / ASAP2 Calibration Map Definition |
| `80920002 2005 JDM Lancer Evolution MT.xml` | **2005** | 12.8 KB | `7e91f77198d041a14d4ed052a28151e5` | ECU / ASAP2 Calibration Map Definition |
| `88570008 2005 JDM Lancer Evolution MT.xml` | **2005** | 21.3 KB | `ed7d88a86808b756ba4a4efa9498aff3` | ECU / ASAP2 Calibration Map Definition |
| `88580013 2006 ADM Lancer Evolution MT.xml` | **2006** | 13.5 KB | `85ad552cbb247033cab11825c3422234` | ECU / ASAP2 Calibration Map Definition |
| `88580014 2007 ADM Lancer Evolution MT.xml` | **2007** | 747 B | `612892fd75963244b372ba53c4b07b3c` | ECU / ASAP2 Calibration Map Definition |
| `88580015 2006 JDM Lancer Evolution MT.xml` | **2006** | 12.6 KB | `4bb15c6fbf616951b4a689f6adbf1559` | ECU / ASAP2 Calibration Map Definition |
| `88590013 2006 USDM Lancer Evolution MT.xml` | **2006** | 11.1 KB | `2dd9f5e0b7567e2ef199296ce1b9c06f` | ECU / ASAP2 Calibration Map Definition |
| `88590014 2006 USDM Lancer Evolution MT.xml` | **2006** | 676 B | `48cd0aeb722f4fa7d6430204f00b6da0` | ECU / ASAP2 Calibration Map Definition |
| `88590015 2006 USDM Lancer Evolution MT.xml` | **2006** | 17.6 KB | `7968a40036c8757645aef3113cf517af` | ECU / ASAP2 Calibration Map Definition |
| `88590016 2006 USDM Lancer Evolution MT.xml` | **2006** | 742 B | `dd77927db6114201d91d7aa20cfcf795` | ECU / ASAP2 Calibration Map Definition |
| `88780004 2008 JDM Lancer Evolution AT.xml` | **2008** | 26.2 KB | `fd28577228ab613e0ee957aef7b0cd15` | ECU / ASAP2 Calibration Map Definition |
| `88840013 2006 EDM Lancer Evolution MT.xml` | **2006** | 8.9 KB | `a593e71fb0c2569c8b15cb81b3f95163` | ECU / ASAP2 Calibration Map Definition |
| `88840016 2006 EDM Lancer Evolution MT.xml` | **2006** | 11.2 KB | `f4b6d3caf39909b07b5c2a20caeaa780` | ECU / ASAP2 Calibration Map Definition |
| `88840017 2006 EDM Lancer Evolution MT.xml` | **2006** | 11.3 KB | `bbaa5bf9123a91a6d5051245ace7e7f9` | ECU / ASAP2 Calibration Map Definition |
| `89280002 2006 JDM Lancer Evolution MT.xml` | **2006** | 13.2 KB | `e6f7aa34f015f6be7a78b207cfb2aca3` | ECU / ASAP2 Calibration Map Definition |
| `89960000 2005 JDM Lancer Evolution MT.xml` | **2005** | 17.3 KB | `fa9f7c736a22291d498941f9c2318bc5` | ECU / ASAP2 Calibration Map Definition |
| `89980000 2006 JDM Lancer Evolution MT.xml` | **2006** | 13.2 KB | `534abe1d066e6e9dcf8bcb06e17dd754` | ECU / ASAP2 Calibration Map Definition |
| `90550001 2001 EDM Lancer Evo 7 5MT.xml` | **2001** | 8.2 KB | `96d6dbfc78e11363982a4bde3c195664` | ECU / ASAP2 Calibration Map Definition |
| `90551001 2001 EDM Lancer Evo 7 5MT.xml` | **2001** | 917 B | `c6d5767f8cf8cde0970dd2345c3db59a` | ECU / ASAP2 Calibration Map Definition |
| `92460000 2001 JDM Lancer Evo 7 Ralliart 6MT.xml` | **2001** | 10.1 KB | `58aa630bbdb32108f14ce6a6b3f65470` | ECU / ASAP2 Calibration Map Definition |
| `93390000 2001 JDM Evo 7 MT.xml` | **2001** | 15.8 KB | `10a1fbcdc9f13412b21c9e99474898cc` | ECU / ASAP2 Calibration Map Definition |
| `93660005 2004 JDM Lancer Evo 8 FQ300 MT.xml` | **2004** | 8.8 KB | `9db622e5868424cbbcc777f6228b6a95` | ECU / ASAP2 Calibration Map Definition |
| `93670005 2004 JDM Lancer Evo 8 MR RS MT.xml` | **2004** | 13.2 KB | `e988e154cd61e1404d2137948c484ccb` | ECU / ASAP2 Calibration Map Definition |
| `94170008 2004 USDM Lancer Evo 8 MT.xml` | **2004** | 8.6 KB | `dd11b571c7926c627319b6fb37057ff7` | ECU / ASAP2 Calibration Map Definition |
| `94170014 2004 USDM Lancer Evo 8 MT.xml` | **2004** | 9.3 KB | `d770b9ce48fd82895bda096ebe61bd82` | ECU / ASAP2 Calibration Map Definition |
| `94170015 2004 USDM Lancer Evo 8 MT.xml` | **2004** | 9.3 KB | `6a7073d1b8dc6bd021d84b9ac3f15f9b` | ECU / ASAP2 Calibration Map Definition |
| `96260007 2004 JDM Lancer Evo 8 MT.xml` | **2004** | 14.6 KB | `64b721e9e109897613ce549488c8bcbd` | ECU / ASAP2 Calibration Map Definition |
| `96260009 2004 JDM Lancer Evo 8 MT.xml` | **2004** | 37.5 KB | `3df599d56b2514620e5ff744f981ceaf` | ECU / ASAP2 Calibration Map Definition |
| `96420007 2004 USDM Lancer Evo 8 MT.xml` | **2004** | 8.6 KB | `5f9ab1db6820c1ecf6961e59ec399ce9` | ECU / ASAP2 Calibration Map Definition |
| `96420008 2004 USDM Lancer Evo 8 MT.xml` | **2004** | 8.5 KB | `5c25b2e83778d7cc6a755e0d8c0ebf43` | ECU / ASAP2 Calibration Map Definition |
| `96420011 2004 USDM Lancer Evo 8 MT.xml` | **2004** | 8.5 KB | `130f87d2eff2fc0bce34df6a4d7c66ee` | ECU / ASAP2 Calibration Map Definition |
| `96530006 2005 ADM Lancer Evo 8 MT.xml` | **2005** | 29.3 KB | `3612f306a6ab980ad054b3e27d46875f` | ECU / ASAP2 Calibration Map Definition |
| `96940011 2005 USDM Lancer Evo 8 MT.xml` | **2005** | 12.7 KB | `a3d7d588da9b59f8046f4f5735ed71a5` | ECU / ASAP2 Calibration Map Definition |
| `97250001 2004 JDM Lancer Evo 8 GSR MT.xml` | **2004** | 11.5 KB | `77e09ef3e7da1c9bdf894832977ba45d` | ECU / ASAP2 Calibration Map Definition |
| `97470001 2005 JDM Lancer Evo 8 MT.xml` | **2005** | 666 B | `b932c520ca49e578451ccca484721988` | ECU / ASAP2 Calibration Map Definition |
| `98640014 2002 JDM Lancer Evo 7 MT.xml` | **2002** | 21.7 KB | `c8f064f602db956d7452a668702b78cd` | ECU / ASAP2 Calibration Map Definition |
| `98640016 2002 JDM Lancer Evo 7 MT.xml` | **2002** | 15.2 KB | `1502b9712904887868fcb491a7ee454e` | ECU / ASAP2 Calibration Map Definition |
| `98650012 2001 EDM Lancer Evo 7 5MT.xml` | **2001** | 15.7 KB | `6de97a8bf00560d0c03b3aef7a4aa6b4` | ECU / ASAP2 Calibration Map Definition |
| `98650014 2001 JDM Lancer Evo 7 MT.xml` | **2001** | 618 B | `08e650867348370ba87b5a25817dd067` | ECU / ASAP2 Calibration Map Definition |
| `98650015 2001 EDM Lancer Evo 7 5MT.xml` | **2001** | 21.0 KB | `d0a529bf7f28a5af4875d8ee02d435d4` | ECU / ASAP2 Calibration Map Definition |
| `98650017 2001 EDM Lancer Evo 7 5MT.xml` | **2001** | 26.4 KB | `eacb0f1fd4ed37a35f53ccb7074a524c` | ECU / ASAP2 Calibration Map Definition |
| `99270000 2004 EDM Lancer Evo 8 MT.xml` | **2004** | 11.9 KB | `12faafc9df48f3822d5a20dbd7aad785` | ECU / ASAP2 Calibration Map Definition |
| `99860002 2001 JDM Lancer Evo 7 MT.xml` | **2001** | 9.9 KB | `4b56fb6bb2892bfa7f25e25d9945ce08` | ECU / ASAP2 Calibration Map Definition |
| `DM401702 2004 USDM Lancer Evo 8 ACD.xml` | **2004** | 544 B | `323b2b1c7bba24a7b32475394c7a4ebd` | ECU / ASAP2 Calibration Map Definition |
| `SM5237.xml` | **2001–2007** | 3.8 KB | `141250bf9bd32112769819927a4dd71d` | ECU / ASAP2 Calibration Map Definition |
| `evo10base.xml` | **2001–2007** | 95.1 KB | `c1826997f87e4bd1f9b7b68e9e2b9605` | ECU / ASAP2 Calibration Map Definition |
| `evo5base.xml` | **2001–2007** | 24.9 KB | `0b7be2e7cd386475a99d5f76dc9816ae` | ECU / ASAP2 Calibration Map Definition |
| `evo7base.xml` | **2001–2007** | 51.9 KB | `866382b8b4d8d2d38ed5232379de545a` | ECU / ASAP2 Calibration Map Definition |
| `evo9base.xml` | **2001–2007** | 55.1 KB | `a0fc7288706c83d06786d136929d5484` | ECU / ASAP2 Calibration Map Definition |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro yang tersedia, struktur kalibrasi mencakup parameter esensial:
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
