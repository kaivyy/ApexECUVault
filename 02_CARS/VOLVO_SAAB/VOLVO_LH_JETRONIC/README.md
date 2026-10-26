# VOLVO LH JETRONIC Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform VOLVO LH JETRONIC.

* **Rentang Tahun / Model Year**: 1984–1993
* **Total File Terdaftar**: 17 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `0227400208_2227355740_EZK116.bin` | **1984–1993** | 32.0 KB | `c990ca22b7298c3e1ffb4be3498462b1` | Factory Binary Firmware Dump |
| `0280-000-560.BIN` | **1984–1993** | 32.0 KB | `a5d6f19f0197b180279220da1a01be0e` | Factory Binary Firmware Dump |
| `0280-000-913.BIN` | **1984–1993** | 32.0 KB | `a8b749312dd509083a46d235a0591ab8` | Factory Binary Firmware Dump |
| `0280-000-937.BIN` | **1984–1993** | 32.0 KB | `77dd7926bbf4e96f4d5c84fe30ef2ff1` | Factory Binary Firmware Dump |
| `0280-000-954.BIN` | **1984–1993** | 32.0 KB | `a7ee63b62a8c27820018b85eb8a2d04e` | Factory Binary Firmware Dump |
| `0280-000-962.BIN` | **1984–1993** | 32.0 KB | `aced46ff3dd6671e65f30221fbe65bbf` | Factory Binary Firmware Dump |
| `Bensin 984 chip 1 037 358 931.bin` | **1984–1993** | 32.0 KB | `da50f84b31fd0fb26e1921d7de80f371` | Factory Binary Firmware Dump |
| `Volvo_556.xdf` | **1984–1993** | 8.6 KB | `4e93076613a1524add8e97ee10caaaf8` | TunerPro Binary Definition Map |
| `Volvo_560.xdf` | **1984–1993** | 8.4 KB | `ee23511ef143e130171b1818c6303823` | TunerPro Binary Definition Map |
| `Volvo_913.xdf` | **1984–1993** | 10.9 KB | `e34bc384fe96f4f70b75043783336d89` | TunerPro Binary Definition Map |
| `Volvo_954_LH2.4.xdf` | **1984–1993** | 10.4 KB | `eb0c61620d74a2f105ee425d31d155cf` | TunerPro Binary Definition Map |
| `Volvo_962.xdf` | **1984–1993** | 9.6 KB | `06527829d32aa08980389feb24b71577` | TunerPro Binary Definition Map |
| `Volvo_EZK_208.xdf` | **1984–1993** | 12.7 KB | `3dd816f0a5e72a52ca64f10979c76c48` | TunerPro Binary Definition Map |
| `Volvo_LH22_511.xdf` | **1984–1993** | 4.0 KB | `bd27658f8d7bc79f7f5a5ad238c109a0` | TunerPro Binary Definition Map |
| `Volvo_LH22_554.xdf` | **1984–1993** | 5.2 KB | `66136499f03c8a884b3954ad9a749513` | TunerPro Binary Definition Map |
| `Volvo_LH24_937.xdf` | **1984–1993** | 9.0 KB | `9a4b7d1894974fd9c6bf081774eb13ec` | TunerPro Binary Definition Map |
| `lh2.2 NA 511.BIN` | **1984–1993** | 4.0 KB | `c78d51ee419ab6fa10719d12a93f5265` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
