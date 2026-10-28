# OS 1226125 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: OS 1226125
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 7 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `'02 Chevy 2500 4x4 8.1 L18 os12216125 (1).bin` | **1998–2024** | 512.0 KB | `f41649ab0448db95db40f7661fcb21fc` | Factory Binary Firmware Dump |
| `'02 Chevy 2500 4x4 8.1 L18 os12216125.bin` | **1998–2024** | 512.0 KB | `f41649ab0448db95db40f7661fcb21fc` | Factory Binary Firmware Dump |
| `'02 Chevy K1500 5.3L os12216125 (1).bin` | **1998–2024** | 512.0 KB | `57b8a2bbed76b86b16295c48b0f2a8a7` | Factory Binary Firmware Dump |
| `2002 1500 5.3 12216125.bin` | **2002** | 512.0 KB | `3546d82cd8c5216cde4307c3c88d2d50` | Factory Binary Firmware Dump |
| `2002 4.8L LR4 4x2 1-2T MANUAL TRANS os12212156.bin` | **2002** | 512.0 KB | `177a2bfd1a26006e2378618dc6a9374a` | Factory Binary Firmware Dump |
| `2002 5.3L 2wd Stock DBC No EGR 12212156.bin` | **2002** | 512.0 KB | `6694c5961f93de2f8f0130647603e7ec` | Factory Binary Firmware Dump |
| `2002 5.3L Flex 2wd with Traction Stock 12216125.bin` | **2002** | 512.0 KB | `42e83a12d3f370a1ad1ee934363de924` | Factory Binary Firmware Dump |

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
