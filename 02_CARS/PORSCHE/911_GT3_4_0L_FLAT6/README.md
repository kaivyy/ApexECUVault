# 🏎️ Suite Kalibrasi ECU: PORSCHE 911 GT3 4.0L Flat-6 (2013-2026)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Porsche 911 GT3 4.0L Flat-6**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Porsche 911 GT3 4.0L Flat-6
- **Tahun Produksi**: 2013-2026
- **Kode Part ECU**: `99161860300`
- **Arsitektur ECU**: Porsche 911 GT3 4.0L Naturally Aspirated Flat-6 9000 RPM (Bosch MED17.1.11 4MB)
- **Ukuran Flash ROM**: `4096 KB` (4,194,304 bytes)
- **Tenaga Pabrik (Stock)**: 500HP (Rev Limit: 9000 RPM | Top Speed Limiter: 318 km/h)
- **Potensi Stage 1 Remap**: 535HP_9300RPM (Rev Limit: 9300 RPM | Top Speed Limiter: 335 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_99161860300_Porsche_911_GT3_4.0L_Flat-6_(2013-2026)_500HP.bin` | 4096 KB | Binary dump firmware asli pabrik murni (*unmodified baseline*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_99161860300_Porsche_911_GT3_4.0L_Flat-6_535HP_9300RPM.bin` | 4096 KB | Kalibrasi tuning Stage 1 (peningkatan boost, timing pengapian, bukaan throttle, dan limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_99161860300_Porsche_911_GT3_4.0L_Flat-6_(2013-2026).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive Modes & Throttle Response**: Bukaan katup gas elektronik (Manettino / ANIMA / Track / Sport Plus).
4. **Turbo Boost & Wastegate** (jika berturbo): Target tekanan absolut boost (mbar) dan wastegate duty cycle.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, dan penghapusan governor kecepatan.
