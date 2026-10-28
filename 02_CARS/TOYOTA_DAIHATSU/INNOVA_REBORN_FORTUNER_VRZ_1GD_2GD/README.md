# INNOVA REBORN FORTUNER VRZ 1GD 2GD - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: INNOVA REBORN FORTUNER VRZ 1GD 2GD
- **Model Year Coverage**: 2015–2024
- **Total Calibration Assets**: 4 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_89663-F0110_Toyota_Innova_Reborn_2.4_GD_Clean_Diesel_2015_2022.xdf` | **2015–2024** | 1.5 KB | `80771c807597416fcb48c245c3a160f0` | TunerPro Binary Definition Map |
| `GENERATIONAL_89663-F0890_FORTUNER_1GD_2_8_Toyota_Fortuner_GR_Sport_2.8_GD_Clean_Diesel_(2022-2026).xdf` | **2022–2026** | 5.4 KB | `de9fbbe8fec08710276d7dc29bd1cb29` | TunerPro Binary Definition Map |
| `GENERATIONAL_89663-F0890_Toyota_Fortuner_GR_Sport_2.8_GD_Clean_Diesel_2022_2026.xdf` | **2015–2024** | 1.5 KB | `0eac985b049c6b3078a56cf83afaa524` | TunerPro Binary Definition Map |
| `TOYOTA_89663-F0110_2GD.xdf` | **2015–2024** | 11.9 KB | `f12bbe2a5654211915b21ca4857e423a` | TunerPro Binary Definition Map |

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
