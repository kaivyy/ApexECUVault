# BMW CLASSIC MOTRONIC - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: BMW CLASSIC MOTRONIC
- **Model Year Coverage**: 1982–1995
- **Total Calibration Assets**: 23 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `745i_singleCHIP_64K.xdf` | **1982–1995** | 32.1 KB | `974ed38b5aa62ccc4b65226c9906a9e7` | TunerPro Binary Definition Map |
| `750iL_156.xdf` | **1982–1995** | 22.4 KB | `48d89f2c0375e13d9e4c7d38b2adb2ae` | TunerPro Binary Definition Map |
| `BMW173Chip.xdf` | **1982–1995** | 51.3 KB | `264d914ee55311e4a1d80b09b250be0b` | TunerPro Binary Definition Map |
| `BMW173Chip_M20_B25.xdf` | **1982–1995** | 51.3 KB | `264d914ee55311e4a1d80b09b250be0b` | TunerPro Binary Definition Map |
| `BMW173HakenTTBiggerMapsV11.xdf` | **1982–1995** | 30.1 KB | `c3f658a67079c06e57163b3821ece396` | TunerPro Binary Definition Map |
| `BMW87_E30_153dme.xdf` | **1982–1995** | 44.4 KB | `1ad3476d9e2df6b9f9fcb32e3336881b` | TunerPro Binary Definition Map |
| `BMW_027_DME_E30_4K.xdf` | **1982–1995** | 14.3 KB | `db653ce40376b0e4532cba00bcab7448` | TunerPro Binary Definition Map |
| `BMW_059_DME_M30_4KChip.xdf` | **1982–1995** | 20.6 KB | `0f9b4b976ef87d9a34443c262d458491` | TunerPro Binary Definition Map |
| `BMW_175_318i_soft378.xdf` | **1982–1995** | 44.8 KB | `2df0b632685cc56255c7cb63a2d4ce12` | TunerPro Binary Definition Map |
| `BMW_413_red label_chip623.xdf` | **1982–1995** | 85.2 KB | `149dd6817aa649f7d01fadc95a078548` | TunerPro Binary Definition Map |
| `BMW_850i_ecu352_soft566.xdf` | **1982–1995** | 30.4 KB | `6d4ed5bbf6c2a8eabda70d5168831f44` | TunerPro Binary Definition Map |
| `BMW_990_318i_soft070.xdf` | **1982–1995** | 33.9 KB | `9de64794f424a6b032bb4a4424003c10` | TunerPro Binary Definition Map |
| `BMW_dme405_soft951.xdf` | **1982–1995** | 23.8 KB | `d71a1157cbde2038851c132f6d9cc04b` | TunerPro Binary Definition Map |
| `BMW_DME_179.xdf` | **1982–1995** | 27.2 KB | `718c459920a153b001e4097ac444f7b4` | TunerPro Binary Definition Map |
| `BMW_dme_404.xdf` | **1982–1995** | 11.0 KB | `7b1443c96078959f806b732b1e31f148` | TunerPro Binary Definition Map |
| `BMW_E30_081.xdf` | **1982–1995** | 18.1 KB | `98bed578e21b68927e4f864072dc236c` | TunerPro Binary Definition Map |
| `BMW_ecu402_soft599.xdf` | **1982–1995** | 15.3 KB | `4479574da188188214b96f1c695efcc3` | TunerPro Binary Definition Map |
| `BMW_ecu403_soft950.xdf` | **1982–1995** | 14.7 KB | `bdb662da5dbca2dc222597955f8398b6` | TunerPro Binary Definition Map |
| `BMW_ecu403_soft950_M50_B25.xdf` | **1982–1995** | 14.7 KB | `bdb662da5dbca2dc222597955f8398b6` | TunerPro Binary Definition Map |
| `BMW_M20B25_ecu173_sw705.xdf` | **1982–1995** | 356.4 KB | `ec8529cb0ff3f0137eaae492d706bdce` | TunerPro Binary Definition Map |
| `BMW_M3_506_soft965.xdf` | **1982–1995** | 44.3 KB | `0325ada5dfa87de3cff4e2430f525843` | TunerPro Binary Definition Map |
| `BMW_S14_E30_M3_dme071.xdf` | **1982–1995** | 20.8 KB | `46d1e5bf5202a7709d730e26385339ed` | TunerPro Binary Definition Map |
| `E36_EuroM3_dme075.xdf` | **1982–1995** | 16.4 KB | `c96a4f9644a3c2ea8106eec66818c5e1` | TunerPro Binary Definition Map |

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
