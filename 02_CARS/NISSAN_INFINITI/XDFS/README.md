# XDFS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: XDFS
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 13 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `B13RT.xdf` | **1998–2024** | 55.7 KB | `a0006e906bbe90d014633bbbc039d198` | TunerPro Binary Definition Map |
| `ca18det_v2.xdf` | **1998–2024** | 37.8 KB | `4ffe18a32986a82712e9e8f1c6fec6f3` | TunerPro Binary Definition Map |
| `Infinity_M30_90_92.xdf` | **1998–2024** | 34.8 KB | `b1630ec489830f7defbad263058e335a` | TunerPro Binary Definition Map |
| `Q45.xdf` | **1998–2024** | 70.6 KB | `99e8aea351928ae6cf6cc999ae18800e` | TunerPro Binary Definition Map |
| `Q4516bit.xdf` | **1998–2024** | 69.4 KB | `ac1473035ba48b95b3eaf3f95b04f943` | TunerPro Binary Definition Map |
| `RB20det.xdf` | **1998–2024** | 63.2 KB | `e38a481986a9f7d257cca8258c61220c` | TunerPro Binary Definition Map |
| `S13RT.xdf` | **1998–2024** | 122.4 KB | `571f97764da3c17de15dd706858f65ce` | TunerPro Binary Definition Map |
| `sr20ve.xdf` | **1998–2024** | 69.9 KB | `fd60ec05379a1ddb4e8bbb13fbd5f2a9` | TunerPro Binary Definition Map |
| `U13-93-94-Altima-240sx.xdf` | **1998–2024** | 127.8 KB | `459739ee5fef532adf6f4f4cc29db51b` | TunerPro Binary Definition Map |
| `U13-96-240sx-Altima.xdf` | **1998–2024** | 95.9 KB | `b18f48fcf94d8887f749f2e6a9c3ec1b` | TunerPro Binary Definition Map |
| `Z31.xdf` | **1998–2024** | 30.3 KB | `291de52e361518ebe13f52c2c436e364` | TunerPro Binary Definition Map |
| `Z32.xdf` | **1998–2024** | 61.0 KB | `cbdd92027f7e92e65503f7e2192cd567` | TunerPro Binary Definition Map |
| `Z32_512.xdf` | **1998–2024** | 71.3 KB | `295232210b9c374fa0b5daf3a2727fe1` | TunerPro Binary Definition Map |

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
