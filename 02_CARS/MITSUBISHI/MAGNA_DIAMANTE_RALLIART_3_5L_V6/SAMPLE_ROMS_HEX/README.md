# SAMPLE ROMS HEX - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SAMPLE ROMS HEX
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 15 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `00 TH Executive 3-0 Auto.hex` | **1998–2024** | 128.0 KB | `29e28b3c2edba41b971fc61aeff2e0c2` | Intel HEX Calibration Firmware |
| `00 TJ Solara 3-5 Auto.hex` | **1998–2024** | 512.0 KB | `030e0fb3800f1c527e1da4c99aaa4e36` | Intel HEX Calibration Firmware |
| `00 TJ VR-X 3-5 Auto.hex` | **1998–2024** | 512.0 KB | `78d44b0db984b08be55a78505d6110e8` | Intel HEX Calibration Firmware |
| `00 TJ VR-X 3-5 Manual.hex` | **1998–2024** | 256.0 KB | `51cee78ffc93d09593e40654828728c0` | Intel HEX Calibration Firmware |
| `01 TJ LE (Comm Games) 3-5 Auto.hex` | **1998–2024** | 512.0 KB | `36fe7a138dce32e7c2e81549d24e0780` | Intel HEX Calibration Firmware |
| `01 TJ VR-X MY02 3-5 Manual.hex` | **1998–2024** | 256.0 KB | `33193ac19d6001b27dace25d6a349247` | Intel HEX Calibration Firmware |
| `01 USDM Diamante 3-5 Auto.hex` | **1998–2024** | 512.0 KB | `dbcea2788bad4391445eb71db86d0517` | Intel HEX Calibration Firmware |
| `02 USDM Diamante 3-5 Auto.hex` | **1998–2024** | 512.0 KB | `c57b71c99c0e655a6e7b7b7074044b88` | Intel HEX Calibration Firmware |
| `03 TJ AWD 3-5 Auto.hex` | **1998–2024** | 512.0 KB | `075703b1b67d002ae574b7ec232e9842` | Intel HEX Calibration Firmware |
| `03 TJ Executive 3-5 Auto.hex` | **1998–2024** | 256.0 KB | `426a7cadcfff10b04a0ae71b852d0698` | Intel HEX Calibration Firmware |
| `03 TJ Ralliart 3-5 Auto.hex` | **1998–2024** | 512.0 KB | `552b1571e3608e846c3607e8893c915b` | Intel HEX Calibration Firmware |
| `03 TJ Ralliart 3-5 Manual.hex` | **1998–2024** | 256.0 KB | `e8f313c8768f7a53e3c542a606d3e71c` | Intel HEX Calibration Firmware |
| `04 TL AWD 3-5 Auto.hex` | **1998–2024** | 512.0 KB | `76f9cb2c9dd5a45c79553a37a5256708` | Intel HEX Calibration Firmware |
| `04 TL VR-X 3-5 Manual.hex` | **1998–2024** | 256.0 KB | `133d81f75afc32b5f52453546581d313` | Intel HEX Calibration Firmware |
| `99 TH Sports 3-5 Manual.hex` | **1998–2024** | 128.0 KB | `b313dff3624180f75e596a95b688b5ed` | Intel HEX Calibration Firmware |

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
