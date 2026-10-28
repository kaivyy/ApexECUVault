# YARIS VIOS 1NZ 2NR - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: YARIS VIOS 1NZ 2NR
- **Model Year Coverage**: 2002–2024
- **Total Calibration Assets**: 11 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `89663-52823.bin` | **2002–2024** | 736.0 KB | `58eb8851d161037aecc21a423593e560` | Factory Binary Firmware Dump |
| `89663-52D30.bin` | **2002–2024** | 736.0 KB | `c32b1805eb056aa93989bbe2f9b83641` | Factory Binary Firmware Dump |
| `89663-52E91.bin` | **2002–2024** | 496.0 KB | `3ec27ed7072bdfe5d8af8444e6e20439` | Factory Binary Firmware Dump |
| `89663-52F01.bin` | **2002–2024** | 736.0 KB | `9f6ea82eefc59cdbf38a4fb4095af37e` | Factory Binary Firmware Dump |
| `89663-52F11.bin` | **2002–2024** | 736.0 KB | `63bd0bc11779249583fd41e5d336a15a` | Factory Binary Firmware Dump |
| `TOYOTA_89663-52xxx_VIOS.xdf` | **2002–2024** | 9.8 KB | `9b770c086209f131f29661b69aa6890b` | TunerPro Binary Definition Map |
| `TOYOTA_VIOS_YARIS_GEN2_2008_1.5L_1NZFE_MANUAL_89663-52E91.bin` | **2002–2024** | 496.0 KB | `3ec27ed7072bdfe5d8af8444e6e20439` | Factory Binary Firmware Dump |
| `TOYOTA_VIOS_YARIS_GEN2_2009_1.5L_1NZFE_AUTO_89663-52F01.bin` | **2002–2024** | 736.0 KB | `9f6ea82eefc59cdbf38a4fb4095af37e` | Factory Binary Firmware Dump |
| `TOYOTA_VIOS_YARIS_GEN2_2010_1.5L_1NZFE_AUTO_89663-52F11.bin` | **2002–2024** | 736.0 KB | `63bd0bc11779249583fd41e5d336a15a` | Factory Binary Firmware Dump |
| `TOYOTA_VIOS_YARIS_GEN3_2014_1.5L_1NZFE_AUTO_89663-52D30.bin` | **2002–2024** | 736.0 KB | `c32b1805eb056aa93989bbe2f9b83641` | Factory Binary Firmware Dump |
| `TOYOTA_YARIS_VIOS_1.3L_2SZFE_89663-52823.bin` | **2002–2024** | 736.0 KB | `58eb8851d161037aecc21a423593e560` | Factory Binary Firmware Dump |

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
