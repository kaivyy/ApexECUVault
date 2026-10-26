# GOLF VR6 ABA BINS Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform GOLF VR6 ABA BINS.

* **Rentang Tahun / Model Year**: 1992–1998
* **Total File Terdaftar**: 6 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `0261203219_soft109.bin` | **1992–1998** | 64.0 KB | `60542b159fae38a22d365e0d4360bc94` | Factory Binary Firmware Dump |
| `ABA_OBD1_AA.BIN` | **1992–1998** | 64.0 KB | `15679eed51c586319e3a564cb6fa65ff` | Factory Binary Firmware Dump |
| `ABA_OBD1_AE.bin` | **1992–1998** | 64.0 KB | `7ac9542e53ac6edffa3d4f47e46ad8f7` | Factory Binary Firmware Dump |
| `ABA_OBD1_AH.bin` | **1992–1998** | 64.0 KB | `9d13af3043ee1c865fdebffeaafa154f` | Factory Binary Firmware Dump |
| `VR6_0261203117_021906258AF_357529_27C512.bin` | **1992–1998** | 64.0 KB | `1ecf38e31ba7de233981b2598bb3db7b` | Factory Binary Firmware Dump |
| `VW golf 2.8 VR6 AAA 021906258A 0261200496 357205.bin` | **1992–1998** | 64.0 KB | `dc1b1c577f336811f8f506af1aacbaff` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
