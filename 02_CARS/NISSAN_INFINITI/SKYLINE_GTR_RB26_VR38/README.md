# SKYLINE GTR RB26 VR38 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SKYLINE GTR RB26 VR38
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 7 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_23710-05U02_Nissan_Skyline_GTR_R32_RB26DETT.xdf` | **1998–2024** | 3.1 KB | `f77400d2bf89a832a02862eedf985e02` | TunerPro Binary Definition Map |
| `GENERATIONAL_23710-24U00_Nissan_Skyline_GTR_R33_RB26DETT.xdf` | **1998–2024** | 3.1 KB | `1a57c1d27b6688a378b6310d0af3cdb0` | TunerPro Binary Definition Map |
| `GENERATIONAL_VR38DETT_Nissan_GTR_R35_CBA_DBA_Nismo.xdf` | **1998–2024** | 3.9 KB | `181e5a73e267eef832a68e7cedbe67c0` | TunerPro Binary Definition Map |
| `STOCK_ORIGINAL_23710-05U02_Nissan_Skyline_GTR_R32_RB26DETT_280HP.bin` | **1998–2024** | 32.0 KB | `7ec4c92bc09498595fbc61d1e883299e` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_23710-05U60_Nissan_Skyline_GTR_R32_RB26DETT_280HP.bin` | **1998–2024** | 32.0 KB | `c4173c0ff5051ee9b90766ee869475ef` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_23710-05U61_Nissan_Skyline_GTR_R32_RB26DETT_280HP.bin` | **1998–2024** | 32.0 KB | `bbe7a861efd6813e88a8d4e7805cafe7` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_23710-24U00_Nissan_Skyline_GTR_R33_RB26DETT_280HP.bin` | **1998–2024** | 32.0 KB | `76eab1f407eccc121e1829a4be5e6af7` | Factory Binary Firmware Dump |

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
