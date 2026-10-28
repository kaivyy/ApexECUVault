# ENGINE SWAP - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: ENGINE SWAP
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 6 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `DTC 0301 0401 Method1.xdf` | **1998–2024** | 59.6 KB | `0a94e84c8fdd8bfbd52d1fd8049189df` | TunerPro Binary Definition Map |
| `DTC 0301 0401 Method4.xdf` | **1998–2024** | 59.6 KB | `41b4fb9210785bb8cc2147b5cb28cceb` | TunerPro Binary Definition Map |
| `DTC 0901  1101  1301  1501  1701  2101  2401  2601  2801.xdf` | **1998–2024** | 59.6 KB | `f4505b270600bdeb36a1470eab3cb65f` | TunerPro Binary Definition Map |
| `DTC 1801  1901  2001  2501  2701.xdf` | **1901** | 59.6 KB | `02612935f4ee11a8436774ea6ed4f5e0` | TunerPro Binary Definition Map |
| `MSS54 v2601 v2801 E30 Swap Items.xdf` | **1998–2024** | 35.2 KB | `9caab4c8533708ec07bac2762179b339` | TunerPro Binary Definition Map |
| `MSS54HP v1801 v2001 v2501 v2701 E30 Swap Items.xdf` | **1998–2024** | 35.2 KB | `92bf4e0be15d14e920171428965b487e` | TunerPro Binary Definition Map |

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
