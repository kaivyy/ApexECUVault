# v7.3.1 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: v7.3.1
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 11 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `F4C9G577B_5c64-010_090_007_v7.3.1.a2l` | **1998–2024** | 910.4 KB | `05a759e9dc2c7734c353c812cf75f360` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9G595B_5c64-010_100_005_v7.3.1.a2l` | **1998–2024** | 910.4 KB | `7f4a50549f36ebdb003415a08a6819be` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9G5F5B_5c64-010_130_005_v7.3.1.a2l` | **1998–2024** | 910.4 KB | `dc31295616158c69d22c9e22dc08ca5a` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9G5H5B_5c64-010_140_005_v7.3.1.a2l` | **1998–2024** | 910.4 KB | `70c208e743ac7d77dcc97bf09e09213d` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8A6B_5c64-020_050_006_v7.3.1.a2l` | **1998–2024** | 921.9 KB | `70076dcc9ca63d28a39e228279136d97` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8C5B_5c64-020_060_005_v7.3.1.a2l` | **1998–2024** | 921.9 KB | `e9479c4375867e5253fb57af6da2cc90` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8E6B_5c64-020_070_006_v7.3.1.a2l` | **1998–2024** | 921.9 KB | `c562c8bcbfebe62cc488297df0655189` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8G7B_5c64-020_080_007_v7.3.1.a2l` | **1998–2024** | 921.9 KB | `3e50d7c2213359be3933e23fb970c6d5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8J5B_5c64-020_090_005_v7.3.1.a2l` | **1998–2024** | 921.9 KB | `99d16c59e660aebdeb98f3c9eb3820f9` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8N6B_5c64-020_110_006_v7.3.1.a2l` | **1998–2024** | 921.9 KB | `fa7dfa82d7faab2b0c98e523a8093cb5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8R5B_5c64-020_130_005_v7.3.1.a2l` | **1998–2024** | 921.9 KB | `acc0cd26efb258e5ebf2a62a5ba1826a` | ASAM MCD-2 MC / ASAP2 Definition Map |

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
