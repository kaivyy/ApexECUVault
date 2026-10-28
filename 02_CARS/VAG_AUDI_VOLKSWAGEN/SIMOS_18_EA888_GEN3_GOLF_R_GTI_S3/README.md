# SIMOS 18 EA888 GEN3 GOLF R GTI S3 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SIMOS 18 EA888 GEN3 GOLF R GTI S3
- **Model Year Coverage**: 2013–2020
- **Total Calibration Assets**: 10 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `8v0906264L.xdf` | **2013–2020** | 199.1 KB | `e86edb2c8f5a659ff71ba17edc9c39b2` | TunerPro Binary Definition Map |
| `8v0906264L__simos-definitions.xdf` | **2013–2020** | 204.1 KB | `d6cec807c0b03b990617d79e37b5b2c0` | TunerPro Binary Definition Map |
| `SC8H64_5G0906259A_0006.xdf` | **2013–2020** | 28.2 KB | `e26655accd094a992157e577bcacc36b` | TunerPro Binary Definition Map |
| `SC8H80_5G0906259D_0002.xdf` | **2013–2020** | 102.0 KB | `1abc61c0c03fe60ea3da0fcf7b8c8908` | TunerPro Binary Definition Map |
| `SC8S30_8v0906264L.xdf` | **2013–2020** | 306.0 KB | `fe8f40f53f4365a3d181533adb1bac0a` | TunerPro Binary Definition Map |
| `SC8S30_8v0906264L__simos-definitions.xdf` | **2013–2020** | 313.9 KB | `ec3097ce509daf1bb4b68ab5fc808083` | TunerPro Binary Definition Map |
| `SC8S50_8V0906259K.xdf` | **2013–2020** | 204.0 KB | `b8c164fce99435acc4d665340252271d` | TunerPro Binary Definition Map |
| `SC8S50_8V0906259K__simos-definitions.xdf` | **2013–2020** | 209.3 KB | `6601fb6a2526e9181c2a610931043660` | TunerPro Binary Definition Map |
| `SC8S50_openflex_simplewgdc.xdf` | **2013–2020** | 345.0 KB | `7f42e977a2a87cf274e1af6cf1f8f110` | TunerPro Binary Definition Map |
| `SC8S50_openflex_simplewgdc__simos-definitions.xdf` | **2013–2020** | 353.9 KB | `f2f2e31f560786f0dce9901671baa033` | TunerPro Binary Definition Map |

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
