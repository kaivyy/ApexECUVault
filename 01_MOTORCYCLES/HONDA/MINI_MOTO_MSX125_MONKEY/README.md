# MINI MOTO MSX125 MONKEY - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MINI MOTO MSX125 MONKEY
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 16 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `38770-K0F-A01.bin` | **1998–2024** | 96.0 KB | `b1b2d8fbdb85538f1b764e9059f0def5` | Factory Binary Firmware Dump |
| `38770-K0F-A01.xdf` | **1998–2024** | 15.5 KB | `cdffe0fc5392f14f81a4456a9e4c2f34` | TunerPro Binary Definition Map |
| `38770-K26-911.bin` | **1998–2024** | 48.0 KB | `eca31aa92cd73763dd6500174de10e0c` | Factory Binary Firmware Dump |
| `38770-K26-911.xdf` | **1998–2024** | 13.8 KB | `707232a042ceed90cd85b7aa09c88505` | TunerPro Binary Definition Map |
| `38770-K26-931.bin` | **1998–2024** | 48.0 KB | `cf324b8b009cf0f527ef34d8d6ba5021` | Factory Binary Firmware Dump |
| `38770-K26-B13.bin` | **1998–2024** | 64.0 KB | `3ce4aee4afaddf4d8ca3f194b13fc168` | Factory Binary Firmware Dump |
| `38770-K26-B13.xdf` | **1998–2024** | 12.5 KB | `5d433c3d0f453a7b4c72d425831b14e0` | TunerPro Binary Definition Map |
| `38770-K26-C31.bin` | **1998–2024** | 64.0 KB | `4ebb017f7ca9287ae5c54db3a8704106` | Factory Binary Firmware Dump |
| `38770-K26-C31.xdf` | **1998–2024** | 23.9 KB | `1d4c0cfe07e37230dd4b486fe80b2dc5` | TunerPro Binary Definition Map |
| `38770-KYT-901.bin` | **1998–2024** | 56.0 KB | `2c4b1f41ef4bb9d110cc2feaa8a6f744` | Factory Binary Firmware Dump |
| `HONDA_CT125_HUNTER_CUB_38770_K2E_T02_96KB_ORI.bin` | **1998–2024** | 96.0 KB | `9961640a253687ce909811b95a1ea5a3` | Factory Binary Firmware Dump |
| `HONDA_GROM_125_38770_K26_G01_96KB_ORI.bin` | **1998–2024** | 96.0 KB | `483437f2b5eea4afad8e424cd0713bc1` | Factory Binary Firmware Dump |
| `HONDA_MONKEY_125_38770_K0F_T01_96KB_ORI.bin` | **1998–2024** | 96.0 KB | `832da9a1bbaa020173dc66bc402b1b17` | Factory Binary Firmware Dump |
| `HONDA_MONKEY_Z125M_38770_K0F_A01_96KB_ORI.bin` | **1998–2024** | 96.0 KB | `b1b2d8fbdb85538f1b764e9059f0def5` | Factory Binary Firmware Dump |
| `HONDA_MSX125_38770_K26_901_48KB_ORI.bin` | **1998–2024** | 48.0 KB | `c273b62d40678dc3ce070963f880f9dc` | Factory Binary Firmware Dump |
| `HONDA_MSX125_SF_38770_K26_B13_64KB_ORI.bin` | **1998–2024** | 64.0 KB | `3ce4aee4afaddf4d8ca3f194b13fc168` | Factory Binary Firmware Dump |

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
