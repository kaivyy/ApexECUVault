# 🏎️ Suite Kalibrasi ECU: PORSCHE 911 Turbo S 3.8L VTG (2013-2026)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Porsche 911 Turbo S 3.8L VTG**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Porsche 911 Turbo S 3.8L VTG
- **Tahun Produksi**: 2013-2026
- **Kode Part ECU**: `99161860700`
- **Arsitektur ECU**: Porsche 911 Turbo S 3.8L Variable Turbine Geometry VTG Twin-Turbo (Bosch MED17 4MB)
- **Ukuran Flash ROM**: `4096 KB` (4,194,304 bytes)
- **Tenaga Pabrik (Stock)**: 580HP (Rev Limit: 7200 RPM | Top Speed Limiter: 330 km/h)
- **Potensi Stage 1 Remap**: 680HP_920NM_Boost1.7bar (Rev Limit: 7600 RPM | Top Speed Limiter: 350 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_99161860700_Porsche_911_Turbo_S_3.8L_VTG_(2013-2026)_580HP.bin` | 4096 KB | Binary dump firmware asli pabrik murni (*unmodified baseline*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_99161860700_Porsche_911_Turbo_S_3.8L_VTG_680HP_920NM_Boost1.7bar.bin` | 4096 KB | Kalibrasi tuning Stage 1 (peningkatan boost, timing pengapian, bukaan throttle, dan limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_99161860700_Porsche_911_Turbo_S_3.8L_VTG_(2013-2026).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive Modes & Throttle Response**: Bukaan katup gas elektronik (Manettino / ANIMA / Track / Sport Plus).
4. **Turbo Boost & Wastegate** (jika berturbo): Target tekanan absolut boost (mbar) dan wastegate duty cycle.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, dan penghapusan governor kecepatan.
