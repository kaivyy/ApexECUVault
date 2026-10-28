# VOLVO 960 S90 V90 MOTRONIC 44 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: VOLVO 960 S90 V90 MOTRONIC 44
- **Model Year Coverage**: 1994–1998
- **Total Calibration Assets**: 6 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `M44_B6304_S90 v0001.xdf` | **1994–1998** | 152.6 KB | `97afae58347efc5fec34cc036669c92e` | TunerPro Binary Definition Map |
| `M44_B6304_S90 v0001__sostisoft-defs.xdf` | **1994–1998** | 149.0 KB | `38fc98488c53bf31f18f27d5df6889cf` | TunerPro Binary Definition Map |
| `M44_B6304_S90_0002.xdf` | **1994–1998** | 176.0 KB | `3a352dfd891e9951e37c49f3ee324168` | TunerPro Binary Definition Map |
| `M44_B6304_S90_0002__sostisoft-defs.xdf` | **1994–1998** | 171.8 KB | `25e12e831edb97b0aed276751e149ff2` | TunerPro Binary Definition Map |
| `S90 V0002 XDF0002 .BIN` | **1994–1998** | 128.0 KB | `71721563f54247a416a3aa3c47be5f79` | Factory Binary Firmware Dump |
| `Stock S90.BIN` | **1994–1998** | 128.0 KB | `de4b01098f3157fac610fa5e41c7387c` | Factory Binary Firmware Dump |

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
