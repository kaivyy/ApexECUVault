# 📁 Suite Kalibrasi ECU: SUZUKI Jimny 5 Door 1.5 K15B 4WD (2023-2026)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Suzuki Jimny 5 Door 1.5 K15B 4WD**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Suzuki Jimny 5 Door 1.5 K15B 4WD
- **Tahun Produksi**: 2023-2026
- **Kode Part ECU**: `33920-78R10`
- **Arsitektur ECU**: Suzuki Jimny 5-Door 1.5L K15B 4WD ALLGRIP PRO (Bosch ME17.9.61 2MB)
- **Ukuran Flash ROM**: `2048 KB` (2,097,152 bytes)
- **Tenaga Pabrik (Stock)**: 102HP (Rev Limit: 6200 RPM | Top Speed Limiter: 145 km/h)
- **Potensi Stage 1 Remap**: 115HP_LowEndTorque (Rev Limit: 6800 RPM | Top Speed Limiter: 185 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_33920-78R10_Suzuki_Jimny_5_Door_1.5_K15B_4WD_(2023-2026)_102HP.bin` | 2048 KB | Binary dump firmware asli pabrik murni (*unmodified calibration*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_33920-78R10_Suzuki_Jimny_5_Door_1.5_K15B_4WD_115HP_LowEndTorque.bin` | 2048 KB | Kalibrasi tuning Stage 1 yang dioptimalkan (AFR/Rail, BTDC timing, DBW response, RPM & Speed limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_33920-78R10_Suzuki_Jimny_5_Door_1.5_K15B_4WD_(2023-2026).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

Suite ini mencakup tabel-tabel kalibrasi utama:
1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive-by-Wire (DBW) Throttle**: Pemetaan sudut pedal akselerator ke bukaan katup gas elektronik (menghilangkan lag pedal gas).
4. **Variable Valve Timing (VVT / MIVEC / i-VTEC / CVVT)**: Sudut pergeseran kem intake/exhaust untuk efisiensi volumetrik maksimum.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, penghapusan governor kecepatan 180 km/h.

---

## ⚠️ Panduan Keamanan Flashing

1. **Selalu Buat Cadangan (Backup)**: Sebelum melakukan flashing binary modifikasi, baca (*read full flash*) dan simpan file asli dengan nama `STOCK_ORIGINAL_...bin`.
2. **Stabilisator Tegangan**: Selalu gunakan *battery maintainer / stabilizer* 13.5V–14.0V selama proses flashing CANBUS untuk mencegah *bricked ECU*.
3. **Koreksi Checksum**: Pastikan checksum tervalidasi sebelum menyalakan mesin.
