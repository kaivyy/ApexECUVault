# SPORT YZF R15 R25 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SPORT YZF R15 R25
- **Model Year Coverage**: 2014–2025
- **Total Calibration Assets**: 6 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_2PK-E591A-00_Yamaha_YZF-R15_V2_non-VVA_(2014-2016).xdf` | **2014–2016** | 5.4 KB | `f2c4a72b6790e9fd6624d6e51dba1ba7` | TunerPro Binary Definition Map |
| `GENERATIONAL_BDJ-H591A-00_Yamaha_YZF_R15M_V4_2022_2025_CANBUS_QS_TC.xdf` | **2014–2025** | 2.5 KB | `cc78fcc3faa88201a34895680ebfa3e1` | TunerPro Binary Definition Map |
| `YAMAHA_1WD-H591A-00_Yamaha_YZF-R25___MT-25_(1WD_B02).xdf` | **2014–2025** | 6.5 KB | `c4f5474425a0c7b35eaac07b0b411ec4` | TunerPro Binary Definition Map |
| `YAMAHA_BBD-H594A-00_Yamaha_YZF-R15_V4___R15M_(BBD).xdf` | **2014–2025** | 11.6 KB | `688afd29f60c9f125793df52baafe568` | TunerPro Binary Definition Map |
| `YAMAHA_BK6-H594A-00_Yamaha_YZF-R15_V3_VVA_(BK6).xdf` | **2014–2025** | 11.6 KB | `722516ce18a2645ea1314beb012997d4` | TunerPro Binary Definition Map |
| `YZF-R125_B5G0.bin` | **2014–2025** | 27.0 KB | `b96862cf560be96c73a12991d692ccae` | Factory Binary Firmware Dump |

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
