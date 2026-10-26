# VW GOLF GTI MK5 MED9 1 Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform VW GOLF GTI MK5 MED9 1.

* **Rentang Tahun / Model Year**: 2004–2009
* **Total File Terdaftar**: 4 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `1K090711S.xdf` | **2004–2009** | 123.0 KB | `b56cf9105edbb814725b5347520376cf` | TunerPro Binary Definition Map |
| `MED9_0261S02469.ecu` | **2004–2009** | 2.34 MB | `1d23e7e7249f4651898389721720872b` | ECU / ASAP2 Calibration Map Definition |
| `MED9_8J0907404D.ecu` | **2004–2009** | 2.75 MB | `f019d1b4527765613d588acbf0f1f956` | ECU / ASAP2 Calibration Map Definition |
| `MED9_STOCK.bin` | **2004–2009** | 2.00 MB | `ccdf0ec340357e2c97d7ef3be8b437c7` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
