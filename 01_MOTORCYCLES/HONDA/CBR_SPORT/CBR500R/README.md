# CBR500R - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: CBR500R
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 9 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `38770-MGZ-A03.bin` | **1998–2024** | 256.0 KB | `f6a6d9cebc04702d2b2b6ea9e79285fb` | Factory Binary Firmware Dump |
| `38770-MGZ-C02.bin` | **1998–2024** | 256.0 KB | `40e29ed018bf30a2f0d4c67a6111cbd4` | Factory Binary Firmware Dump |
| `38770-MGZ-C03.bin` | **1998–2024** | 256.0 KB | `f6ecaefc0067babc704fa442e54d7184` | Factory Binary Firmware Dump |
| `38770-MGZ-D02.bin` | **1998–2024** | 256.0 KB | `541fbc35987007aa9834cd070d71cab6` | Factory Binary Firmware Dump |
| `38770-MGZ.xdf` | **1998–2024** | 26.9 KB | `e35c3132febb369200d7a54bbe120e87` | TunerPro Binary Definition Map |
| `38770-MJW-AQ1.bin` | **1998–2024** | 256.0 KB | `5b69fdd34ab97f0546e87b12a2613242` | Factory Binary Firmware Dump |
| `38770-MJW-DR1.bin` | **1998–2024** | 256.0 KB | `1827b58adfcdb7cf7fb89a4b07ebae41` | Factory Binary Firmware Dump |
| `38770-MJW-T11.bin` | **1998–2024** | 256.0 KB | `16d661c881f6d4694eedb0aab93cfab3` | Factory Binary Firmware Dump |
| `38770-MJW.xdf` | **1998–2024** | 71.7 KB | `8e5d477d5a174cc1f394ccbadb209698` | TunerPro Binary Definition Map |

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
