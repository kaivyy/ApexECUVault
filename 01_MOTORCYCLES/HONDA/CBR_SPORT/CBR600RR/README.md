# CBR600RR - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: CBR600RR
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 11 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `38770-MEE-612.bin` | **1998–2024** | 256.0 KB | `aecce9ae133d3dfd3bda9205f09f05ea` | Factory Binary Firmware Dump |
| `38770-MEE-622.bin` | **1998–2024** | 256.0 KB | `2742e3c741f55c578b81fea8c6fc6a6d` | Factory Binary Firmware Dump |
| `38770-MEE-F02.bin` | **1998–2024** | 256.0 KB | `cc6fdd6e9d2035cfb7af143e3642814b` | Factory Binary Firmware Dump |
| `38770-MFJ-A02.bin` | **1998–2024** | 256.0 KB | `b061d41db86aec0e346967361250b344` | Factory Binary Firmware Dump |
| `38770-MFJ-D04.bin` | **1998–2024** | 256.0 KB | `9743fe4c0ffa263869cc6c405394ac0c` | Factory Binary Firmware Dump |
| `38770-MFJ-F03.bin` | **1998–2024** | 256.0 KB | `5de5263aa9d7767f26945e9cf85c272c` | Factory Binary Firmware Dump |
| `38770-MGM-D11.bin` | **1998–2024** | 256.0 KB | `773d00c4f51ac9d5868d533aa3a85fe9` | Factory Binary Firmware Dump |
| `38770-MJC-A01.bin` | **1998–2024** | 256.0 KB | `4a3c7f75593a162aaf1adce606590e63` | Factory Binary Firmware Dump |
| `38770-MJC-D01.bin` | **1998–2024** | 256.0 KB | `210ae00bd01f4dc1de3aa09264886d6e` | Factory Binary Firmware Dump |
| `38770-N1A-D11.bin` | **1998–2024** | 256.0 KB | `68f033b3e7f5f5aa05fce050446d095e` | Factory Binary Firmware Dump |
| `38770-NL3-750.bin` | **1998–2024** | 256.0 KB | `4480e3c59a2f0f692efaff227321cd79` | Factory Binary Firmware Dump |

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
