# FIAT COUPE PUNTO BINS Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform FIAT COUPE PUNTO BINS.

* **Rentang Tahun / Model Year**: 1993–2000
* **Total File Terdaftar**: 3 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `BOOSTchip_Fiat_punto099.bin` | **1993–2000** | 32.0 KB | `6ef9631617645a9e84c67c8dafde1698` | Factory Binary Firmware Dump |
| `FIAT_COUPE_16VT_IMMO.BIN` | **1993–2000** | 32.0 KB | `fbb413ee43ec4c6603be6465495310df` | Factory Binary Firmware Dump |
| `FiatPuntoGt099_140.bin` | **1993–2000** | 32.0 KB | `753af9e4f2067ff1a68c327e29b8cffe` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
