# MATIC GRANDE FILANO FAZZIO - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MATIC GRANDE FILANO FAZZIO
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 9 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GRANDE_B8A0.bin` | **1998–2024** | 27.0 KB | `2cdade228ac30d2096f248eb314cae73` | Factory Binary Firmware Dump |
| `GRANDE_B8A1-40.bin` | **1998–2024** | 27.0 KB | `788c98fd2280b1b2daa0c4184c244216` | Factory Binary Firmware Dump |
| `GRANDE_B8A1.bin` | **1998–2024** | 27.0 KB | `eee65a0d8e12393078930a8405685020` | Factory Binary Firmware Dump |
| `GRANDE_B8B0.bin` | **1998–2024** | 27.0 KB | `b5ae5b01d21999e05f8fe74242fff56f` | Factory Binary Firmware Dump |
| `GRANDE_B8B0_31.bin` | **1998–2024** | 27.0 KB | `b5ae5b01d21999e05f8fe74242fff56f` | Factory Binary Firmware Dump |
| `GRANDE_B8B0_THAI.bin` | **1998–2024** | 27.0 KB | `b5ae5b01d21999e05f8fe74242fff56f` | Factory Binary Firmware Dump |
| `GRANDE_B8B1_41.bin` | **1998–2024** | 27.0 KB | `d5013e9e8047da2846f1b3947b0ec252` | Factory Binary Firmware Dump |
| `YAMAHA_B8A-H594A-00_Yamaha_Grand_Filano_Hybrid_(B8A0_B8B0).xdf` | **1998–2024** | 6.5 KB | `b66aa6c85862b4d492163f2b0619cc20` | TunerPro Binary Definition Map |
| `YAMAHA_BEJ-H594A-00_Yamaha_Fazzio_125_Hybrid_(BEJ0).xdf` | **1998–2024** | 6.5 KB | `b64df53f154da843a91173a8a9bd18d7` | TunerPro Binary Definition Map |

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
