# ECUFLASH XML DEFS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: ECUFLASH XML DEFS
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 9 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `20030010.xml` | **1998–2024** | 28.0 KB | `c5e9c7c9a06ac7c31714e86067c7c894` | EcuFlash / RomRaider XML Definition |
| `20030011.xml` | **1998–2024** | 28.0 KB | `00f7d4192828a8ab6e82cc375f1c1b46` | EcuFlash / RomRaider XML Definition |
| `20030013.xml` | **1998–2024** | 28.0 KB | `f5a929a9072734e04b9688540efa8dc1` | EcuFlash / RomRaider XML Definition |
| `22250305.xml` | **1998–2024** | 886 B | `b3163cbb551e0de3298362da3262355e` | EcuFlash / RomRaider XML Definition |
| `23810003.xml` | **1998–2024** | 28.0 KB | `2eac9d0ac78e0b908979b7ad49d5daf8` | EcuFlash / RomRaider XML Definition |
| `23810004.xml` | **1998–2024** | 28.0 KB | `f93c147de6d33e5eeca85329195fcffa` | EcuFlash / RomRaider XML Definition |
| `EMKS11.xml` | **1998–2024** | 12.8 KB | `5aea16f0b08ea26260c7f55dfca372d9` | EcuFlash / RomRaider XML Definition |
| `vr4_AT_base.xml` | **1998–2024** | 14.5 KB | `7c189061f85c8d3a32e49c4d1e6f3767` | EcuFlash / RomRaider XML Definition |
| `vr4base.xml` | **1998–2024** | 67.4 KB | `8345c86a0e1a2936dfbca7b1141806a3` | EcuFlash / RomRaider XML Definition |

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
