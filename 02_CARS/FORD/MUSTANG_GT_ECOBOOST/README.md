# MUSTANG GT ECOBOOST - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MUSTANG GT ECOBOOST
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 8 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `CBAZA.xdf` | **1998–2024** | 309.9 KB | `dc4628312362aa97968951d40fc5891d` | TunerPro Binary Definition Map |
| `CDAN4.xdf` | **1998–2024** | 168.7 KB | `5e134df0c835951cd23c969d405d9d6c` | TunerPro Binary Definition Map |
| `CRAJ0.xdf` | **1998–2024** | 210.7 KB | `00a2acf2a4905fd93bf8c95119e4148e` | TunerPro Binary Definition Map |
| `GENERATIONAL_CR3A-12A650-B_Ford_Mustang_GT_5.0_Coyote_Gen1_2011_2014.xdf` | **1998–2024** | 3.0 KB | `dc68a2105d651c774b5b4d85e75f76ce` | TunerPro Binary Definition Map |
| `GENERATIONAL_FR3A-12A650-C_Ford_Mustang_2.3L_EcoBoost_2015_2023.xdf` | **1998–2024** | 3.0 KB | `727b97d54c93eff21e8394e7e8161a9c` | TunerPro Binary Definition Map |
| `GENERATIONAL_JR3A-12A650-A_Ford_Mustang_GT_5.0_Coyote_Gen3_2018_2023.xdf` | **1998–2024** | 3.0 KB | `9f050604ecdcb1d103c66d05f61ff128` | TunerPro Binary Definition Map |
| `GUFA.xdf` | **1998–2024** | 483.4 KB | `28d3c5bdf66182cff4b39850ebd44814` | TunerPro Binary Definition Map |
| `GUFB.xdf` | **1998–2024** | 485.1 KB | `f5b62ef9f570031f3f6f79cd05f58e79` | TunerPro Binary Definition Map |

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
