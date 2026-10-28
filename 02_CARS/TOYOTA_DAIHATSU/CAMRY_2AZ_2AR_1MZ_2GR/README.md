# CAMRY_2AZ_2AR_1MZ_2GR - ECU Calibration Suite

**Repository Path**: `02_CARS/TOYOTA_DAIHATSU/CAMRY_2AZ_2AR_1MZ_2GR`  
**Classification**: `OEM Binary Firmware & Factory Calibration Suite`  
**Total Managed Assets**: `50 files` (50 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CAMRY_2AZ_2AR_1MZ_2GR` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta berkas definisi komprehensif (TunerPro XDF, ASAM ASAP2 A2L, WinOLS DAMOS/KP/OLS) untuk identifikasi parameter mesin presisi.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

* **Rentang Tahun / Model Year**: 2002–2020

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `89663-06431.bin` | **2002–2020** | 736.0 KB | `d15c3a22205f97fe4f9ea8d4e1099584` | Factory Binary Firmware Dump |
| `89663-06693.bin` | **2002–2020** | 992.0 KB | `fcd3892fe43f8244f518341c0186752a` | Factory Binary Firmware Dump |
| `89663-06772.bin` | **2002–2020** | 992.0 KB | `0baf4f54d134bd0cf0ae62c098c4ffa4` | Factory Binary Firmware Dump |
| `89663-06791.bin` | **2002–2020** | 992.0 KB | `848f3d102008b69d45af73efa4b9aafd` | Factory Binary Firmware Dump |
| `89663-06805.bin` | **2002–2020** | 992.0 KB | `9a218ea14933942c52e2832609a9b556` | Factory Binary Firmware Dump |
| `89663-06A31.bin` | **2002–2020** | 992.0 KB | `742affb6f15e9ca15bbd148c834ee206` | Factory Binary Firmware Dump |
| `89663-06A35.bin` | **2002–2020** | 992.0 KB | `9c0ccab2d392fbf346aa23074d8a85b0` | Factory Binary Firmware Dump |
| `89663-06A45.bin` | **2002–2020** | 992.0 KB | `87cf1b53cbc5a6a365c32756ce88f755` | Factory Binary Firmware Dump |
| `89663-06D40.bin` | **2002–2020** | 992.0 KB | `7f1fa6c29551ff417b5b10567c23855f` | Factory Binary Firmware Dump |
| `89663-06D50.bin` | **2002–2020** | 992.0 KB | `8ed6e1a6a5018ab2b4159a11e4435876` | Factory Binary Firmware Dump |
| `89663-06G23.bin` | **2002–2020** | 1.50 MB | `659fd5d5c35f652ea925833f62c22f80` | Factory Binary Firmware Dump |
| `89663-33021.bin` | **2002–2020** | 320.0 KB | `2ebd7847cb579ca406211afa9efae3f8` | Factory Binary Firmware Dump |
| `89663-33041.bin` | **2002–2020** | 320.0 KB | `15e5a676dc6806611d6f00b420d7a094` | Factory Binary Firmware Dump |
| `89663-33054.bin` | **2002–2020** | 320.0 KB | `fcc7ad6fa6e21834084c9da7da77040d` | Factory Binary Firmware Dump |
| `89663-33340.bin` | **2002–2020** | 736.0 KB | `070220d642b51b503f5f700c4224c392` | Factory Binary Firmware Dump |
| `89663-33371.bin` | **2002–2020** | 320.0 KB | `b81c856b4f1e4bb89c141ecedbc0eba7` | Factory Binary Firmware Dump |
| `89663-33372.bin` | **2002–2020** | 320.0 KB | `404e06519c2159f451c4e2d18de6583a` | Factory Binary Firmware Dump |
| `89663-33391.bin` | **2002–2020** | 320.0 KB | `482e6635141e534f0c123beb74903ee8` | Factory Binary Firmware Dump |
| `89663-33392.bin` | **2002–2020** | 320.0 KB | `4e34247cbc892e21e91bef5294275cb8` | Factory Binary Firmware Dump |
| `89663-33401.bin` | **2002–2020** | 368.0 KB | `15937926b5a55ff37e0309527f73fec4` | Factory Binary Firmware Dump |
| `89663-33432.bin` | **2002–2020** | 384.0 KB | `afab3573621784fa3c68d776af80282d` | Factory Binary Firmware Dump |
| `89663-33434.bin` | **2002–2020** | 384.0 KB | `45acb25035cd1b768de587b6962b5db9` | Factory Binary Firmware Dump |
| `89663-33442.bin` | **2002–2020** | 496.0 KB | `53749ae64fece40be18b6d9c3b586633` | Factory Binary Firmware Dump |
| `89663-33443.bin` | **2002–2020** | 496.0 KB | `e06248be0430cc6934833cbca12ebfec` | Factory Binary Firmware Dump |
| `89663-33541.bin` | **2002–2020** | 384.0 KB | `e6cef3b0b7f577dbb933c0be92ef6e0e` | Factory Binary Firmware Dump |
| `89663-33542.bin` | **2002–2020** | 384.0 KB | `bc08a0d46839c5c7a8de8673209b877c` | Factory Binary Firmware Dump |
| `89663-33551.bin` | **2002–2020** | 384.0 KB | `35d0e0bb6c5e1f68e9844f8cfbf37cd3` | Factory Binary Firmware Dump |
| `89663-33561.bin` | **2002–2020** | 384.0 KB | `6f0edcf1de3382196089aacfacbe24b0` | Factory Binary Firmware Dump |
| `89663-33581.bin` | **2002–2020** | 736.0 KB | `a2179b2b9d10188121849de899b47f9d` | Factory Binary Firmware Dump |
| `89663-33591.bin` | **2002–2020** | 736.0 KB | `f07c1b74f9ef39ad7c9956a26851fb4c` | Factory Binary Firmware Dump |
| `89663-33661.bin` | **2002–2020** | 736.0 KB | `9cd71c352b2bad558a30bf6286edf5fc` | Factory Binary Firmware Dump |
| `89663-33681.bin` | **2002–2020** | 736.0 KB | `d9e335fbe7dacbefa691d8b5416f14ac` | Factory Binary Firmware Dump |
| `89663-33721.bin` | **2002–2020** | 736.0 KB | `77f0467d7425b111d32b81128a769829` | Factory Binary Firmware Dump |
| `89663-33822.bin` | **2002–2020** | 736.0 KB | `5ae7246c6abbfd08da4a8491be3d076e` | Factory Binary Firmware Dump |
| `89663-33832.bin` | **2002–2020** | 736.0 KB | `3685eae58b5857e089094c9ed615949b` | Factory Binary Firmware Dump |
| `89663-33880.bin` | **2002–2020** | 384.0 KB | `c93e66ec6efd314eadc0abb52d914a78` | Factory Binary Firmware Dump |
| `89663-33881.bin` | **2002–2020** | 384.0 KB | `c7a8c3251eff43ca989b1c353185a68d` | Factory Binary Firmware Dump |
| `89663-33890.bin` | **2002–2020** | 384.0 KB | `1a5a4b506e3c811f370aa8fc73b7f692` | Factory Binary Firmware Dump |
| `89663-33891.bin` | **2002–2020** | 384.0 KB | `6e7dec971bd2d67590b26e42b99e1ca7` | Factory Binary Firmware Dump |
| `89663-33A50.bin` | **2002–2020** | 736.0 KB | `a1d9d6377f11778c1aaf01b6a95be079` | Factory Binary Firmware Dump |
| `89663-33A51.bin` | **2002–2020** | 736.0 KB | `66646c127dbbbb3c2031cef3f155c89b` | Factory Binary Firmware Dump |
| `89663-33A52.bin` | **2002–2020** | 736.0 KB | `a0391b2e09fbe85bc27b692de79b977b` | Factory Binary Firmware Dump |
| `89663-33A60.bin` | **2002–2020** | 736.0 KB | `a0ca98170ed5a764ef38f5e79b64de35` | Factory Binary Firmware Dump |
| `89663-33A61.bin` | **2002–2020** | 736.0 KB | `dd88c3973d67b2c29a285f70e3a09702` | Factory Binary Firmware Dump |
| `89663-33A70.bin` | **2002–2020** | 736.0 KB | `146d191e52e39bebc4fee64a8448eaa4` | Factory Binary Firmware Dump |
| `89663-33A71.bin` | **2002–2020** | 736.0 KB | `8cd47109e9743e3d100edef798d255a7` | Factory Binary Firmware Dump |
| `89663-33A72.bin` | **2002–2020** | 736.0 KB | `1e2faeab9b567ea5c112f5cb59fb8f63` | Factory Binary Firmware Dump |
| `89663-33A74.bin` | **2002–2020** | 736.0 KB | `96aaa61b6e0d63f1390de314069368a4` | Factory Binary Firmware Dump |
| `89663-33D71.bin` | **2002–2020** | 992.0 KB | `e3e9c99a9aefb71db864f331ba8afd04` | Factory Binary Firmware Dump |
| `89663-33G81.bin` | **2002–2020** | 992.0 KB | `27e9368fdd55f7108ae5cd538cf6a2e2` | Factory Binary Firmware Dump |

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
