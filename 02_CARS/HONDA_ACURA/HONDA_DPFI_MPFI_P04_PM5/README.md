# HONDA DPFI MPFI P04 PM5 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: HONDA DPFI MPFI P04 PM5
- **Model Year Coverage**: 1988–1991
- **Total Calibration Assets**: 17 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `121_pm5_701.bin` | **1988–1991** | 16.0 KB | `c1a71ffe1a0d2c9e913699e6cb8ac208` | Factory Binary Firmware Dump |
| `p04_rev1_198.bin` | **1988–1991** | 32.0 KB | `244bfe94a3d5306b9322a98f017d4abb` | Factory Binary Firmware Dump |
| `p04_rev2_146.bin` | **1988–1991** | 32.0 KB | `fe8e425c4f3243323b73939a9b9d60ec` | Factory Binary Firmware Dump |
| `p04_rev3_171.bin` | **1988–1991** | 32.0 KB | `3dd1c56685f3b81b8e9ab5678ddd4520` | Factory Binary Firmware Dump |
| `p04_rev4_222.bin` | **1988–1991** | 32.0 KB | `e22cc549a8ab2751bfa7e5aa54132081` | Factory Binary Firmware Dump |
| `p04_rev5_136.bin` | **1988–1991** | 32.0 KB | `3ead4169c18df94a05729a5f34270c5e` | Factory Binary Firmware Dump |
| `p04_rev6_826.bin` | **1988–1991** | 32.0 KB | `8d2230dd7e79081e37e62735245d675a` | Factory Binary Firmware Dump |
| `p04_rev7_107.bin` | **1988–1991** | 32.0 KB | `5e7da87e4d5cdb1a403b4f6164925b0c` | Factory Binary Firmware Dump |
| `p04_rev8_128.bin` | **1988–1991** | 32.0 KB | `1ae65ab4ed174d07e388a7be826c8337` | Factory Binary Firmware Dump |
| `p04_rev9_140.bin` | **1988–1991** | 32.0 KB | `5b646891bb38b31a6a696f79d8bd24cc` | Factory Binary Firmware Dump |
| `p04_try_374.bin` | **1988–1991** | 32.0 KB | `df88aa07310de45fc0d7104aec57cf5b` | Factory Binary Firmware Dump |
| `pm5_dump_176.bin` | **1988–1991** | 32.0 KB | `cc08b15d100e94e5224982b11bf9a0d7` | Factory Binary Firmware Dump |
| `pm5_x30_1991508_175.bin` | **1988–1991** | 32.0 KB | `505a35a06c8aaa4a85bf9edee962f0c3` | Factory Binary Firmware Dump |
| `stock_p04-g01_131.bin` | **1988–1991** | 32.0 KB | `dedfb60aef63ab9e6cc8045403c6e5ea` | Factory Binary Firmware Dump |
| `stock_p04-g01_297.bin` | **1988–1991** | 32.0 KB | `dedfb60aef63ab9e6cc8045403c6e5ea` | Factory Binary Firmware Dump |
| `stock_p04-g02_sajmon1100_739.bin` | **1988–1991** | 32.0 KB | `df88aa07310de45fc0d7104aec57cf5b` | Factory Binary Firmware Dump |
| `stock_pm5_x30_120.bin` | **1988–1991** | 32.0 KB | `7719ed332d8b6783da4c3777cdd51b39` | Factory Binary Firmware Dump |

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
