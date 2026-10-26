# Honda OBD1 PGM-FI Master Baserom Tuning Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi biner baserom kalibrasi Honda OBD1 32KB resmi dari BMTune Development Suite untuk ECU P28, P30, P72, PR4 pada platform mesin D16, B16, B18, H22. Mendukung real-time emulation, sensor scaling 3-4 bar MAP, launch control, full throttle shift, dan closed-loop wideband O2 target control.

* **Hardware / ECU**: Honda OBD1 ECU (P28, P30, P72) dengan 27C256 32KB EPROM / Moates Ostrich 2.0 / CobraRTP Honda Edition
* **Metode Flashing & Antarmuka**: EPROM Programmer (TL866/T48) atau RTP USB Direct via BMTune / Crome / HTS.
* **Total File Terdaftar**: 30 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

| Filename | Size | MD5 Checksum | Type / Target |
| :--- | :--- | :--- | :--- |
| `BMTune_V1.0.0.bin` | 32.0 KB | `f70dca12e790e887447a460f8b40e601` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.1.bin` | 32.0 KB | `a6a33c26b5a20971bfad769dce126bec` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.2.bin` | 32.0 KB | `7f1d013a43353fe1d2ca4a40d0ca0f45` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.2_NO_MOD.bin` | 32.0 KB | `162ef252b2dc5d3703028e1a9a15cce8` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.3.bin` | 32.0 KB | `4bbfdd7241811528f31fa9149cc8d28e` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.3_NO_MOD.bin` | 32.0 KB | `eb49ea1df7633c28bf17202a67cfe57e` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.4.bin` | 32.0 KB | `9e10c86989d97117ff5a7aef25e69a64` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.4_NO_MOD.bin` | 32.0 KB | `fa5d39417eb08f3dae74b39e4e09b471` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.5.bin` | 32.0 KB | `87bb8d90f3aa01f48a7e2be97f9fdbca` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.5_NO_MOD.bin` | 32.0 KB | `1bbae2f71585a79ea60a65cc5b9face9` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.6.bin` | 32.0 KB | `cb9b7bb00e990f9b9782416d8ad46d4e` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.6_NO_MOD.bin` | 32.0 KB | `5efcd35a9ad1fd65b3dd24e74365cd10` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.7.bin` | 32.0 KB | `4f2be07be613adcb4aa5812837a36204` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.7_NO_MOD.bin` | 32.0 KB | `2493805c36d0d7ffa4eb3a5b3721a8d1` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.8.bin` | 32.0 KB | `8686b23133c64c3a17b2e46768a4e39b` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.8_NO_MOD.bin` | 32.0 KB | `b8878313ae57a69829a61ae37c726e6d` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.9.bin` | 32.0 KB | `672533024a8247c01c5283d9b83859a3` | Raw Binary Firmware / Dump |
| `BMTune_V1.0.FF.bin` | 32.0 KB | `d55c392b5635701ac5ab10b62f559417` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.0.bin` | 32.0 KB | `57054941ac36cb2a626eee5486263f6d` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.1.bin` | 32.0 KB | `59c5676665a4eae698ea7200ab573701` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.2.bin` | 32.0 KB | `5d2e9cc74073836b63c7f2394ab3c9b1` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.3.bin` | 32.0 KB | `46e27344177034a1c131e1c426efcbb2` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.4.bin` | 32.0 KB | `d9a489751e4b69383a3f397e37214a7c` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.5.bin` | 32.0 KB | `0f091f658761602df7a24783683be0dd` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.6.bin` | 32.0 KB | `e2d5f1ed837f5b80955ebfd8817aef27` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.7.bin` | 32.0 KB | `b3bbf2e6ebe22b917849a7926c5d491b` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.8.bin` | 32.0 KB | `7f8a7e96cb9809a1b86129128c020073` | Raw Binary Firmware / Dump |
| `BMTune_V1.1.9.bin` | 32.0 KB | `2fe160836452f1e3760d3f1beb4b4901` | Raw Binary Firmware / Dump |
| `BMTune_V1.2.0.bin` | 32.0 KB | `090f492ee63b095f3ce49f854db74a24` | Raw Binary Firmware / Dump |
| `BMTune_V1.2.1.bin` | 32.0 KB | `36f4cd9375ed1c94fd39f5627a55e02c` | Raw Binary Firmware / Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
