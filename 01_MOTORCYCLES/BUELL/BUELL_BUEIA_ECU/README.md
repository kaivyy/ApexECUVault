# BUELL BUEIA ECU Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform BUELL BUEIA ECU.

* **Total File Terdaftar**: 2 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

| Filename | Size | MD5 Checksum | Type / Target |
| :--- | :--- | :--- | :--- |
| `BUEIA_V5.adx` | 105.4 KB | `a5d251d4dcbf081f6d5509993475e982` | TunerPro ADX Datalogging Definition |
| `BUEIA_V5.xdf` | 116.0 KB | `00b217769cd8d3802607c3c39d310cbc` | TunerPro Binary Definition Map |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
