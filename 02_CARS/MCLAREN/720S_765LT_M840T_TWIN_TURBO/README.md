# 🏎️ Suite Kalibrasi ECU: MCLAREN 720S 4.0L Twin Turbo (2017-2024)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **McLaren 720S 4.0L Twin Turbo**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: McLaren 720S 4.0L Twin Turbo
- **Tahun Produksi**: 2017-2024
- **Kode Part ECU**: `11A0123CP`
- **Arsitektur ECU**: McLaren 720S 4.0L Twin-Turbo Flat-Plane M840T V8 (Bosch MED17.8.33 Dual ECU 4MB)
- **Ukuran Flash ROM**: `4096 KB` (4,194,304 bytes)
- **Tenaga Pabrik (Stock)**: 720HP (Rev Limit: 8200 RPM | Top Speed Limiter: 341 km/h)
- **Potensi Stage 1 Remap**: 820HP_900NM_Boost1.7bar (Rev Limit: 8500 RPM | Top Speed Limiter: 360 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_11A0123CP_McLaren_720S_4.0L_Twin_Turbo_(2017-2024)_720HP.bin` | 4096 KB | Binary dump firmware asli pabrik murni (*unmodified baseline*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_11A0123CP_McLaren_720S_4.0L_Twin_Turbo_820HP_900NM_Boost1.7bar.bin` | 4096 KB | Kalibrasi tuning Stage 1 (peningkatan boost, timing pengapian, bukaan throttle, dan limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_11A0123CP_McLaren_720S_4.0L_Twin_Turbo_(2017-2024).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive Modes & Throttle Response**: Bukaan katup gas elektronik (Manettino / ANIMA / Track / Sport Plus).
4. **Turbo Boost & Wastegate** (jika berturbo): Target tekanan absolut boost (mbar) dan wastegate duty cycle.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, dan penghapusan governor kecepatan.
