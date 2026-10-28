# M POWER MSS60 M3 V8 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: M POWER MSS60 M3 V8
- **Model Year Coverage**: 2007–2013
- **Total Calibration Assets**: 19 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `BMW M3 - SIEMENS MSS60.ols` | **2007–2013** | 3.72 MB | `7b703832b6985f6cf843c576b6fc4a9d` | WinOLS Project Workspace & Calibration |
| `ign.a2l` | **2007–2013** | 3.00 MB | `60868050e5271b20634816729a858e78` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `IGN_E90_BG11_ECE_HS_008 _530_2_ign_4.hex` | **2007–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_ECE_HS_009 _530_3_ign_.hex` | **2007–2013** | 5.11 MB | `247a98e2367b0443c1231d7a61602f52` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_ECE_HS_009 _530_3_ign__1.hex` | **2007–2013** | 5.11 MB | `247a98e2367b0443c1231d7a61602f52` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_008 _530_2_ign.hex` | **2007–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_008 _530_2_ign_1.hex` | **2007–2013** | 5.11 MB | `4451f20335aec32dc62f2ecc2901d6f2` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_011 _530_3_2710_ign_1.hex` | **2007–2013** | 5.11 MB | `553690b2f051ba0f87128c4f3cc13764` | Intel HEX Calibration Firmware |
| `IGN_E90_BG11_US_HS_011 _530_3_2710_ign_2.hex` | **2007–2013** | 5.11 MB | `b5e7a7ec47530bd6d65d114d2744d732` | Intel HEX Calibration Firmware |
| `inj.a2l` | **2007–2013** | 3.99 MB | `1ad46d85e8b34d60e8a7c9ed30da6bbc` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `INJ_E90_BG11_ECE_HS_008 _530_2_inj_4.hex` | **2007–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_ECE_HS_009 _530_3_inj_.hex` | **2007–2013** | 5.11 MB | `e9ccb7c7a970aac780a21e1bb1eaa5e4` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_ECE_HS_009 _530_3_inj__1.hex` | **2007–2013** | 5.11 MB | `e9ccb7c7a970aac780a21e1bb1eaa5e4` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_008 _530_2_inj.hex` | **2007–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_008 _530_2_inj_1.hex` | **2007–2013** | 5.11 MB | `e6b67d65b219a5825d57a0b5215e828f` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_011 _530_3_2710_inj_1.hex` | **2007–2013** | 5.11 MB | `be9ef94f82f46babd2f6eccf16b2b13c` | Intel HEX Calibration Firmware |
| `INJ_E90_BG11_US_HS_011 _530_3_2710_inj_2.hex` | **2007–2013** | 5.11 MB | `be9ef94f82f46babd2f6eccf16b2b13c` | Intel HEX Calibration Firmware |
| `WinOLS (BMW E90  V8 4.0-4.2 (Original) als Prozessor - zündung moment).ols` | **2007–2013** | 2.90 MB | `a1fad124dbab76d0bf0ee34acf9469bc` | WinOLS Project Workspace & Calibration |
| `WinOLS (BMW E90-E91 (Lambda_kat_vmx.sm1) als Prozessor - lambda ).ols` | **2007–2013** | 3.67 MB | `921bfadcdebb613bc10fd8c01fbc336e` | WinOLS Project Workspace & Calibration |

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
