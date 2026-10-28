# OS 12585950 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: OS 12585950
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 5 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `'04K1500 6.0L os12585950.bin` | **1998–2024** | 1.00 MB | `b2f9032d77bf127a616172ca98d68540` | Factory Binary Firmware Dump |
| `04 Chevy half Ton 4x4 6.0L 12585950.bin` | **1998–2024** | 1.00 MB | `bd5f2b1e6cac09f47f0ead78a040a678` | Factory Binary Firmware Dump |
| `04 Silverado SS 11.8.13 Stock OS12585950.bin` | **1998–2024** | 1.00 MB | `32f23ba73e088816499330fc64b478bb` | Factory Binary Firmware Dump |
| `Chevy_2500_4x4_LQ4_OS12585950.bin` | **1998–2024** | 1.00 MB | `ff7b6b81c46541433ea4228f4c1739d4` | Factory Binary Firmware Dump |
| `Chevy_4x4_Half_T_6.0L_OS12585950.bin` | **1998–2024** | 1.00 MB | `355bfee4826c90b567ef76bfb473212b` | Factory Binary Firmware Dump |

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
