# 🏎️ Suite Kalibrasi ECU: LAMBORGHINI Urus 4.0T V8 (2018-2026)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Lamborghini Urus 4.0T V8**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Lamborghini Urus 4.0T V8
- **Tahun Produksi**: 2018-2026
- **Kode Part ECU**: `4M0907557D`
- **Arsitektur ECU**: Lamborghini Urus 4.0L Twin-Turbo EA825 V8 Super SUV (Bosch MG1CS008 4MB)
- **Ukuran Flash ROM**: `4096 KB` (4,194,304 bytes)
- **Tenaga Pabrik (Stock)**: 650HP (Rev Limit: 6800 RPM | Top Speed Limiter: 305 km/h)
- **Potensi Stage 1 Remap**: 750HP_1000NM_Boost1.8bar (Rev Limit: 7200 RPM | Top Speed Limiter: 335 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_4M0907557D_Lamborghini_Urus_4.0T_V8_(2018-2026)_650HP.bin` | 4096 KB | Binary dump firmware asli pabrik murni (*unmodified baseline*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_4M0907557D_Lamborghini_Urus_4.0T_V8_750HP_1000NM_Boost1.8bar.bin` | 4096 KB | Kalibrasi tuning Stage 1 (peningkatan boost, timing pengapian, bukaan throttle, dan limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_4M0907557D_Lamborghini_Urus_4.0T_V8_(2018-2026).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive Modes & Throttle Response**: Bukaan katup gas elektronik (Manettino / ANIMA / Track / Sport Plus).
4. **Turbo Boost & Wastegate** (jika berturbo): Target tekanan absolut boost (mbar) dan wastegate duty cycle.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, dan penghapusan governor kecepatan.
