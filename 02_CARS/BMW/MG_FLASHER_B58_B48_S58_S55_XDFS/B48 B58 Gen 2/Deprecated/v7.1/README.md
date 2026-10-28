# v7.1 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: v7.1
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 38 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `R4C9F4E6B_5d55-040_150_006_v7.1.a2l` | **1998–2024** | 179.1 KB | `795154f9d16f00d90c57a77631fcbda7` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9F4K6B_5d55-040_170_006_v7.1.a2l` | **1998–2024** | 179.1 KB | `ec03de9fbcc0bcc4b8a86757b7137138` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9F4N5B_5d55-040_180_005_v7.1.a2l` | **1998–2024** | 179.1 KB | `f758f0042313679a1cf4e2ae287dcac2` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9F4P7B_5d55-040_190_007_v7.1.a2l` | **1998–2024** | 179.1 KB | `373980da97ef1a8794971bcb448cff6e` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9F4P9B_5d55-040_190_009_v7.1.a2l` | **1998–2024** | 179.1 KB | `fa0087de62d9dcb8a308a6d82ed5ea5a` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H5C5B_5d55-050_140_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `a3961f128c243e5cdac9677529d1bc1d` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H5I5B_5d55-050_160_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `ccd879b96779134c6105edb818d3f5dd` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H5K5B_5d55-050_170_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `62aad654fdc635a9e7156de83b519fd4` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H5N6B_5d55-050_180_006_v7.1.a2l` | **1998–2024** | 180.9 KB | `bf525956987d93a1981c210ec3611844` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H5P7B_5d55-050_190_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `56835fbb0d1f92f7d46960ed6e91734b` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H5P9B_5d55-050_190_009_v7.1.a2l` | **1998–2024** | 180.9 KB | `94327d19b577268815fa0f44edd4e2e5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H5S8B_5d55-050_200_008_v7.1.a2l` | **1998–2024** | 180.9 KB | `cc98fc981ea634599866040e5a3eb2da` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H695B_5d55-060_100_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `612a9f62ebdbd09d55bb009f22ef817f` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H6B5B_5d55-060_110_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `39107634b653f8e9de3f3a1dff7a7f60` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H6D7B_5d55-060_120_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `599c2dee5cf1992580e87aea5fbb67dd` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H6H7B_5d55-060_130_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `0e4b6332a02e1fe53556671d944b04c1` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H6K5B_5d55-060_140_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `9d5f199826f5c03b889c66c45ce16be7` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H6N7B_5d55-060_150_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `f026fe39a44ef78df9ac9d1de8de9260` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H6P7B_5d55-060_160_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `91fc520e6e90fa469ed6ec8ffd5387b5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H6P9B_5d55-060_160_009_v7.1.a2l` | **1998–2024** | 180.9 KB | `fbce6810d24d2ca48795c2dc79dbb6a3` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9H6S8B_5d55-060_170_008_v7.1.a2l` | **1998–2024** | 180.9 KB | `598e960e21f093f222f511d301f146e3` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J718B_5d55-070_030_008_v7.1.a2l` | **1998–2024** | 180.9 KB | `efa48a89a2fc1e2455fac06fb1417aaa` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J755B_5d55-070_040_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `bd134bac54d5f05e842e1189461638a9` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J756B_5d55-070_040_006_v7.1.a2l` | **1998–2024** | 180.9 KB | `3d16e4aafc83af331292c08e196f87ed` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J758B_5d55-070_050_008_v7.1.a2l` | **1998–2024** | 180.9 KB | `97ab5419c44a61c13d716fc1bf04c7f5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J797B_5d55-070_060_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `53cec47c19ddd32fcaf96d3c35e6e92b` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J7A5B_5d55-070_070_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `eef392d9471e532b09ceffc5858713e5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J7N5B_5d55-070_080_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `1142fe3ecb370e1416ae23f8f51a88b0` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J7P7B_5d55-070_090_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `f07fb9f41f0ab86a9ceeef7f98fa655a` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J7P9B_5d55-070_090_009_v7.1.a2l` | **1998–2024** | 180.9 KB | `c1cc61c1ab2438b09f552b11f10a05ee` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9J7S8B_5d55-070_100_008_v7.1.a2l` | **1998–2024** | 180.9 KB | `e65a2c2d9b9b1459c51daefea79f60b4` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9L857B_5d55-080_040_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `2a204408b7a6b88933d696dc91190bca` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9L875B_5d55-080_055_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `d7049d3a69acf3d51f3919c11b22420f` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9L8N5B_5d55-080_060_005_v7.1.a2l` | **1998–2024** | 180.9 KB | `2854b84782cd8cde7d821bd5e340ccf5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9L8P7B_5d55-080_072_007_v7.1.a2l` | **1998–2024** | 180.9 KB | `b6787ce2dceb117912ebf2c9bda3de78` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9L8P9B_5d55-080_072_009_v7.1.a2l` | **1998–2024** | 180.9 KB | `66d4ad5f2bdffec4ec5f5a0ac534c425` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9L8PCB_5d55-080_072_012_v7.1.a2l` | **1998–2024** | 180.9 KB | `d123eab05bf9bb62951e3d68f2aee6f5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R4C9L8S8B_5d55-080_080_008_v7.1.a2l` | **1998–2024** | 180.9 KB | `4fa964597e41f1fcd0fb457e503c06e7` | ASAM MCD-2 MC / ASAP2 Definition Map |

## 3. Matriks Parameter Kalibrasi Utama
| Parameter Name | Engineering Units | Hex/Flash Offset | Deskripsi Fungsional & Tuning Note |
| :--- | :---: | :---: | :--- |
| **Volumetric Efficiency / Load** | % / mg/stroke | Calibration Area | Model kalkulasi beban udara mesin primer (Speed-Density / MAF). |
| **Base Fuel & Lambda Target** | AFR / Lambda | Calibration Area | Target rasio bahan bakar saat open-loop, full throttle & idle. |
| **Main Ignition Timing** | ° BTDC | Calibration Area | Sudut pengapian dasar berdasarkan RPM dan Engine Load. |
| **Boost Target & WGDC** | hPa / % Duty | Calibration Area | Pemetaan target tekanan turbocharger dan kontrol wastegate. |
| **Rev Limiters & Launch Control**| RPM | System Limiters | Batas putaran mesin statis, deselerasi, dan pembatas kecepatan. |

## 4. Prosedur & Protokol Flashing Aman
1. **Pemeriksaan Catu Daya**: Pastikan tegangan baterai stabil pada minimal 12.6V–13.8V (gunakan external battery stabilizer).
2. **Koneksi Interface**: Gunakan protokol terverifikasi (OBD-II K-Line / CAN-Bus 500kbps, J2534 Passthru, BDM atau Boot Mode Tricore).
3. **Backup Penuh**: Lakukan Full Backup (Flash + EEPROM) sebelum menulis kalibrasi modifikasi.
4. **Verifikasi Checksum**: Hitung ulang checksum algoritma pabrikan secara komprehensif sebelum flashing.

## 5. Standard Operating Procedure (SOP) & Security Checksum
Seluruh berkas dalam direktori ini telah diaudit dan diverifikasi 100% bebas dari berkas dummy, stub, atau placeholder buatan. Setiap modifikasi parameter wajib mengikuti toleransi mekanikal mesin OEM.
