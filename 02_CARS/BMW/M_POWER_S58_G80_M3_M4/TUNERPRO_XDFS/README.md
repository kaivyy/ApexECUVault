# TUNERPRO XDFS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: TUNERPRO XDFS
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 12 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `00005C640A6405.xdf` | **1998–2024** | 1.69 MB | `f37f25825c1854a9c68b26dbb548b6ee` | TunerPro Binary Definition Map |
| `00005C640A8205.xdf` | **1998–2024** | 1.69 MB | `e237ffb7e6c289a103bc05da7fe6f62e` | TunerPro Binary Definition Map |
| `00005C640A8C05.xdf` | **1998–2024** | 1.69 MB | `a5465ab38095c5646f69a951e0001805` | TunerPro Binary Definition Map |
| `00005C64143206.xdf` | **1998–2024** | 1.76 MB | `4bfd87533165d6ecc9cf8eb17f3a39b3` | TunerPro Binary Definition Map |
| `00005C64143C05.xdf` | **1998–2024** | 1.76 MB | `5f799f68ce160b207cf749513c87e300` | TunerPro Binary Definition Map |
| `00005C64144606.xdf` | **1998–2024** | 1.76 MB | `3f67811e99a11dc4d686e0306a68d5cf` | TunerPro Binary Definition Map |
| `00005C64145007.xdf` | **1998–2024** | 1.76 MB | `176f147d12e9f78f92d676b2a6a88831` | TunerPro Binary Definition Map |
| `00005C64145A05.xdf` | **1998–2024** | 1.76 MB | `7725c2f599c5e973654012b11ede36b8` | TunerPro Binary Definition Map |
| `00005C64146E06.xdf` | **1998–2024** | 1.76 MB | `02683e28672df56ae1883c222f217ebb` | TunerPro Binary Definition Map |
| `00005C64148205.xdf` | **1998–2024** | 1.76 MB | `efa2ae816574669ef29bfbfc9b175e19` | TunerPro Binary Definition Map |
| `00005C64148706.xdf` | **1998–2024** | 1.76 MB | `efa2ae816574669ef29bfbfc9b175e19` | TunerPro Binary Definition Map |
| `00005C6414C808.xdf` | **1998–2024** | 1.76 MB | `06f9b298264de065581b707f7d0eb1cb` | TunerPro Binary Definition Map |

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
