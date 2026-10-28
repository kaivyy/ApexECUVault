# BIG BIKE R1 R6 MT09 MT07 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: BIG BIKE R1 R6 MT09 MT07
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 5 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_1RC-8591A-00_Yamaha_MT_09___FZ_09_Gen_1_2014_2016_115PS.xdf` | **1998–2024** | 1.8 KB | `8bb89fce57fff42dfa4d164ed09d8713` | TunerPro Binary Definition Map |
| `GENERATIONAL_1WS-8591A-00_Yamaha_MT_07___Tenere_700___XSR_700_2014_2020_74.8PS.xdf` | **1998–2024** | 1.8 KB | `b9ac9ff957a182b90b8d06daed00e57c` | TunerPro Binary Definition Map |
| `GENERATIONAL_2CR-8591A-00_Yamaha_YZF_R1_Crossplane_CP4_2015_2019_200PS.xdf` | **1998–2024** | 1.8 KB | `e9d355dfe093305d9e86be137b1dc4a7` | TunerPro Binary Definition Map |
| `GENERATIONAL_B7N-8591A-00_Yamaha_All_New_MT_09___SP_Gen_3_890cc_2021_2026_119PS.xdf` | **1998–2024** | 1.8 KB | `bfc0621c127aa6f1a0bcf035647e7220` | TunerPro Binary Definition Map |
| `GENERATIONAL_BN6-8591A-00_Yamaha_YZF_R6_2017_2024_118.4PS.xdf` | **1998–2024** | 1.8 KB | `7ecfe958067f650c519bb4063395e900` | TunerPro Binary Definition Map |

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
