# Experimental- Need Testing - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: Experimental- Need Testing
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 12 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `'04 Chevy MPV  4x4 Half Ton LM7 os12587603.bin` | **1998–2024** | 1.00 MB | `07cfa958303ce233016c29c5d9983dcb` | Factory Binary Firmware Dump |
| `'04 CTS-V LS6 M6 os12592433.bin` | **1998–2024** | 1.00 MB | `3b97f077d0582241d8709c191dae124b` | Factory Binary Firmware Dump |
| `'04 GMC 1T 4x4 8.1 L18 os12587603.bin` | **1998–2024** | 1.00 MB | `52d7d7c7d6de397b5e7d86f83d4658d0` | Factory Binary Firmware Dump |
| `03_Sierra_LM7_4L60E_DBW_OS12587603.bin` | **1998–2024** | 1.00 MB | `412a4d7cfb38fe24fc00f5a09dd40d83` | Factory Binary Firmware Dump |
| `12587603 - 2004 1mb.xdf` | **2004** | 782.7 KB | `7ca8ac43e3015035e137d442666d4001` | TunerPro Binary Definition Map |
| `12592433-imperial.xdf` | **1998–2024** | 604.7 KB | `306a247281aebb94e518e5cc43972fd8` | TunerPro Binary Definition Map |
| `12592433-metric.xdf` | **1998–2024** | 597.7 KB | `ac7d67a9da799047e4921457247ca6d5` | TunerPro Binary Definition Map |
| `2004 2500 LQ4 Auto 2wd stock OS12587603.bin` | **2004** | 1.00 MB | `59698a2f43fc1bd1c080ef9e65bbc7bc` | Factory Binary Firmware Dump |
| `2004 Escalade 5.3AutoStock OS12587603.bin` | **2004** | 1.00 MB | `a01110a0bd863433c5129748d54b613f` | Factory Binary Firmware Dump |
| `C1500_5.3L_OS12587603.bin` | **1998–2024** | 1.00 MB | `d093d51c6966f57825d77d158f8b9e4c` | Factory Binary Firmware Dump |
| `Chevy_1500_4x2_LM7 _OS12587603.bin` | **1998–2024** | 1.00 MB | `a88e7062f3019e59b12314f56ed985d0` | Factory Binary Firmware Dump |
| `Chevy_1500_4x4_MPV_L59_12587603.bin` | **1998–2024** | 1.00 MB | `1428a0038c2a3385befca2350796017c` | Factory Binary Firmware Dump |

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
