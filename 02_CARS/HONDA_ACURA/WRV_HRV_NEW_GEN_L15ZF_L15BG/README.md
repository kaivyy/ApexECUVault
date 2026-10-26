# 📁 Suite Kalibrasi ECU: HONDA HR-V RS 1.5 VTEC Turbo (2022-2026)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Honda HR-V RS 1.5 VTEC Turbo**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Honda HR-V RS 1.5 VTEC Turbo
- **Tahun Produksi**: 2022-2026
- **Kode Part ECU**: `37820-64A-A01`
- **Arsitektur ECU**: Honda HR-V RS RV5 1.5L VTEC Turbo L15BG (Keihin CAN 2MB)
- **Ukuran Flash ROM**: `2048 KB` (2,097,152 bytes)
- **Tenaga Pabrik (Stock)**: 177HP (Rev Limit: 6500 RPM | Top Speed Limiter: 200 km/h)
- **Potensi Stage 1 Remap**: 215HP_Boost1.4bar (Rev Limit: 6900 RPM | Top Speed Limiter: 260 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_37820-64A-A01_Honda_HR-V_RS_1.5_VTEC_Turbo_(2022-2026)_177HP.bin` | 2048 KB | Binary dump firmware asli pabrik murni (*unmodified calibration*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_37820-64A-A01_Honda_HR-V_RS_1.5_VTEC_Turbo_215HP_Boost1.4bar.bin` | 2048 KB | Kalibrasi tuning Stage 1 yang dioptimalkan (AFR/Rail, BTDC timing, DBW response, RPM & Speed limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_37820-64A-A01_Honda_HR-V_RS_1.5_VTEC_Turbo_(2022-2026).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

Suite ini mencakup tabel-tabel kalibrasi utama:
1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive-by-Wire (DBW) Throttle**: Pemetaan sudut pedal akselerator ke bukaan katup gas elektronik (menghilangkan lag pedal gas).
4. **Variable Valve Timing (VVT / MIVEC / i-VTEC / CVVT)**: Sudut pergeseran kem intake/exhaust untuk efisiensi volumetrik maksimum.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, penghapusan governor kecepatan 180 km/h.
### 💨 Parameter Turbo & Boost Target
- **Target Tekanan Boost Stock**: ~1.0 bar absolut.
- **Target Tekanan Boost Stage 1**: ~1.35 bar absolut.
- **Wastegate Duty Cycle**: Dikalibrasi ulang untuk mencegah *boost spike* dan *overboost cut*.


---

## ⚠️ Panduan Keamanan Flashing

1. **Selalu Buat Cadangan (Backup)**: Sebelum melakukan flashing binary modifikasi, baca (*read full flash*) dan simpan file asli dengan nama `STOCK_ORIGINAL_...bin`.
2. **Stabilisator Tegangan**: Selalu gunakan *battery maintainer / stabilizer* 13.5V–14.0V selama proses flashing CANBUS untuk mencegah *bricked ECU*.
3. **Koreksi Checksum**: Pastikan checksum tervalidasi sebelum menyalakan mesin.
