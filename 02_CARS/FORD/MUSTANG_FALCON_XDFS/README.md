# MUSTANG FALCON XDFS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MUSTANG FALCON XDFS
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 19 verified files
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
| `GUF1.xdf` | **1998–2024** | 481.7 KB | `32e206fb24fe927cf56cdf1acd4e9f79` | TunerPro Binary Definition Map |
| `GUFA.xdf` | **1998–2024** | 483.4 KB | `28d3c5bdf66182cff4b39850ebd44814` | TunerPro Binary Definition Map |
| `GUFB.xdf` | **1998–2024** | 485.1 KB | `f5b62ef9f570031f3f6f79cd05f58e79` | TunerPro Binary Definition Map |
| `HWAD3.xdf` | **1998–2024** | 43.1 KB | `9299466a21a1d47cdcfcfc831dd60337` | TunerPro Binary Definition Map |
| `IAW045_06.xdf` | **1998–2024** | 38.7 KB | `08427cd629463934008d86803e9e076f` | TunerPro Binary Definition Map |
| `IAW045_L01.xdf` | **1998–2024** | 39.1 KB | `35dacdb6094f23237b1def5e86a483db` | TunerPro Binary Definition Map |
| `L8edited1.0.xdf` | **1998–2024** | 73.0 KB | `dc3049c4a7ecc85e10cb063d3f15706a` | TunerPro Binary Definition Map |
| `LUX0.xdf` | **1998–2024** | 365.5 KB | `af55aa33baf0c13abedfebb4be45a3cf` | TunerPro Binary Definition Map |
| `N4AGB.xdf` | **1998–2024** | 68.0 KB | `8f4ba768f3f2166bc94447714611b829` | TunerPro Binary Definition Map |
| `NVMG8.xdf` | **1998–2024** | 402.2 KB | `2b4cff99e5ae3571d05a455074577895` | TunerPro Binary Definition Map |
| `P8_research_ver2.0.xdf` | **1998–2024** | 133.8 KB | `13513b416889c1c1e5c3c07d373f3b70` | TunerPro Binary Definition Map |
| `T23B.xdf` | **1998–2024** | 216.3 KB | `d538b0867b73e1afeff6f807f6c228e8` | TunerPro Binary Definition Map |

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
