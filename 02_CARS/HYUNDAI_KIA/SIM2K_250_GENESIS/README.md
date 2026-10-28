# SIM2K 250 GENESIS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SIM2K 250 GENESIS
- **Model Year Coverage**: 2016–2023
- **Total Calibration Assets**: 11 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `HYUNDAI_SIM2K_250_TURBO_G70.xdf` | **2016–2023** | 7.5 KB | `49459dfd9b38e47912679ab611afe91e` | TunerPro Binary Definition Map |
| `SIM2K-250_606X0A5000000_GCC_FuelQuality.bin` | **2016–2023** | 2.50 MB | `7de2bfa910ffa0153cf58a971b76fc95` | Factory Binary Firmware Dump |
| `SIM2K-250_606X0A5000000_Original.bin` | **2016–2023** | 2.50 MB | `d35f24bb40df96db4958378f06d34174` | Factory Binary Firmware Dump |
| `SIM2K-250_606X1A6K00000_GCC_FuelQuality.bin` | **2016–2023** | 2.50 MB | `add9e09f2d27b3d71266b8201464918f` | Factory Binary Firmware Dump |
| `SIM2K-250_606X1A6K00000_Original.bin` | **2016–2023** | 2.50 MB | `29c2c818ad4445dcb7de23e78c42b35a` | Factory Binary Firmware Dump |
| `SIM2K-250_606Y0B4000000_GCC_FuelQuality.bin` | **2016–2023** | 2.50 MB | `6036437e1879c1a287fcccce4ab106c7` | Factory Binary Firmware Dump |
| `SIM2K-250_606Y0B4000000_Original.bin` | **2016–2023** | 2.50 MB | `9968fd8cba6e5e3accbdb828a2ca7fc2` | Factory Binary Firmware Dump |
| `SIM2K-250_606Z0D5K00000_GCC_FuelQuality.bin` | **2016–2023** | 2.50 MB | `f1af1aed8760958b1168697b0bf44642` | Factory Binary Firmware Dump |
| `SIM2K-250_606Z0D5K00000_Original.bin` | **2016–2023** | 2.50 MB | `bfac155aee17f2d6724503eff2644e37` | Factory Binary Firmware Dump |
| `SIM2K-250_6H6N090000000_GCC_FuelQuality.bin` | **2016–2023** | 2.50 MB | `64664ffc449ed904d8e873da6cbb4417` | Factory Binary Firmware Dump |
| `SIM2K-250_6H6N090000000_Original.bin` | **2016–2023** | 2.50 MB | `0c03a7d1d42ada2d965311539730b53f` | Factory Binary Firmware Dump |

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
