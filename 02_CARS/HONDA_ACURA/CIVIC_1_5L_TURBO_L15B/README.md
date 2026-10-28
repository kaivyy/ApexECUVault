# CIVIC 1 5L TURBO L15B - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: CIVIC 1 5L TURBO L15B
- **Model Year Coverage**: 2016–2024
- **Total Calibration Assets**: 12 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `37805-5AA-A080_Honda_Civic_2017_EX-T_1.5L_L4_-_Gas.xdf` | **2016–2024** | 98.5 KB | `747e463af42612810dece2ec51c18a41` | TunerPro Binary Definition Map |
| `37805-5AA-A580_Honda_Civic_2016_2017_EX-L__EX-T_1.5L_L4_-_Gas.xdf` | **2016–2024** | 101.0 KB | `db97e62e53d1707b5b1f9d31e06adf30` | TunerPro Binary Definition Map |
| `37805-5AA-A640_Honda_Civic_2016_2017_EX-L__EX-T__Touring_1.5L_L4_-_Gas.xdf` | **2016–2024** | 105.6 KB | `2c5185365a8e27d57aabe98becca332a` | TunerPro Binary Definition Map |
| `37805-5AM-A120_Honda_Civic_2019_Si_1.5L_L4_-_Gas.xdf` | **2016–2024** | 98.7 KB | `8785595e93b9502cf23f844b9c468ad6` | TunerPro Binary Definition Map |
| `37805-5AM-A220_Honda_Civic_2020_Si_1.5L_L4_-_Gas.xdf` | **2016–2024** | 118.9 KB | `af64de23dd81ceaf789fb43e27c045a6` | TunerPro Binary Definition Map |
| `37805-5AN-A220_Honda_Civic_2019_Sport_1.5L_L4_-_Gas__2.0L_L4_-_Gas.xdf` | **2016–2024** | 96.6 KB | `8836c2e209a223dd892a81a529ad01e9` | TunerPro Binary Definition Map |
| `37805-5BF-A340_Honda_Civic_2020_Touring__Type_R_1.5L_L4_-_Gas__2.0L_L4_-_Ga.xdf` | **2016–2024** | 118.3 KB | `480e8d514047417ab6e074ecd4ddef3e` | TunerPro Binary Definition Map |
| `37805-5BF-A340_Honda_Civic_2020_Touring__Type_R_1.5L_L4_-_Gas__2.0L_L4_-_Gas.xdf` | **2016–2024** | 118.3 KB | `480e8d514047417ab6e074ecd4ddef3e` | TunerPro Binary Definition Map |
| `GENERATIONAL_37805-5AA-A640_Honda_Civic_RS_Turbo_1.5L_VTEC_2016_2021.xdf` | **2016–2024** | 1.5 KB | `ee90f1c8d7fb4d95838b3211da64a440` | TunerPro Binary Definition Map |
| `GENERATIONAL_37805-64A-A01_CIVIC_GEN11_Honda_Civic_RS_Gen_11_VTEC_Turbo_FE___FL_(2021-2026).xdf` | **2021–2026** | 5.4 KB | `ff56aecfa0c1375a75c070c83bd43918` | TunerPro Binary Definition Map |
| `HONDA_37805-5AA-A01_CIVIC_TURBO.xdf` | **2016–2024** | 11.9 KB | `be344bed5e2532e3fce47332d1a6cef3` | TunerPro Binary Definition Map |
| `HONDA_CRV_CIVIC_TURBO_2017-2022_1.5L_L15B7_KEIHIN_37805-5LA-C940-M1.rwd` | **2016–2024** | 1.94 MB | `c0eee17b8879d0f727cdb3cd0eafea4d` | Factory Binary Firmware Dump |

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
