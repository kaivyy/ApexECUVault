# 🏎️ Suite Kalibrasi ECU: FERRARI 488 GTB 3.9L Twin Turbo (2015-2023)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Ferrari 488 GTB 3.9L Twin Turbo**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Ferrari 488 GTB 3.9L Twin Turbo
- **Tahun Produksi**: 2015-2023
- **Kode Part ECU**: `0261S12450`
- **Arsitektur ECU**: Ferrari 488 GTB 3.9L Twin-Turbo F154CB 90° V8 (Bosch MED17.3.5 TriCore 4MB)
- **Ukuran Flash ROM**: `4096 KB` (4,194,304 bytes)
- **Tenaga Pabrik (Stock)**: 670HP (Rev Limit: 8000 RPM | Top Speed Limiter: 330 km/h)
- **Potensi Stage 1 Remap**: 750HP_Boost1.6bar (Rev Limit: 8400 RPM | Top Speed Limiter: 355 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_0261S12450_Ferrari_488_GTB_3.9L_Twin_Turbo_(2015-2023)_670HP.bin` | 4096 KB | Binary dump firmware asli pabrik murni (*unmodified baseline*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_0261S12450_Ferrari_488_GTB_3.9L_Twin_Turbo_750HP_Boost1.6bar.bin` | 4096 KB | Kalibrasi tuning Stage 1 (peningkatan boost, timing pengapian, bukaan throttle, dan limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_0261S12450_Ferrari_488_GTB_3.9L_Twin_Turbo_(2015-2023).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive Modes & Throttle Response**: Bukaan katup gas elektronik (Manettino / ANIMA / Track / Sport Plus).
4. **Turbo Boost & Wastegate** (jika berturbo): Target tekanan absolut boost (mbar) dan wastegate duty cycle.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, dan penghapusan governor kecepatan.
