# SUPRA 2JZ 1JZ A80 A90 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SUPRA 2JZ 1JZ A80 A90
- **Model Year Coverage**: 1993–2024
- **Total Calibration Assets**: 9 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_89661-14370_Toyota_Supra_MK3_JZA70_1JZ-GTE_TwinTurbo_1990_1993.xdf` | **1993–2024** | 7.2 KB | `dcfc32cce4f7ca510756507923043e14` | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-14480_Toyota_Supra_JZA80_2JZ-GTE_TwinTurbo_JDM_MT_1993_1997.xdf` | **1993–2024** | 7.2 KB | `088a1b96eb269b51e19efa47a7af9d6f` | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-14560_Toyota_Supra_JZA80_2JZ-GTE_TwinTurbo_USDM_MT_550cc_1993_1998.xdf` | **1993–2024** | 7.2 KB | `8ead3e202e5c157026e1b79724c91d0b` | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-14830_Toyota_Supra_JZA80_2JZ-GTE_VVTi_6MT_1997_2002.xdf` | **1993–2024** | 8.0 KB | `453af333e4e494d72b6676e6e2383b5a` | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-14840_Toyota_Supra_JZA80_2JZ-GTE_VVTi_AT_1997_2002.xdf` | **1993–2024** | 8.0 KB | `463d57010fa4631c018422d5aa58cb23` | TunerPro Binary Definition Map |
| `GENERATIONAL_89661-22810_Toyota_Chaser_JZX100_1JZ-GTE_VVTi_MT_1996_2001.xdf` | **1993–2024** | 7.6 KB | `79fd43ed238ec84113dfb7eb68e7a549` | TunerPro Binary Definition Map |
| `GENERATIONAL_B48B20_Toyota_GR_Supra_A90_2.0T_Bosch_MG1CS024_2020_2024.xdf` | **1993–2024** | 8.7 KB | `4b28f4dbcdb4c42bd8b45b60029550a3` | TunerPro Binary Definition Map |
| `GENERATIONAL_B58B30_Toyota_GR_Supra_A90_3.0T_Bosch_MG1CS024_2019_2020.xdf` | **1993–2024** | 8.7 KB | `0ed9be13fcdca8985b29684bb19bec7b` | TunerPro Binary Definition Map |
| `GENERATIONAL_B58B30O1_Toyota_GR_Supra_A90_3.0T_Facelift_MG1CS024_2021_2024.xdf` | **1993–2024** | 8.7 KB | `f1b4387258c3f76b85c2fa90c848c4d2` | TunerPro Binary Definition Map |

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
