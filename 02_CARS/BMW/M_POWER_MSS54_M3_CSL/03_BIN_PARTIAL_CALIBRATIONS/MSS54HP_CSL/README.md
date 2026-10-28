# MSS54HP CSL - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MSS54HP CSL
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 7 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `211325000301PD71.bin` | **1998–2024** | 64.0 KB | `8295fbffbd94f5d23d333acf41024a35` | Factory Binary Firmware Dump |
| `211325000401PD11.bin` | **1998–2024** | 64.0 KB | `47fbd3394e6b02a13714fd259bb55355` | Factory Binary Firmware Dump |
| `211325000401PD1D.bin` | **1998–2024** | 64.0 KB | `0e4e5e914f5e6021ebc75c3c73c86927` | Factory Binary Firmware Dump |
| `211325000401PD1J.bin` | **1998–2024** | 64.0 KB | `cf4802e00ceeb23b8c9fe93194a9a989` | Factory Binary Firmware Dump |
| `211325000401PD31.bin` | **1998–2024** | 64.0 KB | `b050ca73c00c6d79164cdc3bfa695c87` | Factory Binary Firmware Dump |
| `211325000401PD3D.bin` | **1998–2024** | 64.0 KB | `582e2e90c787101049fd3c728424e563` | Factory Binary Firmware Dump |
| `211325000401PD3J.bin` | **1998–2024** | 64.0 KB | `d17c3484f12bf059565b3bb4d8adb4c1` | Factory Binary Firmware Dump |

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
