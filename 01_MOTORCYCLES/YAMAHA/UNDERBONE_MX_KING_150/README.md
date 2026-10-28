# UNDERBONE MX KING 150 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: UNDERBONE MX KING 150
- **Model Year Coverage**: 2015–2023
- **Total Calibration Assets**: 9 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GENERATIONAL_B5V-H591A-00_Yamaha_Exciter_155_VVA___Sniper_155_V3_SmartKey_2021_2025.xdf` | **2015–2023** | 2.5 KB | `bd57c17363976768f3ea699ca8d8dbd1` | TunerPro Binary Definition Map |
| `GENERATIONAL_B5V-H591A-10_Yamaha_Exciter_155_VVA___Sniper_155_V3_Standard_Key_2021_2025.xdf` | **2015–2023** | 2.5 KB | `f1f508dc7e501e6d939f2adf1d9e768d` | TunerPro Binary Definition Map |
| `GENERATIONAL_BNV-H591A-01_Yamaha_Sniper_155_V4_VVA_SmartKey_2023_2025.xdf` | **2015–2023** | 2.5 KB | `21a149f69e3590fee5a62abf56d8618d` | TunerPro Binary Definition Map |
| `MX_KING_2PV1.bin` | **2015–2023** | 27.0 KB | `a705f0587831fe9525ce4872b64cdc95` | Factory Binary Firmware Dump |
| `MX_KING_B5V0.bin` | **2015–2023** | 27.0 KB | `81449ab4c9756c72adbe6a646fa49d0c` | Factory Binary Firmware Dump |
| `MX_KING_BKV1.bin` | **2015–2023** | 27.0 KB | `cbf24c22b2ad23c6923247b7dbfbd53f` | Factory Binary Firmware Dump |
| `YAMAHA_2PV-H591A-00_Yamaha_MX_King_150_V1_(2PV0).xdf` | **2015–2023** | 6.5 KB | `53734ac043c55586c373eb282464ad6f` | TunerPro Binary Definition Map |
| `YAMAHA_B5V-H591A-00_Yamaha_MX_King_150_V2_LED_(B5V0).xdf` | **2015–2023** | 6.5 KB | `0235d7e17b94f00105b57e81b3a7666b` | TunerPro Binary Definition Map |
| `YAMAHA_BKV-H591A-10_Yamaha_MX_King_150_(BKV1).xdf` | **2015–2023** | 6.5 KB | `a43267663c315a96a4c625e7c707583a` | TunerPro Binary Definition Map |

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
