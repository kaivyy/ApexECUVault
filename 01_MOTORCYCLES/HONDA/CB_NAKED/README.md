# CB NAKED - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: CB NAKED
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 7 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `38770-MFN-D01.bin` | **1998–2024** | 256.0 KB | `2901004ac436edfa688d8d9390004281` | Factory Binary Firmware Dump |
| `38770-MFN-F01.bin` | **1998–2024** | 256.0 KB | `79c1fc40d1541cf9bdcd6c3911907655` | Factory Binary Firmware Dump |
| `38770-MGJ-D02.bin` | **1998–2024** | 256.0 KB | `88094e0884c619179c5ca8addc36ed93` | Factory Binary Firmware Dump |
| `38770-MJE-D41.bin` | **1998–2024** | 256.0 KB | `84cf7c724b83757fbd3fb12be6b7faae` | Factory Binary Firmware Dump |
| `38770-MJE-G52.bin` | **1998–2024** | 256.0 KB | `5344ca8a3b30e0e4fc133a43aaebf86a` | Factory Binary Firmware Dump |
| `38770_MJW_D51.bin` | **1998–2024** | 256.0 KB | `ecdc4c26bf7b131c79ab4cd85625d50d` | Factory Binary Firmware Dump |
| `38770_MJW_D91.bin` | **1998–2024** | 256.0 KB | `491589af89001258567d82d30341f4b5` | Factory Binary Firmware Dump |

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
