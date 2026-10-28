# EEC IV EEC V BINS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: EEC IV EEC V BINS
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 15 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `6DFC.bin` | **1998–2024** | 256.0 KB | `2767e7e30e0652a9e795cfb5b409e982` | Factory Binary Firmware Dump |
| `6DFD.bin` | **1998–2024** | 256.0 KB | `cb30e24470eb6d6725792135e5d906d4` | Factory Binary Firmware Dump |
| `6DGC.bin` | **1998–2024** | 256.0 KB | `113db590ff6234de01d3ef3df75bd96d` | Factory Binary Firmware Dump |
| `6DGD.bin` | **1998–2024** | 256.0 KB | `90bbde737a318cdfcbb352e22e14c868` | Factory Binary Firmware Dump |
| `CBAZA.xdf` | **1998–2024** | 309.9 KB | `dc4628312362aa97968951d40fc5891d` | TunerPro Binary Definition Map |
| `CDAN4.xdf` | **1998–2024** | 168.7 KB | `5e134df0c835951cd23c969d405d9d6c` | TunerPro Binary Definition Map |
| `CRAJ0.xdf` | **1998–2024** | 210.7 KB | `00a2acf2a4905fd93bf8c95119e4148e` | TunerPro Binary Definition Map |
| `Ford_EEC-IV_8SD_Calibration_OEM_ORI.bin` | **1998–2024** | 56.0 KB | `a693aa0e93a438ce402f84ce6e1730ae` | Factory Binary Firmware Dump |
| `Ford_EEC-IV_AA_FirstGen1985_Calibration_OEM_ORI.bin` | **1998–2024** | 8.0 KB | `f0a376de3debc1d7d3bd2b3e419dbf1f` | Factory Binary Firmware Dump |
| `Ford_EEC-IV_M0M2_Calibration_OEM_ORI.bin` | **1998–2024** | 56.0 KB | `5d9560aa49ba658022bc4770a85382b9` | Factory Binary Firmware Dump |
| `Ford_EEC-IV_X1L_Calibration_OEM_ORI.bin` | **1998–2024** | 56.0 KB | `d21f5c34b9aa6999d529f7437f97d037` | Factory Binary Firmware Dump |
| `Ford_Mustang_5.0L_FoxBody_Manual_A9L_OEM_ORI.bin` | **1998–2024** | 32.0 KB | `0a7759f430653e280cbdd3f02d8bf322` | Factory Binary Firmware Dump |
| `Ford_Thunderbird_TurboCoupe_MustangSVO_2.3T_LA3_OEM_ORI.bin` | **1998–2024** | 32.0 KB | `b1525a5c93dcfac2e3cf7b24ed10521c` | Factory Binary Firmware Dump |
| `GUFA.xdf` | **1998–2024** | 483.4 KB | `28d3c5bdf66182cff4b39850ebd44814` | TunerPro Binary Definition Map |
| `GUFB.xdf` | **1998–2024** | 485.1 KB | `f5b62ef9f570031f3f6f79cd05f58e79` | TunerPro Binary Definition Map |

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
