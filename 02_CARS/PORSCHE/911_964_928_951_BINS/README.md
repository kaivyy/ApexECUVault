# 911 964 928 951 BINS Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform 911 964 928 951 BINS.

* **Rentang Tahun / Model Year**: 1984–1994
* **Total File Terdaftar**: 10 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `0280 002 506_89_90_928GT.bin` | **1989–1990** | 16.0 KB | `a42f8772f60b5349d465505f92808e21` | Factory Binary Firmware Dump |
| `1992_964C2_181240302612004.bin` | **1992** | 32.0 KB | `4a80379710ad06693272201065435fd1` | Factory Binary Firmware Dump |
| `84 Carrera OE EUR 1267355099.BIN` | **1984** | 2.0 KB | `06ef03234fc31811452f6b858a6da12e` | Factory Binary Firmware Dump |
| `84 Carrera OE USA 1267355102.BIN` | **1984** | 2.0 KB | `42da250a6baea01947a93d296a2e9b01` | Factory Binary Firmware Dump |
| `86 Carrera OE EUR 1267355027.BIN` | **1986** | 4.0 KB | `838570336bf5296e7fcccf58bc0b61f1` | Factory Binary Firmware Dump |
| `86 Carrera OE USA 1267355180.BIN` | **1986** | 4.0 KB | `a93082beaf43be3062ceea3eb718d600` | Factory Binary Firmware Dump |
| `87 Carrera OE USA 1267355236.BIN` | **1987** | 4.0 KB | `65e847abf81cd3b82d1ef666c9513aca` | Factory Binary Firmware Dump |
| `Porsche951DME24pin.bin` | **1984–1994** | 4.0 KB | `b1f78205c945d31bb8aade9a93ed3291` | Factory Binary Firmware Dump |
| `Porsche951DME28pin.BIN` | **1984–1994** | 8.0 KB | `ea9d6a82002b68d0b03229c535ce6c4b` | Factory Binary Firmware Dump |
| `gt-91_0280.002.509.bin` | **1984–1994** | 32.0 KB | `98b96e6d79eb8f8f31219aac0967ac65` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
