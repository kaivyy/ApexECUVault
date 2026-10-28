# FORTUNER 1GR FE 4 0L V6 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: FORTUNER 1GR FE 4 0L V6
- **Model Year Coverage**: 2005–2015
- **Total Calibration Assets**: 5 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `TOYOTA_4RUNNER_FORTUNER_2006_4.0L_V6_1GRFE_89663-35292.bin` | **2005–2015** | 384.0 KB | `1669b796a63862e27247ef5b65ad7410` | Factory Binary Firmware Dump |
| `TOYOTA_89663-F0852_1GR.xdf` | **2005–2015** | 9.8 KB | `dd2f881036a4995cd44ae636f78e1db5` | TunerPro Binary Definition Map |
| `TOYOTA_FJ_CRUISER_FORTUNER_2011_4.0L_V6_1GRFE_89663-YWK01.bin` | **2005–2015** | 736.0 KB | `b95a0ca3d0ed2e095d52b84ff552f1d8` | Factory Binary Firmware Dump |
| `TOYOTA_FORTUNER_PRADO_LC120_2008_4.0L_V6_1GRFE_89663-60551.bin` | **2005–2015** | 736.0 KB | `3f49683123aaf9dcabdaa8e5f2a03ae7` | Factory Binary Firmware Dump |
| `TOYOTA_FORTUNER_PRADO_LC150_2014_4.0L_V6_1GRFE_89663-60E64.bin` | **2005–2015** | 992.0 KB | `9b47aa92031ba832eb652c8b2353987b` | Factory Binary Firmware Dump |

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
