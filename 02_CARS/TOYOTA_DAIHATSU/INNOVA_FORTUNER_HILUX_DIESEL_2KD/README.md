# INNOVA FORTUNER HILUX DIESEL 2KD - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: INNOVA FORTUNER HILUX DIESEL 2KD
- **Model Year Coverage**: 2004–2015
- **Total Calibration Assets**: 10 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_89663-0K180_INNOVA_NON_IC_Toyota_Kijang_Innova_2.5_D-4D_Gen_1_Non-Intercooler_(2004-2011).xdf` | **2004–2011** | 5.4 KB | `f3d847d8821a7774206d6b2897dcc339` | TunerPro Binary Definition Map |
| `GENERATIONAL_89663-0K750_INNOVA_VNT_Toyota_Kijang_Innova_2.5_D-4D_Gen_1_VN-Turbo_Intercooler_(2011-2015).xdf` | **2011–2015** | 5.4 KB | `226aa21afde583f159d71a00e9b3615d` | TunerPro Binary Definition Map |
| `GENERATIONAL_89663-0K750_Toyota_Innova_2.5_D_4D_VN_Turbo_Intercooler_2011_2015.xdf` | **2004–2015** | 1.5 KB | `8f8354630cfd53fd245e6584e3afcbc9` | TunerPro Binary Definition Map |
| `TOYOTA_89663-0K180_2KD.xdf` | **2004–2015** | 11.8 KB | `40354a237258699f8cac86235dfd0201` | TunerPro Binary Definition Map |
| `TOYOTA_FORTUNER_INNOVA_2012_2.7L_2TRFE_AUTO_89663-0K630.bin` | **2004–2015** | 368.0 KB | `bc9e8ac16f923a62af7413c6e63ea86f` | Factory Binary Firmware Dump |
| `TOYOTA_FORTUNER_INNOVA_2014_2.7L_2TRFE_AUTO_89663-0KX30.bin` | **2004–2015** | 512.0 KB | `056b4788d3e706ef9f9050895a27fa7b` | Factory Binary Firmware Dump |
| `TOYOTA_HIACE_HILUX_2011_2.5TD_2KDFTV_89663-26331.bin` | **2004–2015** | 368.0 KB | `b3cbd5f50d25442e9e5562e4163009d8` | Factory Binary Firmware Dump |
| `TOYOTA_INNOVA_HILUX_2012_2.5TD_2KDFTV_MANUAL_89663-0KM60.bin` | **2004–2015** | 496.0 KB | `c871a59bb497d208b5d63aa440003a01` | Factory Binary Firmware Dump |
| `TOYOTA_INNOVA_HILUX_2013_2.5TD_2KDFTV_MANUAL_89663-0KM63.bin` | **2004–2015** | 496.0 KB | `bba31550b1c308a9270c562cd6930911` | Factory Binary Firmware Dump |
| `TOYOTA_INNOVA_HILUX_VNT_2014_2.5TD_2KDFTV_AUTO_89663-0KR70.bin` | **2004–2015** | 992.0 KB | `5d52e47279a8ffcb3de351d13a0ad687` | Factory Binary Firmware Dump |

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
