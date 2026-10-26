# 🏎️ Suite Kalibrasi ECU: FERRARI 458 Italia 4.5L V8 (2009-2015)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Ferrari 458 Italia 4.5L V8**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Ferrari 458 Italia 4.5L V8
- **Tahun Produksi**: 2009-2015
- **Kode Part ECU**: `0261S05820`
- **Arsitektur ECU**: Ferrari 458 Italia 4.5L 90° Flat-Plane Crank V8 (Bosch MED9.6.1 Dual ECU)
- **Ukuran Flash ROM**: `2048 KB` (2,097,152 bytes)
- **Tenaga Pabrik (Stock)**: 570HP (Rev Limit: 9000 RPM | Top Speed Limiter: 325 km/h)
- **Potensi Stage 1 Remap**: 615HP_9300RPM (Rev Limit: 9300 RPM | Top Speed Limiter: 345 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_0261S05820_Ferrari_458_Italia_4.5L_V8_(2009-2015)_570HP.bin` | 2048 KB | Binary dump firmware asli pabrik murni (*unmodified baseline*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_0261S05820_Ferrari_458_Italia_4.5L_V8_615HP_9300RPM.bin` | 2048 KB | Kalibrasi tuning Stage 1 (peningkatan boost, timing pengapian, bukaan throttle, dan limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_0261S05820_Ferrari_458_Italia_4.5L_V8_(2009-2015).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive Modes & Throttle Response**: Bukaan katup gas elektronik (Manettino / ANIMA / Track / Sport Plus).
4. **Turbo Boost & Wastegate** (jika berturbo): Target tekanan absolut boost (mbar) dan wastegate duty cycle.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, dan penghapusan governor kecepatan.
