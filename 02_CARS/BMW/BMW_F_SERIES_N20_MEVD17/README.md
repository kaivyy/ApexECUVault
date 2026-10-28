# BMW F SERIES N20 MEVD17 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: BMW F SERIES N20 MEVD17
- **Model Year Coverage**: 2011–2017
- **Total Calibration Assets**: 12 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `00000ABF3BA001_n20o1_original.bin` | **2011–2017** | 4.00 MB | `5687afc10dc179d450144940c3ff6b67` | Factory Binary Firmware Dump |
| `00000ABF3BA001_original.bin` | **2011–2017** | 4.00 MB | `2e98a51eae98cd164df41a459065c77a` | Factory Binary Firmware Dump |
| `0000113D3BA001_n20o1_original.bin` | **2011–2017** | 4.00 MB | `d41efa5e96d319f543e4095ec8698b9c` | Factory Binary Firmware Dump |
| `0000113D3BA001_original.bin` | **2011–2017** | 4.00 MB | `6a761f89406c1877f908d54c9c63643f` | Factory Binary Firmware Dump |
| `000013E713AA01_n20o1_original.bin` | **2011–2017** | 4.00 MB | `25e81bbc76f11d2588c6124e7128585a` | Factory Binary Firmware Dump |
| `000013E713AA01_original.bin` | **2011–2017** | 4.00 MB | `e32bf56d3e0fad8cf8c0f26b03bb24ca` | Factory Binary Firmware Dump |
| `000019A813AA01_n20o1_original.bin` | **2011–2017** | 4.00 MB | `ed829b922c1cf74634035f9251cfbcbe` | Factory Binary Firmware Dump |
| `000019A813AA01_original.bin` | **2011–2017** | 4.00 MB | `719221dce7d4e833fac8b0695a5adbd6` | Factory Binary Firmware Dump |
| `00001BC91D9601_n20o1_original.bin` | **2011–2017** | 4.00 MB | `492dd4e3da430c6a61b8ebed77245de3` | Factory Binary Firmware Dump |
| `00001BC91D9601_original.bin` | **2011–2017** | 4.00 MB | `016b16866faed4a13b83b9cc54b7adcd` | Factory Binary Firmware Dump |
| `00001C9F1D9601_n20o1_original.bin` | **2011–2017** | 4.00 MB | `ccda51f278928f4edbbd170ff9f33426` | Factory Binary Firmware Dump |
| `00001C9F1D9601_original.bin` | **2011–2017** | 4.00 MB | `57ffa57f20ff903a39677996d044129b` | Factory Binary Firmware Dump |

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
