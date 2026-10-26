# 📁 Suite Kalibrasi ECU: LAND_ROVER Defender D300 3.0D Ingenium (2020-2026)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Land_Rover Defender D300 3.0D Ingenium**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Land_Rover Defender D300 3.0D Ingenium
- **Tahun Produksi**: 2020-2026
- **Kode Part ECU**: `LR156230`
- **Arsitektur ECU**: Land Rover Defender L663 D300 3.0L Diesel Inline-6 (Bosch MD1CS003 4MB)
- **Ukuran Flash ROM**: `4096 KB` (4,194,304 bytes)
- **Tenaga Pabrik (Stock)**: 300HP (Rev Limit: 4600 RPM | Top Speed Limiter: 191 km/h)
- **Potensi Stage 1 Remap**: 360HP_750NM (Rev Limit: 5000 RPM | Top Speed Limiter: 235 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_LR156230_Land_Rover_Defender_D300_3.0D_Ingenium_(2020-2026)_300HP.bin` | 4096 KB | Binary dump firmware asli pabrik murni (*unmodified calibration*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_LR156230_Land_Rover_Defender_D300_3.0D_Ingenium_360HP_750NM.bin` | 4096 KB | Kalibrasi tuning Stage 1 yang dioptimalkan (AFR/Rail, BTDC timing, DBW response, RPM & Speed limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_LR156230_Land_Rover_Defender_D300_3.0D_Ingenium_(2020-2026).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

---

## 🛠️ Peta Tabel yang Didefinisikan dalam XDF

Suite ini mencakup tabel-tabel kalibrasi utama:
1. **Fuel Injection & AFR Target**: Base fuel map, open-loop target lambda, cold enrichment.
2. **Ignition Timing (BTDC)**: Optimal spark advance, knock recovery retard, low/high det maps.
3. **Drive-by-Wire (DBW) Throttle**: Pemetaan sudut pedal akselerator ke bukaan katup gas elektronik (menghilangkan lag pedal gas).
4. **Variable Valve Timing (VVT / MIVEC / i-VTEC / CVVT)**: Sudut pergeseran kem intake/exhaust untuk efisiensi volumetrik maksimum.
5. **Rev & Speed Limiters**: Hard fuel cut, soft spark retard, penghapusan governor kecepatan 180 km/h.
### 🎛️ Fitur Drive-Mode Mapping & Torque Matrix
ECU ini memiliki peta kalibrasi individual terpisah untuk setiap mode berkendara (*Drive Mode Select*):
1. **NORMAL MODE**: Respons pedal linier halus, efisiensi bahan bakar harian seimbang.
2. **WET / SLIPPERY MODE**: Reduksi torsi instan pada putaran awal, integrasi *Active Yaw Control (AYC)* dan *Traction Control* untuk mencegah *wheelspin* di permukaan basah.
3. **GRAVEL / SPORT MODE**: Torsi putaran bawah lebih padat, *drive-by-wire throttle response* lebih agresif untuk traksi di jalan tanah / kerikil.
4. **MUD / OFFROAD MODE**: Toleransi slip ban ditingkatkan, pembagian torsi optimal untuk meloloskan kendaraan dari jebakan lumpur.

### 💨 Parameter Turbo & Boost Target
- **Target Tekanan Boost Stock**: ~1.3 bar absolut.
- **Target Tekanan Boost Stage 1**: ~1.65 bar absolut.
- **Wastegate Duty Cycle**: Dikalibrasi ulang untuk mencegah *boost spike* dan *overboost cut*.


---

## ⚠️ Panduan Keamanan Flashing

1. **Selalu Buat Cadangan (Backup)**: Sebelum melakukan flashing binary modifikasi, baca (*read full flash*) dan simpan file asli dengan nama `STOCK_ORIGINAL_...bin`.
2. **Stabilisator Tegangan**: Selalu gunakan *battery maintainer / stabilizer* 13.5V–14.0V selama proses flashing CANBUS untuk mencegah *bricked ECU*.
3. **Koreksi Checksum**: Pastikan checksum tervalidasi sebelum menyalakan mesin.
