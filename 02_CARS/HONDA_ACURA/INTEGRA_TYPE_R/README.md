# INTEGRA TYPE R Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform INTEGRA TYPE R.

* **Rentang Tahun / Model Year**: 1994–2001
* **Total File Terdaftar**: 25 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `Int338gr.bin` | **1994–2001** | 48.0 KB | `264e10128d8b21727ca37801b08c56cc` | Factory Binary Firmware Dump |
| `Int340ls.bin` | **1994–2001** | 48.0 KB | `575deaa0e55e51431bd31fe795ab1259` | Factory Binary Firmware Dump |
| `Int359tr.bin` | **1994–2001** | 48.0 KB | `0a79ba65e11c63beee11a8e0b46a5b33` | Factory Binary Firmware Dump |
| `Int422gr.bin` | **1994–2001** | 48.0 KB | `429dae21e8e7c68468ad8be82f94992b` | Factory Binary Firmware Dump |
| `Int474gr.bin` | **1994–2001** | 48.0 KB | `f7f01f2db5d9ee7ffba18edf3c13eca2` | Factory Binary Firmware Dump |
| `Int475ls.bin` | **1994–2001** | 48.0 KB | `68613a835f5e6ac68b92ad40dc837ec6` | Factory Binary Firmware Dump |
| `Int497tr.bin` | **1994–2001** | 48.0 KB | `4ca311f462f1d35847b9754ffc567b8b` | Factory Binary Firmware Dump |
| `Int712gr.bin` | **1994–2001** | 48.0 KB | `f4bb112e8924b2354f8409bb06a38930` | Factory Binary Firmware Dump |
| `P73_M66507-715.bin` | **1994–2001** | 48.0 KB | `7abb209ca071708c7f96fee40af640dd` | Factory Binary Firmware Dump |
| `P74-USDM-214.bin` | **1994–2001** | 32.0 KB | `1c7b48c6dd70e23771a9a8c73f7a5cb4` | Factory Binary Firmware Dump |
| `PR3-900-93.bin` | **1994–2001** | 32.0 KB | `37a1d2d4585cff0dde8e3a9e76e2bbbc` | Factory Binary Firmware Dump |
| `PR3GSR.bin` | **1994–2001** | 32.0 KB | `7da9829e2865e9bb9d38a662a46b0ddc` | Factory Binary Firmware Dump |
| `STOCK-PR3.bin` | **1994–2001** | 32.0 KB | `5490eff6ba0981a520ffe499ff0d19f5` | Factory Binary Firmware Dump |
| `int233stock.bin` | **1994–2001** | 32.0 KB | `d8162fe1dd0efd3b8c86187fc8d41517` | Factory Binary Firmware Dump |
| `p2p_p75-rom.bin` | **1994–2001** | 32.0 KB | `92eb7bead98f2a7b92f4c934a6f2d065` | Factory Binary Firmware Dump |
| `p75-q01-270.bin` | **1994–2001** | 32.0 KB | `1786d82785ae4835093db38aa3bff6b5` | Factory Binary Firmware Dump |
| `pr3-901-58.bin` | **1994–2001** | 32.0 KB | `42f24a6afb95f4568e63bc5b20e98b07` | Factory Binary Firmware Dump |
| `pr3-j01-205.bin` | **1994–2001** | 32.0 KB | `3e40bf6b2821e513bdde2e9ce64260df` | Factory Binary Firmware Dump |
| `pr3-j51-219.bin` | **1994–2001** | 32.0 KB | `b1a63fc1a7796f6414bbbfc72c828f60` | Factory Binary Firmware Dump |
| `pr4-USDM-232.bin` | **1994–2001** | 32.0 KB | `33469c6ffe8b506a0c1a8cfbca743a49` | Factory Binary Firmware Dump |
| `pr4-a02.bin.bin` | **1994–2001** | 32.0 KB | `146bdfb053ff2d90612ec9e33e9a74d4` | Factory Binary Firmware Dump |
| `pr4-q02-54.rom` | **1994–2001** | 32.0 KB | `50fc882709993c8b9684de395cf4b81e` | Factory Binary Firmware Dump |
| `pr4-q51-33.bin` | **1994–2001** | 32.0 KB | `c3f4edc311f96aff3d86c19f4694662f` | Factory Binary Firmware Dump |
| `pr4-q60-92.bin` | **1994–2001** | 32.0 KB | `f7cd387a42778e07a1de54b9fe08e105` | Factory Binary Firmware Dump |
| `pr4-q61-235.bin` | **1994–2001** | 32.0 KB | `b9b35ec946dbb080f7c06d95acdb3692` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
