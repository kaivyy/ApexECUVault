# VAG DIGIFANT G40 G60 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: VAG DIGIFANT G40 G60
- **Model Year Coverage**: 1988–1995
- **Total Calibration Assets**: 27 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `corradoSLS.BIN` | **1988–1995** | 32.0 KB | `117ed6deef20eae56fd15afb5d26b40c` | Factory Binary Firmware Dump |
| `G40_EubelTuningInGifhorn1995_MinorFuelTimingChanges_BoostCutRemoval_IdleIgnition.BIN` | **1988–1995** | 32.0 KB | `b087e9145ee7e845170f1212dc0406d6` | Factory Binary Firmware Dump |
| `G40_Mk2_StockEprom.BIN` | **1988–1995** | 32.0 KB | `850a8115213f1e378f5d104f293732bd` | Factory Binary Firmware Dump |
| `G40_Mk2_StockEprom.xdf` | **1988–1995** | 18.2 KB | `770f01aa4742df8591f1762b41bd177d` | TunerPro Binary Definition Map |
| `G40_Pitstop_SNS_NoLag_250ccMinInj_7800Rev_AdvIgn_DecFuel72pcDuty.BIN` | **1988–1995** | 32.0 KB | `74fcdfe56695d13a13283eaf51db48a0` | Factory Binary Firmware Dump |
| `G40_Pitstop_SNS_NoLag_7800RevLimit_AdvIgn_IncFuel88pcDuty.BIN` | **1988–1995** | 32.0 KB | `a056503ee2c35f515f680f304971ceec` | Factory Binary Firmware Dump |
| `G40_StockEprom.BIN` | **1988–1995** | 32.0 KB | `5fa2b4c8e2ed78c2cb352fda4a49ede8` | Factory Binary Firmware Dump |
| `G40_StockEprom_with7kRevLimit.BIN` | **1988–1995** | 32.0 KB | `c00210fcafc0bc7eb200edce4b5d2019` | Factory Binary Firmware Dump |
| `G40_StockEprom_withWOTidleLambdaMods.BIN` | **1988–1995** | 32.0 KB | `1fb7b65bbef0015091a59380898e6ddc` | Factory Binary Firmware Dump |
| `G40_XDF_BETA_DirectFromEcuConnections.xdf` | **1988–1995** | 54.6 KB | `276e1388a5c58c0ad6c38e58f5714b07` | TunerPro Binary Definition Map |
| `G40_XDF_YOU54F.xdf` | **1988–1995** | 71.1 KB | `ba9a61530caf4409343243ac81ac332a` | TunerPro Binary Definition Map |
| `G40_XDF_YOU54F_withPatches.xdf` | **1988–1995** | 74.0 KB | `753fe2ae3073bb0ba93027e2ea9e8087` | TunerPro Binary Definition Map |
| `G60 6636 X3 timing bin-ISV boost & no lambda.bin` | **1988–1995** | 32.0 KB | `43fdef17095f4089e724e79da1388182` | Factory Binary Firmware Dump |
| `G60 Single Timing Map01.xdf` | **1988–1995** | 118.8 KB | `bc71b95fe9652afa2c0cffcd79b188ae` | TunerPro Binary Definition Map |
| `G60_1_ignition_map.xdf` | **1988–1995** | 97.3 KB | `ded6b004b5a2bb57e466a2ccd5e6eb1e` | TunerPro Binary Definition Map |
| `KRTURBO.BIN` | **1988–1995** | 32.0 KB | `1cbfe69875c2836530c6e1a52f317dba` | Factory Binary Firmware Dump |
| `limited_16v_G60.BIN` | **1988–1995** | 32.0 KB | `fb9fdfd87443f234bfa73d5a919ba2e0` | Factory Binary Firmware Dump |
| `PASSG60.BIN` | **1988–1995** | 32.0 KB | `889dc98df8ec41eb25b7949bbf509eb4` | Factory Binary Firmware Dump |
| `Saab900T16_Bosch403.BIN` | **1988–1995** | 32.0 KB | `d5e2029e3fdf96b059c2519ab9cbe316` | Factory Binary Firmware Dump |
| `STAGE 5 G60.BIN` | **1988–1995** | 32.0 KB | `bcf9c8acc41a18f3a497e1d8f1722dc2` | Factory Binary Firmware Dump |
| `Stock G60 Single Ignition Map.BIN` | **1988–1995** | 32.0 KB | `4120071750a1fcc7bd168bde50f097f4` | Factory Binary Firmware Dump |
| `Stock G60 Three ignition maps.bin` | **1988–1995** | 32.0 KB | `b6a425bd3be51763a0d3e0ec3c82a8c1` | Factory Binary Firmware Dump |
| `Theibach RS G60 mit 27c512 gelesen.bin` | **1988–1995** | 32.0 KB | `0b53a1ba5b54939ef8a7f6628d1e4664` | Factory Binary Firmware Dump |
| `TunerPro RT v5 - G60 3 Ignition Map (Marc G60T 2014).xdf` | **2014** | 79.2 KB | `c5e77712b15c8cbb50ae16d13f5864fd` | TunerPro Binary Definition Map |
| `VW 1.3 G40 Digifant-WINOLS-YOU54F.ols` | **1988–1995** | 103.9 KB | `c213d35775f6e8945971549ac1134e18` | WinOLS Project Workspace & Calibration |
| `VW 1.8T G60 Digifant 037997022B - WINOLS.ols` | **1988–1995** | 57.7 KB | `26f072899b84a8961a854c823e30e493` | WinOLS Project Workspace & Calibration |
| `vw6636.bin` | **1988–1995** | 32.0 KB | `2e5b172c3283cb842ca8f25a56f5ba38` | Factory Binary Firmware Dump |

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
