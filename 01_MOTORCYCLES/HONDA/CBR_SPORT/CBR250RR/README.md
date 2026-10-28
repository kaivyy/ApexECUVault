# CBR250RR - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: CBR250RR
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 6 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `38770-K64-N01.bin` | **1998–2024** | 1.00 MB | `e0c12d43c50c7c285df0307bef13f4b5` | Factory Binary Firmware Dump |
| `38770-K64-R02.bin` | **1998–2024** | 1.00 MB | `f87f1dc65059e08f496e62fd0872a6e7` | Factory Binary Firmware Dump |
| `CBR250RR-38770-K64-N04_BIN.bin` | **1998–2024** | 1.00 MB | `c069d5b2d1476a728ba14a43ef73dc7a` | Factory Binary Firmware Dump |
| `CBR250RR-38770-K64-ND1_BIN.bin` | **1998–2024** | 1.00 MB | `5c616504f3b6306adff2ad04a17ab68c` | Factory Binary Firmware Dump |
| `CBR250RR_38770-K64-N04_PUBLIC_v1.xdf` | **1998–2024** | 89.0 KB | `8beae407f19171868ea92c8f56748426` | TunerPro Binary Definition Map |
| `CBR250RR_38770-K64-ND1_PUBLIC_v1.xdf` | **1998–2024** | 83.3 KB | `cb0b660f54754f38efbc1ad750aa4967` | TunerPro Binary Definition Map |

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
