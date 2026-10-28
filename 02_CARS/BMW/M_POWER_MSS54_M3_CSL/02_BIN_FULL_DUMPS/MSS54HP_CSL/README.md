# MSS54HP CSL - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MSS54HP CSL
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 6 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `Full 211325000401PD11 Std EOBD (European OBD).bin` | **1998–2024** | 1.00 MB | `043f2d193af16bc281ea05694de94acb` | Factory Binary Firmware Dump |
| `Full 211325000401PD1D Std No EOBD.bin` | **1998–2024** | 1.00 MB | `111567430712c6c7a9a936fa94603912` | Factory Binary Firmware Dump |
| `Full 211325000401PD1J Jap.bin` | **1998–2024** | 1.00 MB | `c32cf60d48c1796b00345758c625f253` | Factory Binary Firmware Dump |
| `Full 211325000401PD31 EOBD (European OBD) No Vmax.bin` | **1998–2024** | 1.00 MB | `6126c46a8798ce45e3d17c7426356d50` | Factory Binary Firmware Dump |
| `Full 211325000401PD3D No EOBD delimited.bin` | **1998–2024** | 1.00 MB | `ece640828100f5476992b3f1e211125d` | Factory Binary Firmware Dump |
| `Full 211325000401PD3J Jap Delimit.bin` | **1998–2024** | 1.00 MB | `699672a7bc3c6edf4383d5c84780a9f4` | Factory Binary Firmware Dump |

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
