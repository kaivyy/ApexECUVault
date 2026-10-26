# BMW E46 ZF Automatic Transmission TCU GS20 Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi biner hardware dump asli dan definisi TunerPro XDF untuk unit kontrol transmisi otomatis (Transmission Control Unit - TCU) Siemens GS20 pada BMW E46 330i/325i dengan transmisi ZF 5HP19. Mengatur shift map, TCC lockup timing, serta display gear mode Sport.

* **Hardware / ECU**: Siemens GS20 TCU (64KB EEPROM/Flash)
* **Metode Flashing & Antarmuka**: K+DCAN OBD flashing via Tool32 / WinKFP / TunerPro RT.
* **Rentang Tahun / Model Year**: 1998–2006
* **Total File Terdaftar**: 2 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `GS20_90C0_64KB.bin` | **1998–2006** | 64.0 KB | `4d41ca20706be9963c4bb618188f0be2` | Factory Binary Firmware Dump |
| `Siemens_GS20_G10C9000_7552700_64K.xdf` | **1998–2006** | 949.7 KB | `c69d529314b99b0b5a9eab32e95b9c21` | TunerPro Binary Definition Map |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
