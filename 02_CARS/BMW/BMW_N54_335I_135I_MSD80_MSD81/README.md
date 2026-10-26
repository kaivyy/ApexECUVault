# BMW N54 3.0L Twin Turbo MSD80 & MSD81 Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi biner biner pabrikan asli dan kalibrasi MapSwitchBase beserta definisi TunerPro XDF untuk mesin legendaris 3.0L Twin-Turbo N54B30 yang terdapat pada BMW E90/E92/E93 335i, E82 135i, E89 Z4 35i, dan E60 535i. Didukung oleh DME Siemens MSD80 dan MSD81 (TriCore TC1796, 2MB Flash ROM).

* **Hardware / ECU**: Siemens VDO MSD80 / MSD81 (Infineon TriCore TC1796, 2MB Flash ROM)
* **Metode Flashing & Antarmuka**: K+DCAN USB OBD2 flashing via MHD N54 Flasher, INPA/Winkfp, atau MPPS/Kess.
* **Rentang Tahun / Model Year**: 2006–2010
* **Total File Terdaftar**: 16 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `I8A0S.xdf` | **2006–2010** | 1.06 MB | `fe61acf4f2f17fc29c0a6958ed7bba38` | TunerPro Binary Definition Map |
| `I8A0S_Legacy.xdf` | **2006–2010** | 674.8 KB | `824388ff095dbd1a4175a5a138605327` | TunerPro Binary Definition Map |
| `I8A0S_MapSwitchBase.bin` | **2006–2010** | 2.00 MB | `8a86b378007d508f7e6aef99199c0787` | Factory Binary Firmware Dump |
| `I8A0S_original.bin` | **2006–2010** | 2.00 MB | `b13d862b98e7ab3a9db9630287ca8f89` | Factory Binary Firmware Dump |
| `IJE0S.xdf` | **2006–2010** | 1.07 MB | `b60c3320fb71f2cdbcc799254f147c9c` | TunerPro Binary Definition Map |
| `IJE0S_Legacy.xdf` | **2006–2010** | 732.7 KB | `313401cf2e1166f02ff32ff6b75efe63` | TunerPro Binary Definition Map |
| `IJE0S_MapSwitchBase.bin` | **2006–2010** | 2.00 MB | `814231afd91ba2f09881d63be02d42f8` | Factory Binary Firmware Dump |
| `IJE0S_original.bin` | **2006–2010** | 2.00 MB | `0ece9d8f4e611dfea47c74862e5ce273` | Factory Binary Firmware Dump |
| `IKM0S.xdf` | **2006–2010** | 1.04 MB | `cc4f9f2c99c35d1e30f7b2235ec7c539` | TunerPro Binary Definition Map |
| `IKM0S_Legacy.xdf` | **2006–2010** | 695.1 KB | `a5442dd4d1093777fa5751417bc8ac75` | TunerPro Binary Definition Map |
| `IKM0S_MapSwitchBase.bin` | **2006–2010** | 2.00 MB | `dcea457d33a487d7ca4c20abbd4bf8b3` | Factory Binary Firmware Dump |
| `IKM0S_original.bin` | **2006–2010** | 2.00 MB | `83e0137005894071e935178d5cca44c0` | Factory Binary Firmware Dump |
| `INA0S.xdf` | **2006–2010** | 1.05 MB | `7d38bd739c8fac807d960708afaee9b6` | TunerPro Binary Definition Map |
| `INA0S_Legacy.xdf` | **2006–2010** | 718.1 KB | `ee528627452b0fd78dc4d31ed283ee90` | TunerPro Binary Definition Map |
| `INA0S_MapSwitchBase.bin` | **2006–2010** | 2.00 MB | `c2ffb0415b9d01a3d0c321db5bb9738c` | Factory Binary Firmware Dump |
| `INA0S_original.bin` | **2006–2010** | 2.00 MB | `09c7e7fad5ac497358ba1a85a24141c7` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
