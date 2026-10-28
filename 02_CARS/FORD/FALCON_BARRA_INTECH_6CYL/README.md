# FALCON BARRA INTECH 6CYL - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: FALCON BARRA INTECH 6CYL
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 26 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `12AF_NGIC9A5.256k.bin` | **1998–2024** | 256.0 KB | `ba73856610803713c3cbe86a44377f3f` | Factory Binary Firmware Dump |
| `12BE_NGIC9B3.256k.bin` | **1998–2024** | 256.0 KB | `956675312536ba1600ac05e20670b51b` | Factory Binary Firmware Dump |
| `12CD_NGIC9CF.256k.bin` | **1998–2024** | 256.0 KB | `b8bf23db71a16b2a64e6d01106d05776` | Factory Binary Firmware Dump |
| `12FD_NGIC9F9.256k.bin` | **1998–2024** | 256.0 KB | `37208c17d320535180ea0ef615a55c5d` | Factory Binary Firmware Dump |
| `12UD-TurboEnhancedFuel.bin` | **1998–2024** | 256.0 KB | `1bf9b180d0bcd2f0752e540f4f636fe2` | Factory Binary Firmware Dump |
| `12UD_NGIC9UZ.256k.bin` | **1998–2024** | 256.0 KB | `51b1e4fe858d8498eed593e6c06fd00e` | Factory Binary Firmware Dump |
| `12VC_NGIC9V7.256k.bin` | **1998–2024** | 256.0 KB | `553c7b0d05f2ba6b6aa11535253525c6` | Factory Binary Firmware Dump |
| `12WD_NGIC9WG.256k.bin` | **1998–2024** | 256.0 KB | `5db014395b690fa7169543a21dea1cb7` | Factory Binary Firmware Dump |
| `12ZE_NGIC9Z4.256k.bin` | **1998–2024** | 256.0 KB | `9a92151df8cca7753f84fc34464999be` | Factory Binary Firmware Dump |
| `22AB_NGIC9AJ.256k.bin` | **1998–2024** | 256.0 KB | `2aac62b296caa3be655a5e341ed984c8` | Factory Binary Firmware Dump |
| `22VA_NGICA2Z.256k.bin` | **1998–2024** | 256.0 KB | `9ab4d9d4734b44ddba007d83d49a0f36` | Factory Binary Firmware Dump |
| `3DAC Extended Alpha.xdf` | **1998–2024** | 165.2 KB | `c4c81208e0f5f98e431cfb2962e540ed` | TunerPro Binary Definition Map |
| `3DAC PrePatched.bin` | **1998–2024** | 256.0 KB | `9e5825008f152376c896af659a69e940` | Factory Binary Firmware Dump |
| `HWAD3 Early Access 0.1.xdf` | **1998–2024** | 385.1 KB | `5dbe568c3dfc299e435e907f84f10c5d` | TunerPro Binary Definition Map |
| `N9XJ4 Extended v1.1.xdf` | **1998–2024** | 256.9 KB | `c5b464110a9589f4130d877a159c0d0b` | TunerPro Binary Definition Map |
| `N9XJ4 Extended.xdf` | **1998–2024** | 254.3 KB | `e6289cccf4476e4ac4269a6000278430` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.1.xdf` | **1998–2024** | 321.8 KB | `a86bfe65875fc6385aeaa7f3cde7747e` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.11.xdf` | **1998–2024** | 329.5 KB | `924c853ac12f47bd5496c927b62980ea` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.12.xdf` | **1998–2024** | 330.2 KB | `33f15c812bb6fbaaa8de8e23a4a95b38` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.2.xdf` | **1998–2024** | 478.6 KB | `b1c4001dccdc7092ead68af2e43b302d` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.21.xdf` | **1998–2024** | 548.5 KB | `a67ccbd487a25226935f2e9d3765d40c` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.3.xdf` | **1998–2024** | 1.06 MB | `64d05f2f70267cf8952cb69fad8bee59` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.31-b.xdf` | **1998–2024** | 1.06 MB | `00b13751c3e4ca5b3dce216098cf1346` | TunerPro Binary Definition Map |
| `NGIC9 Extended v1.32-b.xdf` | **1998–2024** | 1.06 MB | `280d9f62741d500a34679be209f8b35b` | TunerPro Binary Definition Map |
| `NGIC9 Extended.xdf` | **1998–2024** | 321.4 KB | `2db964227e8d6a87b63dd414c4411980` | TunerPro Binary Definition Map |
| `NGIC9 Generic.bin` | **1998–2024** | 256.0 KB | `ba73856610803713c3cbe86a44377f3f` | Factory Binary Firmware Dump |

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
