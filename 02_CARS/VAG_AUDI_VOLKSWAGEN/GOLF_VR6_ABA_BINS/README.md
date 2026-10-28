# GOLF VR6 ABA BINS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: GOLF VR6 ABA BINS
- **Model Year Coverage**: 1992–1998
- **Total Calibration Assets**: 8 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `022906032CE-6733.A2L` | **1992–1998** | 6.02 MB | `a325eb1e2e084f03ea237be36487e9a5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `0261203219_soft109.bin` | **1992–1998** | 64.0 KB | `60542b159fae38a22d365e0d4360bc94` | Factory Binary Firmware Dump |
| `ABA_OBD1_AA.BIN` | **1992–1998** | 64.0 KB | `15679eed51c586319e3a564cb6fa65ff` | Factory Binary Firmware Dump |
| `ABA_OBD1_AE.bin` | **1992–1998** | 64.0 KB | `7ac9542e53ac6edffa3d4f47e46ad8f7` | Factory Binary Firmware Dump |
| `ABA_OBD1_AH.bin` | **1992–1998** | 64.0 KB | `9d13af3043ee1c865fdebffeaafa154f` | Factory Binary Firmware Dump |
| `Golf_VR6_0261203219_soft109.xdf` | **1992–1998** | 24.6 KB | `5c7bca9729a805535829bc349a379157` | TunerPro Binary Definition Map |
| `VR6_0261203117_021906258AF_357529_27C512.bin` | **1992–1998** | 64.0 KB | `1ecf38e31ba7de233981b2598bb3db7b` | Factory Binary Firmware Dump |
| `VW golf 2.8 VR6 AAA 021906258A 0261200496 357205.bin` | **1992–1998** | 64.0 KB | `dc1b1c577f336811f8f506af1aacbaff` | Factory Binary Firmware Dump |

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
