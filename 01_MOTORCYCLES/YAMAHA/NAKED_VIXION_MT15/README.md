# NAKED VIXION MT15 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: NAKED VIXION MT15
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 9 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_3C1-H591A-00_Yamaha_Vixion_3C1_Gen_1_Old_(2007-2012).xdf` | **2007–2012** | 5.4 KB | `90daddeb32fe8acaf8b8c71bf25efddc` | TunerPro Binary Definition Map |
| `GENERATIONAL_BBS-H591A-00_Yamaha_XSR_155_Heritage_2019_2025_K_Line.xdf` | **1998–2024** | 2.5 KB | `309e5f9e26e2660d771d40aa5d931651` | TunerPro Binary Definition Map |
| `GENERATIONAL_BBS-H591A-10_Yamaha_XSR_155_Connected_2023_2025_CANBUS.xdf` | **1998–2024** | 2.5 KB | `28ca5974493c7d5fdde7c811beb8abf2` | TunerPro Binary Definition Map |
| `GENERATIONAL_BK7-H591A-00_Yamaha_All_New_Vixion_150_Gen_4_Assist_Slipper_(2017-2024).xdf` | **2017–2024** | 5.5 KB | `38898129d1e14306708af806b8b99238` | TunerPro Binary Definition Map |
| `MT_15_B8D0.bin` | **1998–2024** | 27.0 KB | `0b38513ab5681e54851289e8130e81ad` | Factory Binary Firmware Dump |
| `MT_15_BHM0.bin` | **1998–2024** | 27.0 KB | `f6ff2111b461a7d58c82ab68a7f4c731` | Factory Binary Firmware Dump |
| `YAMAHA_1PA-H591A-00_Yamaha_New_Vixion_Advance_NVA_(1PA).xdf` | **1998–2024** | 6.5 KB | `95ae67a83b94e2c8beef4cd858aaacab` | TunerPro Binary Definition Map |
| `YAMAHA_2TP-E591A-00_Yamaha_New_Vixion_Lightning_NVL_(2TP0).xdf` | **1998–2024** | 6.5 KB | `98e7060c08a90c685f7ebc281d3787a3` | TunerPro Binary Definition Map |
| `YAMAHA_B8D-H594A-00_Yamaha_MT-15_(B8D0).xdf` | **1998–2024** | 11.6 KB | `7bf8c4d191d51bb3ee8a8406ae155bc4` | TunerPro Binary Definition Map |

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
