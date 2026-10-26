# MAZDA MX5 NC 2 0L MZR Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform MAZDA MX5 NC 2 0L MZR.

* **Rentang Tahun / Model Year**: 2005–2015
* **Total File Terdaftar**: 1 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `SW-LFG1EK.BIN` | **2005–2015** | 1.00 MB | `5d6d2e7ceb9476ffa75a55e6c77574da` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
