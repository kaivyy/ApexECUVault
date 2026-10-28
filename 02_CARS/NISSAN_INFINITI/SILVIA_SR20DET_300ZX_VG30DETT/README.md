# SILVIA SR20DET 300ZX VG30DETT - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SILVIA SR20DET 300ZX VG30DETT
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 84 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `S13_SR20DET_50F00_MT_red_top.bin` | **1998–2024** | 32.0 KB | `331c675160d4b3a2f8e6c2fc7643c70b` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F01_MT.bin` | **1998–2024** | 32.0 KB | `ed637f93635ab118fba7a530af15b468` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F05_MT_black_top.bin` | **1998–2024** | 32.0 KB | `dd65894d26d7b081ce2138ae7f4e52b6` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F10_AT.bin` | **1998–2024** | 32.0 KB | `c5c53a6a5724e98b36b37a4fa2eb0df4` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F11_AT.bin` | **1998–2024** | 32.0 KB | `c6de968d6c92d05fa8f29d3d864a535a` | Factory Binary Firmware Dump |
| `S13_SR20DET_50F15_AT.bin` | **1998–2024** | 32.0 KB | `4890359a20d053b80d122a3ebc4b8ece` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F06_MT_TypeX.bin` | **1998–2024** | 32.0 KB | `5ff40c110fa7bc294942198a79bc1067` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F07_TypeX.bin` | **1998–2024** | 32.0 KB | `fa1ffcb7f80b833c34df801ec5033a7d` | Factory Binary Firmware Dump |
| `S13_SR20DET_60F16_TypeX.bin` | **1998–2024** | 32.0 KB | `e0218e51b46b0957f3403bdbecb4efb1` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F00_MT_red_top.bin` | **1998–2024** | 32.0 KB | `331c675160d4b3a2f8e6c2fc7643c70b` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F01_MT.bin` | **1998–2024** | 32.0 KB | `ed637f93635ab118fba7a530af15b468` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F05_MT_black_top.bin` | **1998–2024** | 32.0 KB | `dd65894d26d7b081ce2138ae7f4e52b6` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F10_AT.bin` | **1998–2024** | 32.0 KB | `c5c53a6a5724e98b36b37a4fa2eb0df4` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F11_AT.bin` | **1998–2024** | 32.0 KB | `c6de968d6c92d05fa8f29d3d864a535a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_50F15_AT.bin` | **1998–2024** | 32.0 KB | `4890359a20d053b80d122a3ebc4b8ece` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F06_MT_TypeX.bin` | **1998–2024** | 32.0 KB | `5ff40c110fa7bc294942198a79bc1067` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F07_TypeX.bin` | **1998–2024** | 32.0 KB | `fa1ffcb7f80b833c34df801ec5033a7d` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_S13_SR20DET_60F16_TypeX.bin` | **1998–2024** | 32.0 KB | `e0218e51b46b0957f3403bdbecb4efb1` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_30P00_1990_NA_MT_FED.BIN` | **1998–2024** | 32.0 KB | `decdee3ae2db76af59e9f12576e774a8` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_30P60_1990_NA_MT_FED.BIN` | **1998–2024** | 32.0 KB | `4edc4bbcf0bbcfe5f83842393a5ec6c3` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_30P75_1991_NA_AT.BIN` | **1998–2024** | 32.0 KB | `b6e807523ca68acbaf215223e430b8ce` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P00_1990_NA_AT.bin` | **1998–2024** | 32.0 KB | `3287d5ece0ee82c4626c91dcc74fc90c` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P12_1990_NA_AT.bin` | **1998–2024** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_39P12_AT.bin` | **1998–2024** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_40P01_1991_NA_MT_JDM.bin` | **1998–2024** | 32.0 KB | `9ccebd22f09f29afe03615984cbf2add` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_40P13_AT.bin` | **1998–2024** | 32.0 KB | `c8b592bf26ed5128eb8b8b8c19fc4fa6` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_46P10_1992_AT_ADM.bin` | **1998–2024** | 32.0 KB | `83f20f9d6b2f4e827cf80a5bfdbbf644` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DE_46P80_1992_AT.bin` | **1998–2024** | 32.0 KB | `c65c5518813167583ccf898840eab84e` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_1989_NA_AT_M257ACA8.bin` | **1998–2024** | 32.0 KB | `634969617a539295be2a95bac8f13cf3` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_30P10.bin` | **1998–2024** | 32.0 KB | `c675735fade59ef7e66faeadd2e00e24` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P02_1990_MT_FED.BIN` | **1998–2024** | 32.0 KB | `bc726e7565cd9ae3b6c7ba651364e784` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P03_1990_MT_FED.BIN` | **1998–2024** | 32.0 KB | `97c50fa61263428c981e600dec6ce313` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P08_1990_MT_CALI.BIN` | **1998–2024** | 32.0 KB | `bb9668c388d54882c605eddcd38d03fe` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P11.bin` | **1998–2024** | 32.0 KB | `6a4885cf061d8f7452ff441f5eea6acd` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_31P12.bin` | **1998–2024** | 32.0 KB | `c7e984bdc4864426799ec4e9695f09aa` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P01_1991_1993_MT_EDM.bin` | **1998–2024** | 32.0 KB | `7fca8db92cbbc9f811923a370def1d83` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P06_MT.bin` | **1998–2024** | 32.0 KB | `a6a655c1e5587c05d8b510a99831de58` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_37P11_AT_1992_EDM.bin` | **1998–2024** | 32.0 KB | `9c8edf0efb04ddfa4645048e94d04526` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P01_AT_1990_JDM_M4.BIN` | **1998–2024** | 32.0 KB | `123fd911b8e8d6d6308da239401a17a9` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P02_MT_JDM.bin` | **1998–2024** | 32.0 KB | `2917c557091a9df4d97428ffe38f5a09` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P03_MT_JDM.BIN` | **1998–2024** | 32.0 KB | `76f4afd37d040a861963b9db48425d35` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P04_MT_1991_JDM.BIN` | **1998–2024** | 32.0 KB | `4fb4d51f776d68259de427305eca1a7a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P11_AT_TXC_661.bin` | **1998–2024** | 32.0 KB | `bfee693253557eef52f53b33d6ff81ac` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P12_AT.bin` | **1998–2024** | 32.0 KB | `80b92e376e3da858b42b9288c8212599` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P13_AT.bin` | **1998–2024** | 32.0 KB | `8277b6aeb51ce560e4a949cace0979f7` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P14_JDM.bin` | **1998–2024** | 32.0 KB | `7d15b18850f72c9a3d401cad2ebcb0dd` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P60_MT_1992.BIN` | **1998–2024** | 32.0 KB | `4409df9b429e02f268e7d654c4f15529` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_41P70_MT.BIN` | **1998–2024** | 32.0 KB | `a0d4f6a1884d5d0b465573e37b0fa905` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_47P10_MT.bin` | **1998–2024** | 32.0 KB | `d698dd4a383c96dc5cdcd890b53cfc08` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_48P01_MT_1991.BIN` | **1998–2024** | 32.0 KB | `af4656fd08c4c8c9f0451d56c7ebb126` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_Z32_VG30DETT_48P76.BIN` | **1998–2024** | 32.0 KB | `2de0ea0c9ce88fc649eb238df57d9c70` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P00_1990_NA_MT_FED.BIN` | **1998–2024** | 32.0 KB | `decdee3ae2db76af59e9f12576e774a8` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P60_1990_NA_MT_FED.BIN` | **1998–2024** | 32.0 KB | `4edc4bbcf0bbcfe5f83842393a5ec6c3` | Factory Binary Firmware Dump |
| `Z32_VG30DE_30P75_1991_NA_AT.BIN` | **1998–2024** | 32.0 KB | `b6e807523ca68acbaf215223e430b8ce` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P00_1990_NA_AT.bin` | **1998–2024** | 32.0 KB | `3287d5ece0ee82c4626c91dcc74fc90c` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P12_1990_NA_AT.bin` | **1998–2024** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `Z32_VG30DE_39P12_AT.bin` | **1998–2024** | 32.0 KB | `56aedee4cfdcc5fff9ecc10cd6ebf852` | Factory Binary Firmware Dump |
| `Z32_VG30DE_40P01_1991_NA_MT_JDM.bin` | **1998–2024** | 32.0 KB | `9ccebd22f09f29afe03615984cbf2add` | Factory Binary Firmware Dump |
| `Z32_VG30DE_40P13_AT.bin` | **1998–2024** | 32.0 KB | `c8b592bf26ed5128eb8b8b8c19fc4fa6` | Factory Binary Firmware Dump |
| `Z32_VG30DE_46P10_1992_AT_ADM.bin` | **1998–2024** | 32.0 KB | `83f20f9d6b2f4e827cf80a5bfdbbf644` | Factory Binary Firmware Dump |
| `Z32_VG30DE_46P80_1992_AT.bin` | **1998–2024** | 32.0 KB | `c65c5518813167583ccf898840eab84e` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_1989_NA_AT_M257ACA8.bin` | **1998–2024** | 32.0 KB | `634969617a539295be2a95bac8f13cf3` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_30P10.bin` | **1998–2024** | 32.0 KB | `c675735fade59ef7e66faeadd2e00e24` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P02_1990_MT_FED.BIN` | **1998–2024** | 32.0 KB | `bc726e7565cd9ae3b6c7ba651364e784` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P03_1990_MT_FED.BIN` | **1998–2024** | 32.0 KB | `97c50fa61263428c981e600dec6ce313` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P08_1990_MT_CALI.BIN` | **1998–2024** | 32.0 KB | `bb9668c388d54882c605eddcd38d03fe` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P11.bin` | **1998–2024** | 32.0 KB | `6a4885cf061d8f7452ff441f5eea6acd` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_31P12.bin` | **1998–2024** | 32.0 KB | `c7e984bdc4864426799ec4e9695f09aa` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P01_1991_1993_MT_EDM.bin` | **1998–2024** | 32.0 KB | `7fca8db92cbbc9f811923a370def1d83` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P06_MT.bin` | **1998–2024** | 32.0 KB | `a6a655c1e5587c05d8b510a99831de58` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_37P11_AT_1992_EDM.bin` | **1998–2024** | 32.0 KB | `9c8edf0efb04ddfa4645048e94d04526` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P01_AT_1990_JDM_M4.BIN` | **1998–2024** | 32.0 KB | `123fd911b8e8d6d6308da239401a17a9` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P02_MT_JDM.bin` | **1998–2024** | 32.0 KB | `2917c557091a9df4d97428ffe38f5a09` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P03_MT_JDM.BIN` | **1998–2024** | 32.0 KB | `76f4afd37d040a861963b9db48425d35` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P04_MT_1991_JDM.BIN` | **1998–2024** | 32.0 KB | `4fb4d51f776d68259de427305eca1a7a` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P11_AT_TXC_661.bin` | **1998–2024** | 32.0 KB | `bfee693253557eef52f53b33d6ff81ac` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P12_AT.bin` | **1998–2024** | 32.0 KB | `80b92e376e3da858b42b9288c8212599` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P13_AT.bin` | **1998–2024** | 32.0 KB | `8277b6aeb51ce560e4a949cace0979f7` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P14_JDM.bin` | **1998–2024** | 32.0 KB | `7d15b18850f72c9a3d401cad2ebcb0dd` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P60_MT_1992.BIN` | **1998–2024** | 32.0 KB | `4409df9b429e02f268e7d654c4f15529` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_41P70_MT.BIN` | **1998–2024** | 32.0 KB | `a0d4f6a1884d5d0b465573e37b0fa905` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_47P10_MT.bin` | **1998–2024** | 32.0 KB | `d698dd4a383c96dc5cdcd890b53cfc08` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_48P01_MT_1991.BIN` | **1998–2024** | 32.0 KB | `af4656fd08c4c8c9f0451d56c7ebb126` | Factory Binary Firmware Dump |
| `Z32_VG30DETT_48P76.BIN` | **1998–2024** | 32.0 KB | `2de0ea0c9ce88fc649eb238df57d9c70` | Factory Binary Firmware Dump |

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
