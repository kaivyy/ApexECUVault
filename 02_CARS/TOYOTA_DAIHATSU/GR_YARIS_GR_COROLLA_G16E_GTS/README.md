# 🏎️ Suite Kalibrasi ECU: TOYOTA GR Corolla 1.6T G16E-GTS (2022-2026)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Toyota GR Corolla 1.6T G16E-GTS**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Toyota GR Corolla 1.6T G16E-GTS
- **Tahun Produksi**: 2022-2026
- **Kode Part ECU**: `89663-12C80`
- **Arsitektur ECU**: Toyota GR Corolla GZEA14 1.6L G16E-GTS High Output Triple Exhaust GR-FOUR
- **Ukuran Flash ROM**: `2048 KB` (2,097,152 bytes)
- **Tenaga Pabrik (Stock)**: 304HP (Rev Limit: 7200 RPM | Top Speed Limiter: 230 km/h)
- **Potensi Stage 1 Remap**: 355HP_Boost1.9bar (Rev Limit: 7700 RPM | Top Speed Limiter: 290 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_89663-12C80_Toyota_GR_Corolla_1.6T_G16E-GTS_(2022-2026)_304HP.bin` | 2048 KB | Binary dump firmware asli pabrik murni (*unmodified baseline*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_89663-12C80_Toyota_GR_Corolla_1.6T_G16E-GTS_355HP_Boost1.9bar.bin` | 2048 KB | Kalibrasi tuning Stage 1 (peningkatan boost, timing pengapian, bukaan throttle, dan limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_89663-12C80_Toyota_GR_Corolla_1.6T_G16E-GTS_(2022-2026).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive Modes & Throttle Response**: Bukaan katup gas elektronik (Manettino / ANIMA / Track / Sport Plus).
4. **Turbo Boost & Wastegate** (jika berturbo): Target tekanan absolut boost (mbar) dan wastegate duty cycle.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, dan penghapusan governor kecepatan.
