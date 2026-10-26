# 🏎️ Suite Kalibrasi ECU: LAMBORGHINI Huracan LP610-4 5.2L V10 (2014-2024)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Lamborghini Huracan LP610-4 5.2L V10**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Lamborghini Huracan LP610-4 5.2L V10
- **Tahun Produksi**: 2014-2024
- **Kode Part ECU**: `07L907309B`
- **Arsitektur ECU**: Lamborghini Huracan LP610-4 5.2L Odd-Firing V10 (Bosch MED17.1.1 Dual ECU 4MB)
- **Ukuran Flash ROM**: `4096 KB` (4,194,304 bytes)
- **Tenaga Pabrik (Stock)**: 610HP (Rev Limit: 8500 RPM | Top Speed Limiter: 325 km/h)
- **Potensi Stage 1 Remap**: 650HP_8800RPM (Rev Limit: 8800 RPM | Top Speed Limiter: 345 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_07L907309B_Lamborghini_Huracan_LP610-4_5.2L_V10_(2014-2024)_610HP.bin` | 4096 KB | Binary dump firmware asli pabrik murni (*unmodified baseline*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_07L907309B_Lamborghini_Huracan_LP610-4_5.2L_V10_650HP_8800RPM.bin` | 4096 KB | Kalibrasi tuning Stage 1 (peningkatan boost, timing pengapian, bukaan throttle, dan limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_07L907309B_Lamborghini_Huracan_LP610-4_5.2L_V10_(2014-2024).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive Modes & Throttle Response**: Bukaan katup gas elektronik (Manettino / ANIMA / Track / Sport Plus).
4. **Turbo Boost & Wastegate** (jika berturbo): Target tekanan absolut boost (mbar) dan wastegate duty cycle.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, dan penghapusan governor kecepatan.
