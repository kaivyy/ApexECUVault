# LANDCRUISER_PRADO_LC200_LC150_LC120 - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/LANDCRUISER_PRADO_LC200_LC150_LC120`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `62 files` (62 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `LANDCRUISER_PRADO_LC200_LC150_LC120` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2003–2021

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `89663-60551.bin` | **2003–2021** | 736.0 KB | `3f49683123aaf9dcabdaa8e5f2a03ae7` | Factory Binary Firmware Dump |
| `89663-60561.bin` | **2003–2021** | 736.0 KB | `8f723e88b4c47639b456e2b83e51032b` | Factory Binary Firmware Dump |
| `89663-60590.bin` | **2003–2021** | 496.0 KB | `df46f5ec5cfb1bd26422c62912ac4f3e` | Factory Binary Firmware Dump |
| `89663-60640.bin` | **2003–2021** | 992.0 KB | `8308af00559434344cc5bf736a7e1f03` | Factory Binary Firmware Dump |
| `89663-60641.bin` | **2003–2021** | 992.0 KB | `d1414f7e2c3db09b3f11e1d4ac3e071f` | Factory Binary Firmware Dump |
| `89663-60642.bin` | **2003–2021** | 992.0 KB | `0f7d568155829987c4e74b9743076ddc` | Factory Binary Firmware Dump |
| `89663-60643.bin` | **2003–2021** | 992.0 KB | `05f283489ca8bc6343c1617cbf79d7b8` | Factory Binary Firmware Dump |
| `89663-60883.bin` | **2003–2021** | 496.0 KB | `813f87c0f705446146637a921b356a8f` | Factory Binary Firmware Dump |
| `89663-60884.bin` | **2003–2021** | 496.0 KB | `1b561547ab6c3e538af11c7367c9e565` | Factory Binary Firmware Dump |
| `89663-60A31.bin` | **2003–2021** | 992.0 KB | `55357b624a144b08e53a4cfbc4832f02` | Factory Binary Firmware Dump |
| `89663-60A32.bin` | **2003–2021** | 992.0 KB | `58561bebdc952395feb49596aff96680` | Factory Binary Firmware Dump |
| `89663-60A33.bin` | **2003–2021** | 992.0 KB | `1ddf5a38af6045ef4418070818f93b7b` | Factory Binary Firmware Dump |
| `89663-60A34.bin` | **2003–2021** | 992.0 KB | `625b5b2605673fee479e7d7f6ed09545` | Factory Binary Firmware Dump |
| `89663-60A60.bin` | **2003–2021** | 992.0 KB | `a0a5417ad828bb7b0c953918cb06786f` | Factory Binary Firmware Dump |
| `89663-60A61.bin` | **2003–2021** | 992.0 KB | `285592255a9a97aa9060fc42534cc9a3` | Factory Binary Firmware Dump |
| `89663-60A63.bin` | **2003–2021** | 992.0 KB | `2312a35f5c14082c998730c7e94b1759` | Factory Binary Firmware Dump |
| `89663-60A70.bin` | **2003–2021** | 992.0 KB | `c00279abec0624e019be1ee866f725ec` | Factory Binary Firmware Dump |
| `89663-60A71.bin` | **2003–2021** | 992.0 KB | `b09e362f5d1ac7dd13aaa3152e82ac31` | Factory Binary Firmware Dump |
| `89663-60A72.bin` | **2003–2021** | 992.0 KB | `a21cd9e754f376ed234d88d1b16cc3e0` | Factory Binary Firmware Dump |
| `89663-60A73.bin` | **2003–2021** | 992.0 KB | `a7f1f183e63502bfac859af2d3cdaabf` | Factory Binary Firmware Dump |
| `89663-60A80.bin` | **2003–2021** | 992.0 KB | `8a393de043f599e2208152f2798c9bed` | Factory Binary Firmware Dump |
| `89663-60A82.bin` | **2003–2021** | 992.0 KB | `c31106417e512b7d5caeec6a0cacf47a` | Factory Binary Firmware Dump |
| `89663-60A83.bin` | **2003–2021** | 992.0 KB | `da57b196a1392b4f4e80733a07c680b1` | Factory Binary Firmware Dump |
| `89663-60B02.bin` | **2003–2021** | 992.0 KB | `899c2e68a542de7f7e9d0a50b3c3cb58` | Factory Binary Firmware Dump |
| `89663-60B03.bin` | **2003–2021** | 992.0 KB | `8b0c0c01fc89f5adb1604ed46f50f208` | Factory Binary Firmware Dump |
| `89663-60B30.bin` | **2003–2021** | 992.0 KB | `8798a9633d355e17c77e00648c867196` | Factory Binary Firmware Dump |
| `89663-60C01.bin` | **2003–2021** | 736.0 KB | `af02ec275027827c11e799b4fdb053b3` | Factory Binary Firmware Dump |
| `89663-60C02.bin` | **2003–2021** | 736.0 KB | `7edc7da25a3f78f6c16cf1a537b28127` | Factory Binary Firmware Dump |
| `89663-60C51.bin` | **2003–2021** | 992.0 KB | `45a643d138331cf2236ac8102c6b05a3` | Factory Binary Firmware Dump |
| `89663-60D82.bin` | **2003–2021** | 992.0 KB | `3a5a2a3b913a4567072bf4f519eb982b` | Factory Binary Firmware Dump |
| `89663-60E64.bin` | **2003–2021** | 992.0 KB | `9b47aa92031ba832eb652c8b2353987b` | Factory Binary Firmware Dump |
| `89663-60G90.bin` | **2003–2021** | 992.0 KB | `70610c7ec36fe0706717eb53fcc83a32` | Factory Binary Firmware Dump |
| `89663-60J01.bin` | **2003–2021** | 992.0 KB | `f3370135aa9e3e1efc17f3c2af3551e9` | Factory Binary Firmware Dump |
| `89663-60J10.bin` | **2003–2021** | 992.0 KB | `cf22b49d25065b7168cb553f9d52f4eb` | Factory Binary Firmware Dump |
| `89663-60J20.bin` | **2003–2021** | 992.0 KB | `ccc6801112ac8f70900bec3d9ed187ba` | Factory Binary Firmware Dump |
| `89663-60J21.bin` | **2003–2021** | 992.0 KB | `727c5dccb060e2ff800dc45f38d959e5` | Factory Binary Firmware Dump |
| `89663-60J30.bin` | **2003–2021** | 992.0 KB | `0e775d09a0c2c749ab06783bea7e0c75` | Factory Binary Firmware Dump |
| `89663-60J50.bin` | **2003–2021** | 992.0 KB | `81d61fbfced11c64bedbd88201c2cc40` | Factory Binary Firmware Dump |
| `89663-60J80.bin` | **2003–2021** | 992.0 KB | `67d72be69ffac266f6f668e430031d21` | Factory Binary Firmware Dump |
| `89663-60K40.bin` | **2003–2021** | 992.0 KB | `8bab7f28376b29f07189405da8c7286b` | Factory Binary Firmware Dump |
| `89663-60K41.bin` | **2003–2021** | 992.0 KB | `ea5dc86500846af9e4adda1771c716e5` | Factory Binary Firmware Dump |
| `89663-60K60.bin` | **2003–2021** | 992.0 KB | `c333a9f5ec648bef7d7178646ca2ad35` | Factory Binary Firmware Dump |
| `89663-60K62.bin` | **2003–2021** | 992.0 KB | `d07c52d3a8de043eeb485f9ba3f6075b` | Factory Binary Firmware Dump |
| `89663-60K90.bin` | **2003–2021** | 992.0 KB | `7a445abd4153ab7d1adfc4f02dd2d8b1` | Factory Binary Firmware Dump |
| `89663-60K91.bin` | **2003–2021** | 992.0 KB | `5eb9e31cfb4df1a48e74bef948671953` | Factory Binary Firmware Dump |
| `89663-60L20.bin` | **2003–2021** | 992.0 KB | `2b83a7eba7aed042c453e109c1432f9e` | Factory Binary Firmware Dump |
| `89663-60L21.bin` | **2003–2021** | 992.0 KB | `c8cf943fa8a05d58790d3b3eaffc405b` | Factory Binary Firmware Dump |
| `89663-60L50.bin` | **2003–2021** | 992.0 KB | `f67769e9162c49444bc4913369459392` | Factory Binary Firmware Dump |
| `89663-60M50.bin` | **2003–2021** | 992.0 KB | `d70c01fb29c20c9752926c288ccdf219` | Factory Binary Firmware Dump |
| `89663-60N40.bin` | **2003–2021** | 992.0 KB | `2f92d3aab6c10abe9e943cbbe6c6f971` | Factory Binary Firmware Dump |
| `89663-60N41.bin` | **2003–2021** | 992.0 KB | `ca900f6d5bdeb7b205242d02c86ad540` | Factory Binary Firmware Dump |
| `89663-60N70.bin` | **2003–2021** | 992.0 KB | `442d6da4ee189ecd7876bb25c2a5fb23` | Factory Binary Firmware Dump |
| `89663-60N72.bin` | **2003–2021** | 992.0 KB | `b28364e528a442ec814ae7e91451cdb7` | Factory Binary Firmware Dump |
| `89663-60N73.bin` | **2003–2021** | 992.0 KB | `71bc9f784136ee174deb161d63fa3d58` | Factory Binary Firmware Dump |
| `89663-60N74.bin` | **2003–2021** | 992.0 KB | `c30e237a55afc67665db201678c33087` | Factory Binary Firmware Dump |
| `89663-60P10.bin` | **2003–2021** | 992.0 KB | `10d151913b8c200d835d8ce83ab37a04` | Factory Binary Firmware Dump |
| `89663-60P90.bin` | **2003–2021** | 992.0 KB | `d4f3405846b6bf782f8b6b5035670aba` | Factory Binary Firmware Dump |
| `89663-60U90.bin` | **2003–2021** | 992.0 KB | `3b9d0fc4a313aa2fb6209a5f4aa4854a` | Factory Binary Firmware Dump |
| `89663-60U91.bin` | **2003–2021** | 992.0 KB | `1a5b4ee738e707b7c97f8bcfe754075a` | Factory Binary Firmware Dump |
| `89663-60V20.bin` | **2003–2021** | 992.0 KB | `11a24183c8df46b9287d913130ac017e` | Factory Binary Firmware Dump |
| `89663-60V60.bin` | **2003–2021** | 992.0 KB | `8c1d5e80fa0496784a3e0961c58cf8ce` | Factory Binary Firmware Dump |
| `Original.bin` | **2003–2021** | 512.0 KB | `cb7c243d17c7a5d7208970152f54e9e1` | Factory Binary Firmware Dump |

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
