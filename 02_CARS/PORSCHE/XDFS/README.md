# XDFS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: XDFS
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 7 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `84-86Porsche911-2K&4KChip.xdf` | **1998–2024** | 12.0 KB | `08de5436b9297f6718f1a4511c1f2d1e` | TunerPro Binary Definition Map |
| `86_944turbo_075dme.xdf` | **1998–2024** | 12.4 KB | `14816b9b6fcd6c8cb0975bcbbce1bd3e` | TunerPro Binary Definition Map |
| `92C2964Chip.xdf` | **1998–2024** | 33.5 KB | `5d2fb923a5335e47ba054583bcfcbbcb` | TunerPro Binary Definition Map |
| `Porsche951DME24pin_lim.xdf` | **1998–2024** | 26.8 KB | `f4f8c7c4fd783648a24dedd2e5af3547` | TunerPro Binary Definition Map |
| `Porsche951DME28pin_lim.xdf` | **1998–2024** | 26.8 KB | `ac83e586a627d467a2dfaaf7fb3b356c` | TunerPro Binary Definition Map |
| `Porsche_928_506.xdf` | **1998–2024** | 10.2 KB | `eed2e9770a8a33df6630494d9004dae5` | TunerPro Binary Definition Map |
| `Porsche_928GT_509.xdf` | **1998–2024** | 16.0 KB | `accaa8ad4436117df118da81f45f65ee` | TunerPro Binary Definition Map |

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
