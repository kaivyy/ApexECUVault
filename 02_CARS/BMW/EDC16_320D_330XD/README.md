# EDC16_320D_330XD - ECU Calibration Suite

**Repository Path**: `02_CARS/BMW/EDC16_320D_330XD`  
**Classification**: `Binary Firmware & High-Precision Calibration Definition Suite`  
**Total Managed Assets**: `47 files` (10 binary dumps, 37 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `EDC16_320D_330XD` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2003–2010

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `361811BMWEDC16.ols` | **2003–2010** | 2.13 MB | `6f270c1bf38d9b8f12f5ca765759a3a8` | WinOLS Project Workspace |
| `4M534389.A2L` | **2003–2010** | 11.00 MB | `7869d6fd587f2ba2547c07db84ff1b20` | ASAM ASAP2 ECU Description File |
| `4M702389.A2L` | **2003–2010** | 11.75 MB | `3c419bd4c5ee5316fc7130c93d15f8ee` | ASAM ASAP2 ECU Description File |
| `4ZB1379.A2L` | **2003–2010** | 1.64 MB | `a8ecafde30fd7e910c0a5031bdf4fb3f` | ASAM ASAP2 ECU Description File |
| `4ZB1379.DAM` | **2003–2010** | 874.8 KB | `83d03f07bb1409eeb72ed3511831cdf8` | WinOLS DAMOS Definition Map |
| `4zB1379 (2).dam` | **2003–2010** | 874.8 KB | `83d03f07bb1409eeb72ed3511831cdf8` | WinOLS DAMOS Definition Map |
| `4zB1379.dam` | **2003–2010** | 874.8 KB | `83d03f07bb1409eeb72ed3511831cdf8` | WinOLS DAMOS Definition Map |
| `530D.OLS` | **2003–2010** | 3.12 MB | `eed10a0e58e35010d7294a824b2871b9` | WinOLS Project Workspace |
| `6M962411.A2L` | **2003–2010** | 12.78 MB | `f7cfe638b72527158d524046aa0d4fc9` | ASAM ASAP2 ECU Description File |
| `6P8KB574_a.a2l` | **2003–2010** | 14.99 MB | `1c512c2a9dc0721b8a86793dc28979c3` | ASAM ASAP2 ECU Description File |
| `6PP01390.A2L` | **2003–2010** | 11.21 MB | `74bb3be1c6707cac8470e88f8e13f44e` | ASAM ASAP2 ECU Description File |
| `6PR01390-.A2L` | **2003–2010** | 4.37 MB | `eeb30c3004d324762c783391c7924663` | ASAM ASAP2 ECU Description File |
| `6PR01390.A2L` | **2003–2010** | 12.32 MB | `a895e09d918efb21564e276ca176cc2b` | ASAM ASAP2 ECU Description File |
| `6ZC1179 (2).A2L` | **2003–2010** | 1.67 MB | `0785a5c7a47f119e332bc111299456e9` | ASAM ASAP2 ECU Description File |
| `6ZC1179.A2L` | **2003–2010** | 1.67 MB | `0785a5c7a47f119e332bc111299456e9` | ASAM ASAP2 ECU Description File |
| `6m661411.A2L` | **2003–2010** | 11.24 MB | `eb4ccf01310c0c984f85fa5ae683f2d1` | ASAM ASAP2 ECU Description File |
| `6m661411.hex` | **2003–2010** | 3.52 MB | `a9c75274ada28b903be3dcc7583877f7` | Intel HEX Calibration Firmware |
| `8S9E3383.A2L` | **2003–2010** | 14.64 MB | `acd3e6710065b03c0d0ed536601f5f25` | ASAM ASAP2 ECU Description File |
| `BMW 330XD - EGR OFF _ DPF OFF _ AI STAGE 1.bin` | **2003–2010** | 2.00 MB | `738ffa234b695480dcf5c2641cc7b2c9` | Factory Binary Firmware Dump |
| `BMW 330XD - ORI.bin` | **2003–2010** | 2.00 MB | `7a0b5e3a883087fd9638eb68f8251235` | Factory Binary Firmware Dump |
| `BMW 530d.a2l` | **2003–2010** | 1.67 MB | `0785a5c7a47f119e332bc111299456e9` | ASAM ASAP2 ECU Description File |
| `BMW 530d.dam` | **2003–2010** | 874.8 KB | `83d03f07bb1409eeb72ed3511831cdf8` | WinOLS DAMOS Definition Map |
| `BMW E60 3.0d M57Top DDE 6.0 __429661.ols` | **2003–2010** | 12.18 MB | `2b15cc5e8a5930517bb454ea78eaadbc` | WinOLS Project Workspace |
| `BMW E87 120d DDE5.0 120kW.ols` | **2003–2010** | 14.10 MB | `97d9edce84f129f1c49d523dbeb2bfce` | WinOLS Project Workspace |
| `BMW E87 2.0d M47TÜ2oL DDE 6.0 120kW.ols` | **2003–2010** | 14.10 MB | `9c8c7932b9f39cfa4d4db7034e762df7` | WinOLS Project Workspace |
| `BMW E90 2.0d M47TU2oL DDE 6.0 120kW.ols` | **2003–2010** | 9.44 MB | `0b8514ac51a15ac7ffb956f746943d31` | WinOLS Project Workspace |
| `BMW EDC15C2.ols` | **2003–2010** | 3.00 MB | `095ceb597dd1903e5c7e7e134669e28e` | WinOLS Project Workspace |
| `BMW EDC16.A2L` | **2003–2010** | 14.64 MB | `acd3e6710065b03c0d0ed536601f5f25` | ASAM ASAP2 ECU Description File |
| `BMW EDC16.hex` | **2003–2010** | 5.91 MB | `0823735c8d30ecdac65e9a4e29dcaa81` | Intel HEX Calibration Firmware |
| `BMW EDC17CP09 530D.ols` | **2003–2010** | 15.95 MB | `0940ecf981508861e8d4137388bae7eb` | WinOLS Project Workspace |
| `BMW R6 EDC16.ols` | **2003–2010** | 8.99 MB | `f60fa89fc476e870f8a4c857a9121892` | WinOLS Project Workspace |
| `BMW-120D-DD6.2-EDC16.OLS` | **2003–2010** | 6.71 MB | `d2c06a3b2d1a4564bc0f3b7d01765e6c` | WinOLS Project Workspace |
| `BMW-330D-0 090799 14-0281010314-788016-DAMOS.OLS` | **2003–2010** | 3.07 MB | `cb5e0ed461811f5b8a45c5865a925b41` | WinOLS Project Workspace |
| `BMW-DA.ols` | **2003–2010** | 3.03 MB | `6935ec7942392a601a142e39756234e5` | WinOLS Project Workspace |
| `BMW330d-0281011121 -EDC16C31-ori.ols` | **2003–2010** | 1.50 MB | `f0e8cac1bdb1196c00480acb52115be8` | WinOLS Project Workspace |
| `BMW530d.ols` | **2003–2010** | 3.07 MB | `cb5e0ed461811f5b8a45c5865a925b41` | WinOLS Project Workspace |
| `BMW_30D_EDC16_218PS__E60.ols` | **2003–2010** | 8.99 MB | `f60fa89fc476e870f8a4c857a9121892` | WinOLS Project Workspace |
| `E46 320D - EGR OFF_ STAGE 1 - 1037361858.bin` | **2003–2010** | 1.44 MB | `e677226f36d256322e0379e01235459f` | Factory Binary Firmware Dump |
| `EDC15C4 Damos BMW 530d.ols` | **2003–2010** | 3.07 MB | `cb5e0ed461811f5b8a45c5865a925b41` | WinOLS Project Workspace |
| `EDC16_0281011762.ols` | **2003–2010** | 8.25 MB | `0a3946ee0f62fbc0c7d9b8d51442cd76` | WinOLS Project Workspace |
| `M57hex.hex` | **2003–2010** | 1.24 MB | `0c85a2d6388a0c4abe409a3ee032d0ed` | Intel HEX Calibration Firmware |
| `SC18_CLP_.hex` | **2003–2010** | 1.24 MB | `c290330d532c4525a405b556677d01d4` | Intel HEX Calibration Firmware |
| `SC18_CLP_hex (2).hex` | **2003–2010** | 1.24 MB | `c290330d532c4525a405b556677d01d4` | Intel HEX Calibration Firmware |
| `SC18_CLP_hex.hex` | **2003–2010** | 1.24 MB | `c290330d532c4525a405b556677d01d4` | Intel HEX Calibration Firmware |
| `X_78KBMN022A.hex` | **2003–2010** | 4.81 MB | `4649963aeca1ce362d332c7476612b0e` | Intel HEX Calibration Firmware |
| `bmw_edc16_218PS_30d_e60.ols` | **2003–2010** | 8.99 MB | `f60fa89fc476e870f8a4c857a9121892` | WinOLS Project Workspace |
| `edc15.ols` | **2003–2010** | 3.00 MB | `095ceb597dd1903e5c7e7e134669e28e` | WinOLS Project Workspace |

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
