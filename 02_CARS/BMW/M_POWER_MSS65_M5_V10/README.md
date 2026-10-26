# M POWER MSS65 M5 V10 Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform M POWER MSS65 M5 V10.

* **Total File Terdaftar**: 3 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

| Filename | Size | MD5 Checksum | Type / Target |
| :--- | :--- | :--- | :--- |
| `IGN.A2L` | 640.3 KB | `8234c0cae14b51ffbe469e7cf7d1cc6e` | ECU / ASAP2 Calibration Map Definition |
| `INJ.A2L` | 522.1 KB | `8162476abac09c5b7cdc7d7ea57eb7cf` | ECU / ASAP2 Calibration Map Definition |
| `SMG_Release.xdf` | 1.0 KB | `6b84491886acc5d33c165d95361defc7` | TunerPro Binary Definition Map |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
