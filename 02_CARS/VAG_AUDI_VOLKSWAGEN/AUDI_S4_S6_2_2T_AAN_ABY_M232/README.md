# Audi S4/S6 2.2L Turbo 20V AAN / S2 ABY Bosch Motronic M2.3.2 Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi dump biner EPROM pabrikan asli (stock) dan modifikasi kalibrasi untuk mesin legendaris 5-silinder 2.2 Turbo 20V kode AAN (Audi S4/S6 C4) dan ABY (Audi S2 Coupe/Avant). Menggunakan ECU Bosch Motronic M2.3.2 dengan konfigurasi dual-EPROM (Boost control 27C256 / 87C257 dan Fuel/Ignition 27C512).

* **Hardware / ECU**: Bosch Motronic M2.3.2 (Dual DIP EPROM: 27C256/87C257 32KB & 27C512 64KB)
* **Metode Flashing & Antarmuka**: Socketing EPROM programmer (TL866II Plus / T48) atau CobraRTP MotronicRT dual channel.
* **Rentang Tahun / Model Year**: 1991–1997
* **Total File Terdaftar**: 4 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `bigturbo_WMI_27c512.bin` | **1991–1997** | 64.0 KB | `416e5f10ac4ebbc33a3ff9293ca9ca5f` | Factory Binary Firmware Dump |
| `bigturbo_WMI_87c257.bin` | **1991–1997** | 32.0 KB | `9ffa47b5d495e70b28c36c8f01329862` | Factory Binary Firmware Dump |
| `stock_AANABY_27c512.bin` | **1991–1997** | 64.0 KB | `6aa9cb08d0d27ce9adfa7f44be6f6f7a` | Factory Binary Firmware Dump |
| `stock_AANABY_87c257.bin` | **1991–1997** | 32.0 KB | `a94c0fddcb4a353043773a3a45347cd7` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
