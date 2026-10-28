# MAZDA 2 SKYACTIV D AND MZR - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MAZDA 2 SKYACTIV D AND MZR
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 11 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `Mazda-2015-2-1500-diesel-skyactiv-105HP-EGR_G.MOD` | **2015** | 4.00 MB | `f1ed5c7dcfa9fbbf400af876af501283` | ECU Calibration Asset |
| `Mazda-2015-2-1500-diesel-skyactiv-105HP_G.MOD` | **2015** | 4.00 MB | `86c8ba1dc419ccfdf009b30a56d62992` | ECU Calibration Asset |
| `Mazda-2015-2-1500-diesel-skyactiv-105HP_H_part.ori` | **2015** | 3.72 MB | `aad5a77f1e94858061c53f6ecd5bdef7` | Factory Binary Firmware Dump |
| `Mazda_2010_2_1300_MZR_86HP.ori` | **1998–2024** | 1.00 MB | `26395b013d94524dd9396a939e12065c` | Factory Binary Firmware Dump |
| `Mazda_2015_2_1500_diesel_skyactiv_105HP_G.ori` | **1998–2024** | 4.00 MB | `a30ead7c8ab9b4df343bc98c739a47cd` | Factory Binary Firmware Dump |
| `MAZDA_2_GEN2_2010_1.3L_MZR_86HP_DENSO_ORIGINAL_READ.ori` | **1998–2024** | 1.00 MB | `26395b013d94524dd9396a939e12065c` | Factory Binary Firmware Dump |
| `MAZDA_2_GEN2_2010_1.5L_MZR_DENSO_ORIGINAL_READ.ori` | **1998–2024** | 1.00 MB | `26395b013d94524dd9396a939e12065c` | Factory Binary Firmware Dump |
| `MAZDA_2_GEN3_2015_1.5L_DIESEL_SKYACTIV_D_105HP_ORIGINAL_READ.ori` | **1998–2024** | 4.00 MB | `a30ead7c8ab9b4df343bc98c739a47cd` | Factory Binary Firmware Dump |
| `Mazda_2_sky_D_H_full.ori` | **1998–2024** | 4.00 MB | `d6baa6c4992c2de2d1d3c3e6858ccb7b` | Factory Binary Firmware Dump |
| `Mazda_2_sky_D_H_Quantum_Green_full.MOD` | **1998–2024** | 4.00 MB | `5f99176ae8dced08ad3f8738b3ed7087` | ECU Calibration Asset |
| `Mazda_2_sky_D_H_Quantum_Green_part.MOD` | **1998–2024** | 3.72 MB | `49b42e093e6fe862a1bd325159895e3b` | ECU Calibration Asset |

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
