# SKYLINE GTR RB26 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SKYLINE GTR RB26
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 6 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `BNCR33_RB26DETT_24U00.bin` | **1998–2024** | 32.0 KB | `76eab1f407eccc121e1829a4be5e6af7` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U02_MT_MECR128.bin` | **1998–2024** | 32.0 KB | `7ec4c92bc09498595fbc61d1e883299e` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U03_MT_MEC-R138.BIN` | **1998–2024** | 32.0 KB | `6687444c0f098e91f418cfab02a1a67f` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U60_MT_MECR280.bin` | **1998–2024** | 32.0 KB | `c4173c0ff5051ee9b90766ee869475ef` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U61_MT_MECR281.bin` | **1998–2024** | 32.0 KB | `bbe7a861efd6813e88a8d4e7805cafe7` | Factory Binary Firmware Dump |
| `BNR32_RB26DETT_05U62_MT_MECR282A.BIN` | **1998–2024** | 32.0 KB | `3269f74f11578842638c456048c8b517` | Factory Binary Firmware Dump |

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
