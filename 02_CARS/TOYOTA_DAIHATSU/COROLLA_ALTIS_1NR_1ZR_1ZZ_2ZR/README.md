# COROLLA ALTIS 1NR 1ZR 1ZZ 2ZR Calibration Suite

## 1. Technical Overview
Koleksi biner kalibrasi pabrikan OEM dan definisi tuning untuk modul ECU platform COROLLA ALTIS 1NR 1ZR 1ZZ 2ZR.

* **Rentang Tahun / Model Year**: 2001–2019
* **Total File Terdaftar**: 13 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `89663-02023.bin` | **2001–2007** | 320.0 KB | `5ddef7c2ce9c5abbefa2cb8777628d13` | Factory Binary (Toyota Corolla 1.8 1ZZFE) |
| `89663-02161.bin` | **2001–2007** | 320.0 KB | `d1ae6fb54e61566ae61e4056154def06` | Factory Binary (Toyota Corolla 1.8 1ZZFE) |
| `89663-02162.bin` | **2001–2007** | 320.0 KB | `dcbe18885ef74606548a923362f147b5` | Factory Binary (Toyota Corolla 1.8 1ZZFE) |
| `89663-02172.bin` | **2001–2007** | 320.0 KB | `bb4c9d3fb90a71d01256df472084d983` | Factory Binary (Toyota Corolla 1.8 1ZZFE) |
| `89663-02173.bin` | **2001–2007** | 320.0 KB | `aa21e2bea3f428607d36e113fc6167dc` | Factory Binary (Toyota Corolla 1.8 1ZZFE) |
| `89663-02241.bin` | **2001–2019** | 368.0 KB | `9bc2041a3ec839cfd9c8017fd72d77ff` | Factory Binary (Toyota Corolla 1.6) |
| `89663-02270.bin` | **2001–2007** | 368.0 KB | `d1f80cabcd6dd3a2cf2be553de6f1e8e` | Factory Binary (Toyota Corolla 1.6 3ZZFE) |
| `89663-02482.bin` | **2008–2019** | 496.0 KB | `2dd339b573686fbc28c6698133ba16bf` | Factory Binary (Toyota Corolla 1.6 1ZRFE) |
| `89663-02502.bin` | **2008–2019** | 496.0 KB | `69b5ac8f844408bc29de9180f4c4e603` | Factory Binary (Toyota Corolla 1.6 1ZRFE) |
| `89663-02661.bin` | **2008–2019** | 736.0 KB | `d8cc949db374e6eea05971f1892a1efc` | Factory Binary (Toyota Corolla 1.8 2ZRFE) |
| `89663-02E73.bin` | **2013–2021** | 992.0 KB | `01c750bb362506d8026022a952303b60` | Factory Binary (Toyota Corolla 1.3 1NRFE) |
| `89663-02J13.bin` | **2002–2012** | 736.0 KB | `4206fdd3371c26cdeee436b3c26d6c24` | Factory Binary (Toyota Corolla 2.4 2AZFE) |
| `89663-02J22.bin` | **2002–2012** | 736.0 KB | `3d4a843cdf1faf04d594e6aa9f62ea05` | Factory Binary (Toyota Corolla 2.4 2AZFE) |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan sensor wideband AFR pada beban dyno.
