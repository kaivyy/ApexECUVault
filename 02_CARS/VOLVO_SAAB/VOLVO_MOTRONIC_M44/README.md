# VOLVO MOTRONIC M44 Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform VOLVO MOTRONIC M44.

* **Total File Terdaftar**: 4 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

| Filename | Size | MD5 Checksum | Type / Target |
| :--- | :--- | :--- | :--- |
| `M44_B6304_S90 v0001.xdf` | 152.6 KB | `97afae58347efc5fec34cc036669c92e` | TunerPro Binary Definition Map |
| `M44_B6304_S90_0002.xdf` | 176.0 KB | `3a352dfd891e9951e37c49f3ee324168` | TunerPro Binary Definition Map |
| `S90 V0002 XDF0002 .BIN` | 128.0 KB | `71721563f54247a416a3aa3c47be5f79` | Factory Binary Firmware Dump |
| `Stock S90.BIN` | 128.0 KB | `de4b01098f3157fac610fa5e41c7387c` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
