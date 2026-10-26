# PRIUS HYBRID 1NZ FXE Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform PRIUS HYBRID 1NZ FXE.

* **Rentang Tahun / Model Year**: 2003–2009
* **Total File Terdaftar**: 4 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `89663-47051.bin` | **2003–2009** | 496.0 KB | `5eea4d975e47830bf15385d16e22c608` | Factory Binary (Toyota Prius 1.5hyb 1NZFXE) |
| `89663-47052.bin` | **2003–2009** | 496.0 KB | `9401d11ad8673eed15badbf0a85f90f7` | Factory Binary (Toyota Prius 1.5hyb 1NZFXE) |
| `89663-47054.bin` | **2003–2009** | 496.0 KB | `2d8669d15ebd6acceeb5d824d7a8bda7` | Factory Binary (Toyota Prius 1.5hyb 1NZFXE) |
| `89663-47102.bin` | **2003–2009** | 496.0 KB | `157c8dd5f6adfb605eeb5e713010d762` | Factory Binary (Toyota Prius 1.5hyb 1NZFXE) |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
