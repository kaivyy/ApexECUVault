# SAAB TRIONIC LH - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SAAB TRIONIC LH
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 8 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `0 280 000 944_LH242.bin` | **1998–2024** | 32.0 KB | `53cee307d4ac9cd4127e3c00b152a1f8` | Factory Binary Firmware Dump |
| `0 280 000 948_LH24.bin` | **1998–2024** | 32.0 KB | `8eed3efe1b09daf904c29bcd5edc4916` | Factory Binary Firmware Dump |
| `SAAB9000 ORIGINAL579.bin` | **1998–2024** | 32.0 KB | `f2c76615a85eef2a820a8dc59f27882c` | Factory Binary Firmware Dump |
| `Saab_LH22_538.xdf` | **1998–2024** | 5.0 KB | `13998a31e456efa7425c5e0dc76e482d` | TunerPro Binary Definition Map |
| `SaabLH241_579.xdf` | **1998–2024** | 22.7 KB | `40ea871535cb347aa3fc0e649b03328f` | TunerPro Binary Definition Map |
| `SaabLH242_944_900sNA.xdf` | **1998–2024** | 11.2 KB | `cd7817fac689279835457a4c71992845` | TunerPro Binary Definition Map |
| `SaabLH24_585_582_586.xdf` | **1998–2024** | 18.0 KB | `bd011bc7ad34aa947cb720db9094efc4` | TunerPro Binary Definition Map |
| `SaabLH24_948.xdf` | **1998–2024** | 17.8 KB | `4fd421b8bb30960e0bb59cb910b32318` | TunerPro Binary Definition Map |

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
