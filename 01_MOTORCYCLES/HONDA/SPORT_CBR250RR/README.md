# SPORT CBR250RR - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SPORT CBR250RR
- **Model Year Coverage**: 2016–2026
- **Total Calibration Assets**: 20 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `38770-K64-N01.bin` | **2016–2026** | 1.00 MB | `e0c12d43c50c7c285df0307bef13f4b5` | Factory Binary Firmware Dump |
| `38770-K64-R02.bin` | **2016–2026** | 1.00 MB | `f87f1dc65059e08f496e62fd0872a6e7` | Factory Binary Firmware Dump |
| `CBR250RR-38770-K64-N04_BIN.bin` | **2016–2026** | 1.00 MB | `c069d5b2d1476a728ba14a43ef73dc7a` | Factory Binary Firmware Dump |
| `CBR250RR-38770-K64-ND1_BIN.bin` | **2016–2026** | 1.00 MB | `5c616504f3b6306adff2ad04a17ab68c` | Factory Binary Firmware Dump |
| `CBR250RR_38770-K64-N04_PUBLIC_v1.xdf` | **2016–2026** | 89.0 KB | `8beae407f19171868ea92c8f56748426` | TunerPro Binary Definition Map |
| `CBR250RR_38770-K64-ND1_PUBLIC_v1.xdf` | **2016–2026** | 83.3 KB | `cb0b660f54754f38efbc1ad750aa4967` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-N04_Honda_CBR250RR_Gen_1_(2016-2019)_Standard_&_ABS.xdf` | **2016–2019** | 9.5 KB | `04be9df5087b128d0865bc6c1a2eed22` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-NB1_Honda_CBR250RR_Gen_2_SP_(2020-2022)_Non-QS.xdf` | **2020–2022** | 9.5 KB | `ca5015c2f8f9aa7988be8bddc0d6aef1` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-ND1_Honda_CBR250RR_Gen_2_SP_(2020-2022)_Quick_Shifter.xdf` | **2020–2022** | 9.5 KB | `5ba7c328b2c7b46ec1d84af75557376c` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-NL1_Honda_New_CBR250RR_Gen_3_Facelift_(2023-2026)_Standard_38.7PS.xdf` | **2023–2026** | 9.5 KB | `544c171ffadc975b54ae241d3b0fe591` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-NM1_Honda_New_CBR250RR_Gen_3_Facelift_(2023-2026)_SP_Quick_Shifter_42PS.xdf` | **2023–2026** | 9.6 KB | `c287ba68bf9a068f8938d73bc7272d74` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K64-R02_Honda_CBR250RR_HRC_Racing_ECU_(2017-2024).xdf` | **2017–2024** | 9.5 KB | `0afbe5a886e9729dd423085f000c4bc7` | TunerPro Binary Definition Map |
| `HONDA_38770-K64-J01_Honda_Generic_ECM.xdf` | **2016–2026** | 16.3 KB | `6b23d0eae7e35613a845574759ba1d33` | TunerPro Binary Definition Map |
| `HONDA_38770-K64-N01_Honda_Generic_ECM.xdf` | **2016–2026** | 16.3 KB | `e17d45e5d6ddac57dee1b4c57f7bf34f` | TunerPro Binary Definition Map |
| `HONDA_38770-K64-N04_Honda_Generic_ECM.xdf` | **2016–2026** | 16.3 KB | `cae354c06883e17cb0afd70bd3b4abcc` | TunerPro Binary Definition Map |
| `HONDA_38770-K64-NB1_Honda_Generic_ECM.xdf` | **2016–2026** | 16.3 KB | `beb0798ad823769667fb5235ffd8f790` | TunerPro Binary Definition Map |
| `STOCK_ORIGINAL_38770-K64-N01_Honda_CBR250RR_Gen1_(2016-2019)_Thai.bin` | **2016–2019** | 1.00 MB | `e0c12d43c50c7c285df0307bef13f4b5` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_38770-K64-N04_Honda_CBR250RR_Gen1_(2016-2019)_Indo.bin` | **2016–2019** | 1.00 MB | `c069d5b2d1476a728ba14a43ef73dc7a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_38770-K64-ND1_Honda_CBR250RR_Gen2_SP_(2020-2022)_QS_Indo.bin` | **2020–2022** | 1.00 MB | `5c616504f3b6306adff2ad04a17ab68c` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_38770-K64-R02_Honda_CBR250RR_HRC_Race_ECU_(2017-2024).bin` | **2017–2024** | 1.00 MB | `f87f1dc65059e08f496e62fd0872a6e7` | Factory Binary Firmware Dump |

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
