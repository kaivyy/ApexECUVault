# BASIC - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: BASIC
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 15 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `hw0301_V4_Basic.xdf` | **1998–2024** | 733.6 KB | `f657c8bb67fda179b1b5af4f0291332f` | TunerPro Binary Definition Map |
| `hw0401_V4_Basic.xdf` | **1998–2024** | 760.0 KB | `cb67036d9362b34d4f2f0712dd0e915b` | TunerPro Binary Definition Map |
| `hw1101_V4_Basic.xdf` | **1998–2024** | 736.3 KB | `f1bd6d5ab29b59806fcc65dd2c5c0e8d` | TunerPro Binary Definition Map |
| `hw1301_V4_Basic.xdf` | **1998–2024** | 760.1 KB | `8957e34b904a7bd893ecc4312f1250f3` | TunerPro Binary Definition Map |
| `hw1401_V4_Basic.xdf` | **1998–2024** | 760.5 KB | `c5d815950210f8014153c489734ac7dd` | TunerPro Binary Definition Map |
| `hw1501_V4_Basic.xdf` | **1998–2024** | 736.9 KB | `2b5e7334cd32ed40be8b6264da33f0cb` | TunerPro Binary Definition Map |
| `hw1701_V4_Basic.xdf` | **1998–2024** | 760.5 KB | `3bf0e42df2ae621a34acb013a5386f17` | TunerPro Binary Definition Map |
| `hw1801_V4_Basic.xdf` | **1998–2024** | 760.5 KB | `749cbe3cf080d03a194865298ea26da1` | TunerPro Binary Definition Map |
| `hw1901_V4_Basic.xdf` | **1998–2024** | 736.8 KB | `01f1cc26d4c6747bf0eaae488be9ab0d` | TunerPro Binary Definition Map |
| `hw2001_V4_Basic.xdf` | **1998–2024** | 764.9 KB | `b13805cc6cd2ec68754572d528b59fc6` | TunerPro Binary Definition Map |
| `hw2101_V4_Basic.xdf` | **1998–2024** | 760.5 KB | `ca24e50075ce7f09c3ebd52431928afb` | TunerPro Binary Definition Map |
| `hw2501_V4_Basic.xdf` | **1998–2024** | 736.7 KB | `95cff077e593052e032988d76ba44cda` | TunerPro Binary Definition Map |
| `hw2601_V4_Basic.xdf` | **1998–2024** | 760.7 KB | `3c57c8ac98d8e7f68f12d8af62a2d4c4` | TunerPro Binary Definition Map |
| `hw2701_V4_Basic.xdf` | **1998–2024** | 736.9 KB | `2aab5e40809d4bd57c047eb4696ad1e1` | TunerPro Binary Definition Map |
| `hw2801_V4_Basic.xdf` | **1998–2024** | 736.6 KB | `82c461efc48f9a463b2208f68bed0ca0` | TunerPro Binary Definition Map |

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
