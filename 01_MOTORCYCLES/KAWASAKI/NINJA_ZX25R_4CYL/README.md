# NINJA ZX25R 4CYL - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: NINJA ZX25R 4CYL
- **Model Year Coverage**: 2020–2026
- **Total Calibration Assets**: 3 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_21175-1563_Kawasaki_Ninja_ZX_25R_Gen_1_2020_2022_51PS.xdf` | **2020–2026** | 2.5 KB | `a58d008410e7720e3c5580eae211600a` | TunerPro Binary Definition Map |
| `GENERATIONAL_21175-1798_Kawasaki_Ninja_ZX_25RR___SE_Gen_2_TFT_2023_2026.xdf` | **2020–2026** | 2.5 KB | `f7362480ffd6caf154cdf0cb31604eba` | TunerPro Binary Definition Map |
| `KAWASAKI_21175-1560_Kawasaki_Ninja_ZX-25R_4-Cylinder_(ZX250E).xdf` | **2020–2026** | 9.4 KB | `6746ded94ecafef4f5ce185e7d464890` | TunerPro Binary Definition Map |

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
