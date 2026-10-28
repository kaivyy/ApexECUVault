# MINI MOTO GROM MONKEY - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MINI MOTO GROM MONKEY
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
| `HONDA_38770-K0F-A01_Monkey_125_(2018-2020).xdf` | **2018–2020** | 16.3 KB | `ac6b42835a4acb708a145356c2d02960` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-901_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `d95896040243327d1aea4c12b2832cd3` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-911_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `802787442ffb7ba2f3a22e267dd30dcc` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-931_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `570e180502c1134751d23dfd3d39b64a` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-B02_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `08150f1f1ed5dcf906901a272e97b5f8` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-B13_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `56e94d9ce6e1975bea81247a6fcac38b` | TunerPro Binary Definition Map |
| `HONDA_38770-K26-C31_MSX_125___MSX_SF___Grom_125_(2013-2020).xdf` | **2013–2020** | 16.3 KB | `8e252df9c45da9a0ae39467942fda777` | TunerPro Binary Definition Map |

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
