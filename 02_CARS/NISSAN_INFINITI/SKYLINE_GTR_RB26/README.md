# SKYLINE GTR RB26 Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform SKYLINE GTR RB26.

* **Rentang Tahun / Model Year**: 1989–2002
* **Total File Terdaftar**: 6 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `BNCR33_RB26DETT_24U00.bin` | **1989–2002** | 32.0 KB | `76eab1f407eccc121e1829a4be5e6af7` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U02_MT_MECR128.bin` | **1989–1994** | 32.0 KB | `7ec4c92bc09498595fbc61d1e883299e` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U03_MT_MEC-R138.BIN` | **1989–1994** | 32.0 KB | `6687444c0f098e91f418cfab02a1a67f` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U60_MT_MECR280.bin` | **1989–1994** | 32.0 KB | `c4173c0ff5051ee9b90766ee869475ef` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U61_MT_MECR281.bin` | **1989–1994** | 32.0 KB | `bbe7a861efd6813e88a8d4e7805cafe7` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U62_MT_MECR282A.BIN` | **1989–1994** | 32.0 KB | `3269f74f11578842638c456048c8b517` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
