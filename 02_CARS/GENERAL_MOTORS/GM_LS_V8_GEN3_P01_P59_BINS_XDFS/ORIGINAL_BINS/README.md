# ORIGINAL BINS - ECU Calibration Suite

**Repository Path**: `02_CARS/GENERAL_MOTORS/GM_LS_V8_GEN3_P01_P59_BINS_XDFS/ORIGINAL_BINS`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `88 files` (88 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `ORIGINAL_BINS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 1989–2006

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `'01 C1500 LM7 os12208322.bin` | **2001** | 512.0 KB | `dc8741067b31fce1a74a88456164a14c` | Factory Binary Firmware Dump |
| `'01 GMC c1500 LM7 os 12208322.bin` | **2001** | 512.0 KB | `ba98023374ab41ed3aa9652a3cd96129` | Factory Binary Firmware Dump |
| `'01 K1500 4.8 LR4 os12208322.bin` | **2001** | 512.0 KB | `fca2b93c60909bd1f233f86927607d05` | Factory Binary Firmware Dump |
| `'01 K2500 8.1L18 0s12208322.bin` | **2001** | 512.0 KB | `309656e529aec44ce9d949873d0538a1` | Factory Binary Firmware Dump |
| `'01 LM7 os12208322.bin` | **2001** | 512.0 KB | `dc8741067b31fce1a74a88456164a14c` | Factory Binary Firmware Dump |
| `'01C1500 LM7 os12208322.bin` | **1999–2002 (P01)** | 512.0 KB | `b442ef77351cfcdfac594125f3c36141` | Factory Binary Firmware Dump |
| `'01K2500 6.0L os12208322.bin` | **1999–2002 (P01)** | 512.0 KB | `e02c04385d5323db5c8a0d913f204886` | Factory Binary Firmware Dump |
| `'02 Chevy 2500 4x4 8.1 L18 os12216125 (1).bin` | **2002** | 512.0 KB | `f41649ab0448db95db40f7661fcb21fc` | Factory Binary Firmware Dump |
| `'02 Chevy 2500 4x4 8.1 L18 os12216125.bin` | **2002** | 512.0 KB | `f41649ab0448db95db40f7661fcb21fc` | Factory Binary Firmware Dump |
| `'02 Chevy K1500 5.3L os12216125 (1).bin` | **2002** | 512.0 KB | `57b8a2bbed76b86b16295c48b0f2a8a7` | Factory Binary Firmware Dump |
| `'03 Chevy 1500 4x4 LM7 os12579405.bin` | **2003** | 1.00 MB | `eb3a08402aab9a3a966b727cf2a143d0` | Factory Binary Firmware Dump |
| `'03 Chevy 4x2  6.0L os12579405.bin` | **2003** | 1.00 MB | `60e49dc54dbaa4a98b32f7cb86d6c8ce` | Factory Binary Firmware Dump |
| `'03 Chevy Half 4x2 6.0 LQ4 os12579405.bin` | **2003** | 1.00 MB | `f379160f2dccfbc69aace87b365cb3f5` | Factory Binary Firmware Dump |
| `'03 Chevy Half T 4x4 6.0L os12593058.bin` | **2003** | 1.00 MB | `cc49cb8a9060a7cb8d3aafc6cb43d167` | Factory Binary Firmware Dump |
| `'03 Chevy MPV Half T 4x2 4.8 LR4 os12579405.bin` | **2003** | 1.00 MB | `493de6a6380a12b2b27ce4e3a8ceded0` | Factory Binary Firmware Dump |
| `'03 K1500 6.0L os12579405.bin` | **2003** | 1.00 MB | `a100ec03bc95a254fea9faac408d6db0` | Factory Binary Firmware Dump |
| `'03 K1500 6.0L os12593058.bin` | **2003** | 1.00 MB | `a0b2eaf5978f8757a35cd1dcd4c88f07` | Factory Binary Firmware Dump |
| `'04 CTS-V LS6 M6 os12592433.bin` | **2004** | 1.00 MB | `3b97f077d0582241d8709c191dae124b` | Factory Binary Firmware Dump |
| `'04 Chevy MPV  4x4 Half Ton LM7 os12587603.bin` | **2004** | 1.00 MB | `07cfa958303ce233016c29c5d9983dcb` | Factory Binary Firmware Dump |
| `'04 GMC 1T 4x4 8.1 L18 os12587603.bin` | **2004** | 1.00 MB | `52d7d7c7d6de397b5e7d86f83d4658d0` | Factory Binary Firmware Dump |
| `'04K1500 6.0L os12585950.bin` | **2012–2018** | 1.00 MB | `b2f9032d77bf127a616172ca98d68540` | Factory Binary Firmware Dump |
| `'05 Cadillac CTS-V LS6 M6 os12592618.bin` | **2005** | 1.00 MB | `bb2ec0b9107986fdfa12a5a86671a497` | Factory Binary Firmware Dump |
| `'05 Chevy 1500 4x4 os 12592618.bin` | **2005** | 1.00 MB | `587227f6f9cf7915c71bd6b382421f12` | Factory Binary Firmware Dump |
| `'05 Chevy MPV  Half ton4x4 LM7 os 12592618.bin` | **2005** | 1.00 MB | `51d94e2af75900194e7a13e9db096545` | Factory Binary Firmware Dump |
| `'05 Chevy MPV 4x2 1500 4.8L 12592618.bin` | **2005** | 1.00 MB | `a737cc6ccc8f25b6dcf42876b2c20d85` | Factory Binary Firmware Dump |
| `'05 GMC MPV 4x2 2500 6.0 LQ4 os12592618.bin` | **2005** | 1.00 MB | `c20b175cddafefada1df916f8b11a3ad` | Factory Binary Firmware Dump |
| `'05Chevy 1500 4x44.8 LR4  12592618.bin` | **2003–2007 (P59)** | 1.00 MB | `b80f4e948e75039f3cb1616cb18cb064` | Factory Binary Firmware Dump |
| `01 LM7 12202088 (1).bin` | **2001** | 512.0 KB | `18ad0009d5aecbd08507ada55a71507e` | Factory Binary Firmware Dump |
| `01 LM7 12202088.bin` | **2001** | 512.0 KB | `18ad0009d5aecbd08507ada55a71507e` | Factory Binary Firmware Dump |
| `01 chevy MPV 4x4 Half T LM7 os12208322.bin` | **2001** | 512.0 KB | `4dab85f1aa344500eca42a4260abb648` | Factory Binary Firmware Dump |
| `03 Chevy 1500 4x2 6.0 LQ4 12579405.bin` | **2003** | 1.00 MB | `57e4fd16cde97f980c125f8fde7033b8` | Factory Binary Firmware Dump |
| `03 Chevy 2500 4x2 6.0 LQ4 os12579405.bin` | **2003** | 1.00 MB | `3a99b53916bb6ab40bac6ae4abb5b830` | Factory Binary Firmware Dump |
| `03_Sierra_LM7_4L60E_DBW_OS12587603.bin` | **2003** | 1.00 MB | `412a4d7cfb38fe24fc00f5a09dd40d83` | Factory Binary Firmware Dump |
| `04 Chevy half Ton 4x4 6.0L 12585950.bin` | **2004** | 1.00 MB | `bd5f2b1e6cac09f47f0ead78a040a678` | Factory Binary Firmware Dump |
| `04 Silverado SS 11.8.13 Stock OS12585950.bin` | **2004** | 1.00 MB | `32f23ba73e088816499330fc64b478bb` | Factory Binary Firmware Dump |
| `05 Chevy 1500 4X4 6.0L  12592618.bin` | **2005** | 1.00 MB | `b6d30733003fb08fa98a4ac583e7dba5` | Factory Binary Firmware Dump |
| `05 Chevy 1500 4x2 LM7 12592618.bin` | **2005** | 1.00 MB | `e76d7399c2c0f140a9c33944d12ce466` | Factory Binary Firmware Dump |
| `05 Chevy 1500 4x4 MPV L59 12592618.bin` | **2005** | 1.00 MB | `4cf3091a5f21632f73e58ee27a35a967` | Factory Binary Firmware Dump |
| `05 Chevy 1Ton 6.0LQ4 12589463.bin` | **2005** | 1.00 MB | `36024da0f4fad092d6a6426a0efddebc` | Factory Binary Firmware Dump |
| `05 Escalade 4x4 6.0L os12592618.bin` | **2005** | 512.0 KB | `feac6ab58fec81468a07a0e8c2646d5a` | Factory Binary Firmware Dump |
| `05 Escalade 6.0L 4x4 os12592618 (1).bin` | **2005** | 1.00 MB | `8144611480d1bf2ce5f799e99d804336` | Factory Binary Firmware Dump |
| `05 Escalade 6.0L 4x4 os12592618.bin` | **2005** | 1.00 MB | `8144611480d1bf2ce5f799e99d804336` | Factory Binary Firmware Dump |
| `05 Hummer H2 6.0 LQ4 os12592618.bin` | **2005** | 1.00 MB | `bc3f3868f9a2574663931301ac0a2932` | Factory Binary Firmware Dump |
| `2001 5.3 Auto OS12208322.bin` | **2001** | 512.0 KB | `1bbe1d698bb2e4d7476113493dadb26f` | Factory Binary Firmware Dump |
| `2001 8.1 12208322.bin` | **2001** | 512.0 KB | `54244ec3cff1831ac914e488e827befc` | Factory Binary Firmware Dump |
| `2001 Chevrolet Silverado Truck Automatic LQ4 6.0 Litre (12208322).bin` | **2001** | 512.0 KB | `dcb1714dd8a0ccc82f40f07a5108dc8f` | Factory Binary Firmware Dump |
| `2001 Chevy 1500 4x2 4.8 LR4 12208322.bin` | **2001** | 512.0 KB | `1f321826a57415ab8e6d97a8fc6b29e6` | Factory Binary Firmware Dump |
| `2001 Chevy S-10 L35 4.3L 4L60E (12202088).bin` | **2001** | 512.0 KB | `b15c78939740180888c087ebdfe21163` | Factory Binary Firmware Dump |
| `2001 Chevy Tahoe LM7 5.3L Auto (12202088).bin` | **2001** | 512.0 KB | `4ceb219cacd6b2a5f5f361510fac86f1` | Factory Binary Firmware Dump |
| `20014.84x4 12208322.bin` | **1999–2002 (P01)** | 512.0 KB | `fca2b93c60909bd1f233f86927607d05` | Factory Binary Firmware Dump |
| `2001_6.0_2500_2wd _Cal_OS12202088.bin` | **2001** | 512.0 KB | `27bcf28b45720ba064694ebc7cc6b577` | Factory Binary Firmware Dump |
| `2001_6.0_OS12208322.bin` | **2001** | 512.0 KB | `dcb1714dd8a0ccc82f40f07a5108dc8f` | Factory Binary Firmware Dump |
| `2002 1500 5.3 12216125.bin` | **2002** | 512.0 KB | `3546d82cd8c5216cde4307c3c88d2d50` | Factory Binary Firmware Dump |
| `2002 4.8L LR4 4x2 1-2T MANUAL TRANS os12212156.bin` | **2002** | 512.0 KB | `177a2bfd1a26006e2378618dc6a9374a` | Factory Binary Firmware Dump |
| `2002 5.3L 2wd Stock DBC No EGR 12212156.bin` | **2002** | 512.0 KB | `6694c5961f93de2f8f0130647603e7ec` | Factory Binary Firmware Dump |
| `2002 5.3L Flex 2wd with Traction Stock 12216125.bin` | **2002** | 512.0 KB | `42e83a12d3f370a1ad1ee934363de924` | Factory Binary Firmware Dump |
| `2002 Chevrolet Express Van Automatic L31 5.7L 4L60e 2wd (12212156) Lean Cruise (1).bin` | **2002** | 512.0 KB | `7d07f3cdc53881af805336b9e1d2ccd0` | Factory Binary Firmware Dump |
| `2002 Chevrolet Express Van Automatic L31 5.7L 4L60e 2wd (12212156) Lean Cruise.bin` | **2002** | 512.0 KB | `7d07f3cdc53881af805336b9e1d2ccd0` | Factory Binary Firmware Dump |
| `2002 Chevrolet Express Van L31 5.7 Litre 4L80E(12212156).bin` | **2002** | 512.0 KB | `cfefc4bf9306f47a51cdb10533b77907` | Factory Binary Firmware Dump |
| `2002 Chevrolet Silverado Truck Auto LM7 5.3L (12212156) (1).bin` | **2002** | 512.0 KB | `05377159d32794dac3dda81f9e30cbb8` | Factory Binary Firmware Dump |
| `2002 Chevrolet Silverado Truck Auto LM7 5.3L (12212156).bin` | **2002** | 512.0 KB | `05377159d32794dac3dda81f9e30cbb8` | Factory Binary Firmware Dump |
| `2002 Chevrolet Silverado Truck Manual LM7 5.3 Litre (12212156) (1).bin` | **2002** | 512.0 KB | `bc4516bb3aaa4c2ea4975b46d3696126` | Factory Binary Firmware Dump |
| `2002 Chevrolet Silverado Truck Manual LM7 5.3 Litre (12212156).bin` | **2002** | 512.0 KB | `bc4516bb3aaa4c2ea4975b46d3696126` | Factory Binary Firmware Dump |
| `2002 Chevy S-10 L35 4.3L 4L60E (12212156).bin` | **2002** | 512.0 KB | `0c64d7ceddad860c30b88d2922c24ec6` | Factory Binary Firmware Dump |
| `2002 Chevy S-10 L35 4.3L 4L60E (12212156)Lean Cruise.bin` | **2002** | 512.0 KB | `8d787123561de59bf70cd29a456c41bc` | Factory Binary Firmware Dump |
| `2003 Express Van 6.0 DBC 4L80E OS 12579405.bin` | **2003** | 1.00 MB | `8620ae325bc9afe5db9a5e6b410d336c` | Factory Binary Firmware Dump |
| `2003SuburbanDBW5.3FlexFuel_OS12579405.bin` | **2003** | 1.00 MB | `5bbd0f37deb8a58753c0e7256e46f298` | Factory Binary Firmware Dump |
| `2003_jimmy_5.3_auto_4x4_Stock_OS12593058.bin` | **2003** | 1.00 MB | `28bcbc5e9d45ee66b552885c778f078b` | Factory Binary Firmware Dump |
| `2004 2500 LQ4 Auto 2wd stock OS12587603.bin` | **2004** | 1.00 MB | `59698a2f43fc1bd1c080ef9e65bbc7bc` | Factory Binary Firmware Dump |
| `2004 Corvette M6 Stock.bin` | **2004** | 1.00 MB | `aef67389fbf7981bb6313727282acfe7` | Factory Binary Firmware Dump |
| `2004 Escalade 5.3AutoStock OS12587603.bin` | **2004** | 1.00 MB | `a01110a0bd863433c5129748d54b613f` | Factory Binary Firmware Dump |
| `2005_5.3_Auto_4X4_OS12592618.bin` | **2005** | 1.00 MB | `a5b92c7e2b9fc41e27f115e443c9fc39` | Factory Binary Firmware Dump |
| `2006 Express 2500 4.8L DBC 4L80E 12606807.bin` | **2006** | 1.00 MB | `c43bb7cbf423dad7b0e0f3d1f778275a` | Factory Binary Firmware Dump |
| `2006 Silverado C2500HD 6.0L 4L80E 12587811.bin` | **2006** | 1.00 MB | `0945ed1242e1fdec8eeef8ce835ed660` | Factory Binary Firmware Dump |
| `2006 Silverado C2500HD 6.0L 4L80E 12613246.bin` | **2006** | 1.00 MB | `aa5cfc33fb8d71dfa3165630c1ee42cc` | Factory Binary Firmware Dump |
| `2006 Silverado K1500 5.3L 4L60E 12587811.bin` | **2006** | 1.00 MB | `73c4ec3f76c0023d692e11ae0031b6eb` | Factory Binary Firmware Dump |
| `2006 Silverado K1500 5.3L 4L60E 12613246.bin` | **2006** | 1.00 MB | `b0358bc963ae3cb9292382f90fc6c450` | Factory Binary Firmware Dump |
| `2006 Silverado K2500HD 6.0L 4L80E 12606807.bin` | **2006** | 1.00 MB | `56c29920b2a62760c001cf55cef52e66` | Factory Binary Firmware Dump |
| `2006 Silverado K2500HD 6.0L 4L80E 12613246.bin` | **2006** | 1.00 MB | `c81be2cdfc45f5059f1ce7653639aec0` | Factory Binary Firmware Dump |
| `2006 Yukon XL Denali 6.0L AWD 4L60E 12587811.bin` | **2006** | 1.00 MB | `9ab240d49c2891af8541fcc93f401b40` | Factory Binary Firmware Dump |
| `2006_Silverado_5.3_Auto_OS12619623.bin` | **2006** | 1.00 MB | `6c786b7b1e49c7c099a46cd50b989bad` | Factory Binary Firmware Dump |
| `2006_Tahoe_5.3_Auto_4x4_OS12619623.bin` | **2006** | 1.00 MB | `11d8f2ca4328755ed43e71db45dc62f2` | Factory Binary Firmware Dump |
| `2006_stock_4.8_4x4 os 12606807.bin` | **2006** | 1.00 MB | `ab36c87055c1234042feb98260291444` | Factory Binary Firmware Dump |
| `C1500_5.3L_OS12587603.bin` | **2003–2007 (P59)** | 1.00 MB | `d093d51c6966f57825d77d158f8b9e4c` | Factory Binary Firmware Dump |
| `Chevy_1500_4x2_LM7 _OS12587603.bin` | **2003–2007 (P59)** | 1.00 MB | `a88e7062f3019e59b12314f56ed985d0` | Factory Binary Firmware Dump |
| `Chevy_1500_4x4_MPV_L59_12587603.bin` | **2003–2007 (P59)** | 1.00 MB | `1428a0038c2a3385befca2350796017c` | Factory Binary Firmware Dump |
| `Chevy_2500_4x4_LQ4_OS12585950.bin` | **1989–2006** | 1.00 MB | `ff7b6b81c46541433ea4228f4c1739d4` | Factory Binary Firmware Dump |
| `Chevy_4x4_Half_T_6.0L_OS12585950.bin` | **1989–2006** | 1.00 MB | `355bfee4826c90b567ef76bfb473212b` | Factory Binary Firmware Dump |

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
