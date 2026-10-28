# SUBARU 5EAT TRANSMISSION - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SUBARU 5EAT TRANSMISSION
- **Model Year Coverage**: 2004–2014
- **Total Calibration Assets**: 29 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `5AT_3.272_LEGAS_EJDM2008.bin` | **2004–2014** | 1.00 MB | `51e1b9ed0e72938573fe6c4c2fedb74e` | Factory Binary Firmware Dump |
| `5AT_3.583_LEGASE_JDM2008.bin` | **2004–2014** | 1.00 MB | `05fe405c9fe39c7c1484adcd11155be6` | Factory Binary Firmware Dump |
| `5EAT_ADE0236000.bin` | **2004–2014** | 512.0 KB | `afdf6cbc3f44987a43f5a2dc6b5bc313` | Factory Binary Firmware Dump |
| `5eat_tcu_denso_romraider_defs.xml` | **2004–2014** | 2.24 MB | `113bebbd405e3c8f28ee18e609c44378` | EcuFlash / RomRaider XML Definition |
| `5eat_tcu_logger.xml` | **2004–2014** | 45.4 KB | `5037f152a7321fbbe8f81952d1cb6145` | EcuFlash / RomRaider XML Definition |
| `5eat_tcu_romraider_defs.xml` | **2004–2014** | 5.66 MB | `16ef133d34b9ed9642c2057a57da18c9` | EcuFlash / RomRaider XML Definition |
| `8AF0237300_MB500NJ0VF32C_2006_TRIBECA_USDM.bin` | **2004–2014** | 512.0 KB | `825cc624a601a89d95e2d95c4e477e70` | Factory Binary Firmware Dump |
| `8EFB206000_08FB2WA0_14_tribeca_usdm.bin` | **2004–2014** | 1.00 MB | `f67520400d791d3dd91bfa79568f14f5` | Factory Binary Firmware Dump |
| `91A0217300_MB4365.bin` | **2004–2014** | 384.0 KB | `dfb7bcc281f984f06c24e280d5974c1b` | Factory Binary Firmware Dump |
| `91A0217400_MB4372_A61022.bin` | **2004–2014** | 512.0 KB | `2c5a2360d6474a3428d90cb8b5aa1751` | Factory Binary Firmware Dump |
| `91A1207300_MB4364.bin` | **2004–2014** | 384.0 KB | `7834b35a6c25ecf96cde7321f3b14df2` | Factory Binary Firmware Dump |
| `91D0207500_MB436T_AH572_5EAT_JDM.bin` | **2004–2014** | 384.0 KB | `0f3e2c9db853b656918440c425e8c80c` | Factory Binary Firmware Dump |
| `91D1206000_5EAT.bin` | **2004–2014** | 384.0 KB | `b0f1f9c7c65657570bc70bfdbb42cbd8` | Factory Binary Firmware Dump |
| `91F0217100_MB436P_AG810_OBK03USDM.bin` | **2004–2014** | 384.0 KB | `8bd88dfde570bb07032ed429ecacb475` | Factory Binary Firmware Dump |
| `91FE207100_MB436L_AG802_5EAT_LGT05USDM.bin` | **2004–2014** | 384.0 KB | `cf82058608e4718e175b416f68985f7d` | Factory Binary Firmware Dump |
| `91FE216300.bin` | **2004–2014** | 512.0 KB | `104888b35ae076e2ad215dad688fac8f` | Factory Binary Firmware Dump |
| `[91D1207900-A61022]_31711AG589.bin` | **2004–2014** | 384.0 KB | `09764d513b8e9d39c662ba586a137d71` | Factory Binary Firmware Dump |
| `[AAD1A07100-A61022]_31711AJ782.bin` | **2004–2014** | 384.0 KB | `72760d6006e21fb9b87e651b27168393` | Factory Binary Firmware Dump |
| `[ABD1207000-A61022].bin` | **2004–2014** | 384.0 KB | `1e37115dee4255c99b2b3918159f884a` | Factory Binary Firmware Dump |
| `AAD1A06000.bin` | **2004–2014** | 512.0 KB | `49afb305231252504b713d3ed9aa344c` | Factory Binary Firmware Dump |
| `ABD1A03100_A61022_LGT_JDM_2005_5EAT.bin` | **2004–2014** | 384.0 KB | `e4637da77d0e2fe1a434554866264696` | Factory Binary Firmware Dump |
| `ACD1207000_MB558D01_LGT06_JDM.bin` | **2004–2014** | 512.0 KB | `74fbae3aca373c955c7f6e348ec68904` | Factory Binary Firmware Dump |
| `ACD1A06000_JDM_5EAT_2007_M32176F4V.bin` | **2004–2014** | 512.0 KB | `439c4c3d3e5e9a0dd0841ec7c6ed8dae` | Factory Binary Firmware Dump |
| `B1AE207100_EZAE2WB1_2010_LGT_EDM.bin` | **2004–2014** | 1.00 MB | `52c1f1fd2fea4a230035e9ed4051f887` | Factory Binary Firmware Dump |
| `Forester_SH9_STI_3.283_JDM2010.bin` | **2004–2014** | 1.00 MB | `453872ab890176fd6198bc1163620f20` | Factory Binary Firmware Dump |
| `Impreza_STI_3.583_JDM2011.bin` | **2004–2014** | 1.00 MB | `c7eb900692734f0174e964d7eb305ca0` | Factory Binary Firmware Dump |
| `SH7058S-3171121010_STI.bin` | **2004–2014** | 1.00 MB | `fc492e13db2ee78b54f0a7601724167d` | Factory Binary Firmware Dump |
| `SH7058S_TG5_3.083.bin` | **2004–2014** | 1.00 MB | `9abc6f3a7c8a428e5a9ba79f3f7fafc2` | Factory Binary Firmware Dump |
| `Tribeca_3.583_EDM_2009.bin` | **2004–2014** | 1.00 MB | `bc566b8311fb7cf26e40e28dec3e58f7` | Factory Binary Firmware Dump |

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
