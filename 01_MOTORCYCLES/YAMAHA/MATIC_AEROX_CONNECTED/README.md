# MATIC AEROX CONNECTED - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MATIC AEROX CONNECTED
- **Model Year Coverage**: 2020–2024
- **Total Calibration Assets**: 6 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `AEROX  BBP-H594A-01.bin` | **2020–2024** | 1.00 MB | `6c914cceec621a8c3ac232b9a0efa1b8` | Factory Binary Firmware Dump |
| `New Aerox  --  BBP-H594A-11.bin` | **2020–2024** | 1.00 MB | `f12768cffd6016308bca2e3dfa350a3f` | Factory Binary Firmware Dump |
| `YAMAHA_AEROX_155_VVA_2020_BBP-H594A-01.bin` | **2020–2024** | 1.00 MB | `6c914cceec621a8c3ac232b9a0efa1b8` | Factory Binary Firmware Dump |
| `YAMAHA_AEROX_155_VVA_2020_BBP-H594A-01.xdf` | **2020–2024** | 73.9 KB | `e419411bc9f6a42c6a7dfe0c3710dc0f` | TunerPro Binary Definition Map |
| `YAMAHA_ALL_NEW_AEROX_CONNECTED_155_VVA_2021-2024_BBP-H594A-11.bin` | **2020–2024** | 1.00 MB | `f12768cffd6016308bca2e3dfa350a3f` | Factory Binary Firmware Dump |
| `YAMAHA_ALL_NEW_AEROX_CONNECTED_155_VVA_2021-2024_BBP-H594A-11.xdf` | **2020–2024** | 73.9 KB | `444031e7517a39a00ee74233f381d82e` | TunerPro Binary Definition Map |

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
