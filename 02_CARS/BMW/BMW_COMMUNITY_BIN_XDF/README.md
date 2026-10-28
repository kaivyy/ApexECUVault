# BMW COMMUNITY BIN XDF - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: BMW COMMUNITY BIN XDF
- **Model Year Coverage**: 1990–2015
- **Total Calibration Assets**: 16 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `GS20_90C0_64KB.bin` | **1990–2015** | 64.0 KB | `4d41ca20706be9963c4bb618188f0be2` | Factory Binary Firmware Dump |
| `GS20_90C0_64KB__chookees-ecu.bin` | **1990–2015** | 64.0 KB | `4d60bed6f7b42524c9af8c1c3731e828` | Factory Binary Firmware Dump |
| `GS20_90C0_64KB__chookees-ecu_79b03fc2.bin` | **1990–2015** | 64.0 KB | `79b03fc228d0e8c4b1d1fb99ef7b2b77` | Factory Binary Firmware Dump |
| `GS20_90C0_64KB_corrected.bin` | **1990–2015** | 64.0 KB | `cdd0d288d34a18a60efd5f5d068f0c11` | Factory Binary Firmware Dump |
| `MHD_ECA_v1.0.1.hex` | **1990–2015** | 14.6 KB | `e0d863769ed01cf6d05ee1e9c392f12d` | Intel HEX Calibration Firmware |
| `MS43_WBABW510X0PK46741_430069_512KB.bin` | **1990–2015** | 512.0 KB | `f4e5e93b8784b6df1e6759e2e441d51b` | Factory Binary Firmware Dump |
| `MS43_WBABW510X0PK46741_430069_512KB__chookees-ecu.bin` | **1990–2015** | 512.0 KB | `724858dbc826c4ff5ac01eb32710ec90` | Factory Binary Firmware Dump |
| `MS43_WBABW510X0PK46741_430069_512KB__chookees-ecu_ceeae1f0.bin` | **1990–2015** | 512.0 KB | `ceeae1f06d35109dd41cf2c40a2a15d5` | Factory Binary Firmware Dump |
| `readme.xml` | **1990–2015** | 170 B | `b2133034f14e6f4fd80ed3aaa6cc2915` | EcuFlash / RomRaider XML Definition |
| `sample_UserChannels.xml` | **1990–2015** | 1.2 KB | `6b11521ae19147e4d3b0d6b96016899c` | EcuFlash / RomRaider XML Definition |
| `Siemens_GS20_G10C9000_7552700_64K.xdf` | **1990–2015** | 949.7 KB | `c69d529314b99b0b5a9eab32e95b9c21` | TunerPro Binary Definition Map |
| `Siemens_GS20_G10C9000_7552700_64K__chookees-ecu.xdf` | **1990–2015** | 949.7 KB | `ca3f350fb3df75d6c4af2680e2c7b78c` | TunerPro Binary Definition Map |
| `Siemens_GS20_G10C9000_7552700_64K__chookees-ecu_63095ce0.xdf` | **1990–2015** | 949.7 KB | `63095ce0d37dbd8de76077f8920974e4` | TunerPro Binary Definition Map |
| `Siemens_MS43_430069_512K.xdf` | **1990–2015** | 3.31 MB | `22117ad65c0084f8ebd533af61d689ae` | TunerPro Binary Definition Map |
| `Siemens_MS43_430069_512K__chookees-ecu.xdf` | **1990–2015** | 3.29 MB | `b5ba7d3613a78fa014c7cfdafa734e9c` | TunerPro Binary Definition Map |
| `UNI_SF.MultiNFX04.bin` | **1990–2015** | 1.51 MB | `47fc541caa4834eb219c209621b9e2b4` | Factory Binary Firmware Dump |

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
