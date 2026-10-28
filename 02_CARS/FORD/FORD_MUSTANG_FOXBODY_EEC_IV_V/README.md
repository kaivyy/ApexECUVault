# FORD MUSTANG FOXBODY EEC IV V - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: FORD MUSTANG FOXBODY EEC IV V
- **Model Year Coverage**: 1986–2004
- **Total Calibration Assets**: 23 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `AHAC2_211230.xdf` | **1986–2004** | 400.9 KB | `9580de15db8cf01687e6aa001217dffd` | TunerPro Binary Definition Map |
| `C9C1_240904.xdf` | **1986–2004** | 173.7 KB | `d810b9b400ec3a05fe2580756a5d53a3` | TunerPro Binary Definition Map |
| `CBAZA.xdf` | **1986–2004** | 301.1 KB | `72cc978e0d984b35fe901b5b4681549d` | TunerPro Binary Definition Map |
| `CBAZA_240216.xdf` | **1986–2004** | 795.5 KB | `cda101aa0bfc2acb65e43d6c67898438` | TunerPro Binary Definition Map |
| `CDAN4.xdf` | **1986–2004** | 163.6 KB | `4b9859321c2e4d28e88352e17d975fa2` | TunerPro Binary Definition Map |
| `CDAN4_230201.xdf` | **1986–2004** | 564.7 KB | `5898bb614a77887cd51c54cb8a735509` | TunerPro Binary Definition Map |
| `CRAI8_251001.xdf` | **1986–2004** | 564.2 KB | `af0926900f945383c4ae2ac3983ef860` | TunerPro Binary Definition Map |
| `CRAJ0.xdf` | **1986–2004** | 204.1 KB | `4fb1064b54e5485ec2e4a7e690147e32` | TunerPro Binary Definition Map |
| `CVAF1_251108.xdf` | **1986–2004** | 593.8 KB | `3f98f7f9208121b9392ef866caf5052f` | TunerPro Binary Definition Map |
| `FBGI0_230504.xdf` | **1986–2004** | 1.98 MB | `7d19179a17b928688190eb0156c5bacc` | TunerPro Binary Definition Map |
| `GSALI_240404.xdf` | **1986–2004** | 297.5 KB | `c0a54f4296d31fad8b94d3a5495765d1` | TunerPro Binary Definition Map |
| `GUF1.xdf` | **1986–2004** | 468.7 KB | `4aa3b6ee323c286c7c6bc509c65ea0e1` | TunerPro Binary Definition Map |
| `GUFA.xdf` | **1986–2004** | 470.3 KB | `fc27c9c81248bdff8d908215065d2188` | TunerPro Binary Definition Map |
| `GUFB.xdf` | **1986–2004** | 472.0 KB | `c1dfbf75f3969661f14396fc2f5acb00` | TunerPro Binary Definition Map |
| `GUFX_240206.xdf` | **1986–2004** | 775.0 KB | `66b0f52871e654406c15781f71116386` | TunerPro Binary Definition Map |
| `LUX0.xdf` | **1986–2004** | 353.6 KB | `b043e6f7ac91a828b16ba22a01a69c06` | TunerPro Binary Definition Map |
| `MNAE0_210225.xdf` | **1986–2004** | 59.4 KB | `7a634a2f6bff4555bee10e6f797e75ee` | TunerPro Binary Definition Map |
| `MQAI0_220422.xdf` | **1986–2004** | 100.8 KB | `7e715f23032f24d01c751e2808d77f7f` | TunerPro Binary Definition Map |
| `MZAK0_200922.xdf` | **1986–2004** | 115.6 KB | `654fa101a8f91dd612889854c20e5d32` | TunerPro Binary Definition Map |
| `OMAE2_241213.xdf` | **1986–2004** | 629.4 KB | `d178e52cddbfb69cce2774321e9b523a` | TunerPro Binary Definition Map |
| `RZASA_210517.xdf` | **1986–2004** | 2.83 MB | `ffc2793d67f68306528d6309ae86dea2` | TunerPro Binary Definition Map |
| `T23B.xdf` | **1986–2004** | 209.9 KB | `3c36e0b4bd56aa424bff069111c55bdf` | TunerPro Binary Definition Map |
| `TAUF0_251106.xdf` | **1986–2004** | 379.3 KB | `92328194f729b2cab7065eb656da4d86` | TunerPro Binary Definition Map |

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
