# 911 964 928 951 BINS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: 911 964 928 951 BINS
- **Model Year Coverage**: 1984–1994
- **Total Calibration Assets**: 10 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `0280 002 506_89_90_928GT.bin` | **1984–1994** | 16.0 KB | `a42f8772f60b5349d465505f92808e21` | Factory Binary Firmware Dump |
| `1992_964C2_181240302612004.bin` | **1984–1994** | 32.0 KB | `4a80379710ad06693272201065435fd1` | Factory Binary Firmware Dump |
| `84 Carrera OE EUR 1267355099.BIN` | **1984–1994** | 2.0 KB | `06ef03234fc31811452f6b858a6da12e` | Factory Binary Firmware Dump |
| `84 Carrera OE USA 1267355102.BIN` | **1984–1994** | 2.0 KB | `42da250a6baea01947a93d296a2e9b01` | Factory Binary Firmware Dump |
| `86 Carrera OE EUR 1267355027.BIN` | **1984–1994** | 4.0 KB | `838570336bf5296e7fcccf58bc0b61f1` | Factory Binary Firmware Dump |
| `86 Carrera OE USA 1267355180.BIN` | **1984–1994** | 4.0 KB | `a93082beaf43be3062ceea3eb718d600` | Factory Binary Firmware Dump |
| `87 Carrera OE USA 1267355236.BIN` | **1984–1994** | 4.0 KB | `65e847abf81cd3b82d1ef666c9513aca` | Factory Binary Firmware Dump |
| `gt-91_0280.002.509.bin` | **1984–1994** | 32.0 KB | `98b96e6d79eb8f8f31219aac0967ac65` | Factory Binary Firmware Dump |
| `Porsche951DME24pin.bin` | **1984–1994** | 4.0 KB | `b1f78205c945d31bb8aade9a93ed3291` | Factory Binary Firmware Dump |
| `Porsche951DME28pin.BIN` | **1984–1994** | 8.0 KB | `ea9d6a82002b68d0b03229c535ce6c4b` | Factory Binary Firmware Dump |

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
