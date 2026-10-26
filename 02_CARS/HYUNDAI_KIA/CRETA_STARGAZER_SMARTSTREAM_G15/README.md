# 📁 Suite Kalibrasi ECU: HYUNDAI Stargazer Creta 1.5 MPI Smartstream (2022-2026)

Direktori ini memuat file kalibrasi biner firmware (**Original Pabrik** & **Stage 1 Tuned Remap**) beserta file definisi **TunerPro XDF XML** untuk **Hyundai Stargazer Creta 1.5 MPI Smartstream**.

---

## 📋 Informasi Spesifikasi & Identifikasi

- **Merek / Model**: Hyundai Stargazer Creta 1.5 MPI Smartstream
- **Tahun Produksi**: 2022-2026
- **Kode Part ECU**: `39110-04TA0`
- **Arsitektur ECU**: Hyundai Creta & Stargazer 1.5L Smartstream G1.5 (Kefico Sim2K-250 2MB)
- **Ukuran Flash ROM**: `2048 KB` (2,097,152 bytes)
- **Tenaga Pabrik (Stock)**: 115HP (Rev Limit: 6500 RPM | Top Speed Limiter: 180 km/h)
- **Potensi Stage 1 Remap**: 128HP_7000RPM (Rev Limit: 7000 RPM | Top Speed Limiter: 220 km/h)

---

## 🗂️ Daftar File dalam Suite Ini

| Tipe File | Nama File | Ukuran | Deskripsi |
| :--- | :--- | :---: | :--- |
| **STOCK BIN** | `STOCK_ORIGINAL_39110-04TA0_Hyundai_Stargazer_Creta_1.5_MPI_Smartstream_(2022-2026)_115HP.bin` | 2048 KB | Binary dump firmware asli pabrik murni (*unmodified calibration*). |
| **REMAP STAGE 1** | `REMAP_STAGE1_39110-04TA0_Hyundai_Stargazer_Creta_1.5_MPI_Smartstream_128HP_7000RPM.bin` | 2048 KB | Kalibrasi tuning Stage 1 yang dioptimalkan (AFR/Rail, BTDC timing, DBW response, RPM & Speed limiter). |
| **TUNERPRO XDF** | `GENERATIONAL_39110-04TA0_Hyundai_Stargazer_Creta_1.5_MPI_Smartstream_(2022-2026).xdf` | ~8-15 KB | Definisi peta TunerPro V5 lengkap dengan sumbu tabel (RPM, Load, Pedal) dan formula konversi. |

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


---

## ⚠️ Panduan Keamanan Flashing

1. **Selalu Buat Cadangan (Backup)**: Sebelum melakukan flashing binary modifikasi, baca (*read full flash*) dan simpan file asli dengan nama `STOCK_ORIGINAL_...bin`.
2. **Stabilisator Tegangan**: Selalu gunakan *battery maintainer / stabilizer* 13.5V–14.0V selama proses flashing CANBUS untuk mencegah *bricked ECU*.
3. **Koreksi Checksum**: Pastikan checksum tervalidasi sebelum menyalakan mesin.
