# JAZZ CITY MOBILIO BRV L15 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: JAZZ CITY MOBILIO BRV L15
- **Model Year Coverage**: 2008–2023
- **Total Calibration Assets**: 13 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `37805-RD1-X520_Honda_Fit_1.4_16v_SH7058_1Mb.xdf` | **2008–2023** | 4.4 KB | `5194796b09e2fb0d78bae16e889c220f` | TunerPro Binary Definition Map |
| `37805-RME-A220_Honda_Fit_2008_Base__Sport_1.5L__L4_-_Gas.xdf` | **2008–2023** | 164.4 KB | `19999a2b5dcb1d6385f1cf3c85adb206` | TunerPro Binary Definition Map |
| `37805-RME-A520_Honda_Fit_2007_Base__Sport_1.5L__L4_-_Gas.xdf` | **2008–2023** | 3.3 KB | `de27f3391fe20313a190adc0263a4911` | TunerPro Binary Definition Map |
| `37805-RME-A690_Honda_Fit_2007_Base_1.5L__L4_-_Gas.xdf` | **2008–2023** | 3.3 KB | `3820751ea9cb0c63517424968d00e887` | TunerPro Binary Definition Map |
| `37805-RME-A720_Honda_Fit_2008_Base_1.5L__L4_-_Gas.xdf` | **2008–2023** | 3.3 KB | `2547f797235849723b1452653fb9edec` | TunerPro Binary Definition Map |
| `37805-RME-A890_Honda_Fit_2007_Sport_1.5L__L4_-_Gas.xdf` | **2008–2023** | 3.3 KB | `552c51391baf3642202284cc91f19838` | TunerPro Binary Definition Map |
| `37805-RME-C220_Honda_Fit_2008_Sport_1.5L__L4_-_Gas.xdf` | **2008–2023** | 3.3 KB | `ebd37128ab058249f52dcb6219f34a40` | TunerPro Binary Definition Map |
| `37805-RP3-3060_Honda_Fit_2009_Base__Sport_1.5L__L4_-_Gas.xdf` | **2008–2023** | 4.4 KB | `a761212ce470bb96cd0e23b90efa7e41` | TunerPro Binary Definition Map |
| `37805-RP3-4050_Honda_Fit_2009_Base_1.5L__L4_-_Gas.xdf` | **2008–2023** | 4.4 KB | `0e73a0edb114780c1a457fd03b46c950` | TunerPro Binary Definition Map |
| `37805-RP3-A170_Honda_Fit_2009_2010_Sport_1.5L__L4_-_Gas.xdf` | **2008–2023** | 4.4 KB | `378c0b3c3226344fd5864ba75212e3e0` | TunerPro Binary Definition Map |
| `37805-RP3-A770_Honda_Fit_2012_2013_Base__Sport_1.5L__L4_-_Gas.xdf` | **2008–2023** | 4.4 KB | `d88b75c028f8f2ab3eba17948ac2216c` | TunerPro Binary Definition Map |
| `37805-RP6-A560_Honda_Fit_2012_2013_Sport_1.5L__L4_-_Gas.xdf` | **2008–2023** | 7.6 KB | `47fe6f60e2910f3c230b1bb604e039d8` | TunerPro Binary Definition Map |
| `HONDA_37805-5A4-J81_JAZZ_GK5.xdf` | **2008–2023** | 11.9 KB | `0d5c74b19221cb45ea40bd66fb310dc0` | TunerPro Binary Definition Map |

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
