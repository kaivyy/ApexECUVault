# HOLDEN AUSTRALIA Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform HOLDEN AUSTRALIA.

* **Total File Terdaftar**: 6 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

| Filename | Size | MD5 Checksum | Type / Target |
| :--- | :--- | :--- | :--- |
| `11.xdf` | 277.6 KB | `5dc439ac730d11ebafcb06a824348e02` | TunerPro Binary Definition Map |
| `1227808_5d_mod2.ecu` | 166.3 KB | `27b68caba26a41cec5934df9daf1a60e` | ECU / ASAP2 Calibration Map Definition |
| `16183082_12_v2b.ecu` | 115.2 KB | `8ba370a19f0c2394eeebd876b9ee504f` | ECU / ASAP2 Calibration Map Definition |
| `83HoldenVS_V8_v2.xdf` | 192.5 KB | `40e2e28565bf901645160d8d9b83b312` | TunerPro Binary Definition Map |
| `A5.xdf` | 179.4 KB | `b53b9ee25c49b5c2f2e5ecb6bcf29993` | TunerPro Binary Definition Map |
| `FB.xdf` | 188.3 KB | `0ead088c544d4790bc107658b9814235` | TunerPro Binary Definition Map |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
