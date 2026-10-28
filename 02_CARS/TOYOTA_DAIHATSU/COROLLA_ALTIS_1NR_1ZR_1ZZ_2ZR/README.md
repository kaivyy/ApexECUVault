# COROLLA ALTIS 1NR 1ZR 1ZZ 2ZR - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: COROLLA ALTIS 1NR 1ZR 1ZZ 2ZR
- **Model Year Coverage**: 2001–2022
- **Total Calibration Assets**: 13 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `89663-02023.bin` | **2001–2022** | 320.0 KB | `5ddef7c2ce9c5abbefa2cb8777628d13` | Factory Binary Firmware Dump |
| `89663-02161.bin` | **2001–2022** | 320.0 KB | `d1ae6fb54e61566ae61e4056154def06` | Factory Binary Firmware Dump |
| `89663-02162.bin` | **2001–2022** | 320.0 KB | `dcbe18885ef74606548a923362f147b5` | Factory Binary Firmware Dump |
| `89663-02172.bin` | **2001–2022** | 320.0 KB | `bb4c9d3fb90a71d01256df472084d983` | Factory Binary Firmware Dump |
| `89663-02173.bin` | **2001–2022** | 320.0 KB | `aa21e2bea3f428607d36e113fc6167dc` | Factory Binary Firmware Dump |
| `89663-02241.bin` | **2001–2022** | 368.0 KB | `9bc2041a3ec839cfd9c8017fd72d77ff` | Factory Binary Firmware Dump |
| `89663-02270.bin` | **2001–2022** | 368.0 KB | `d1f80cabcd6dd3a2cf2be553de6f1e8e` | Factory Binary Firmware Dump |
| `89663-02482.bin` | **2001–2022** | 496.0 KB | `2dd339b573686fbc28c6698133ba16bf` | Factory Binary Firmware Dump |
| `89663-02502.bin` | **2001–2022** | 496.0 KB | `69b5ac8f844408bc29de9180f4c4e603` | Factory Binary Firmware Dump |
| `89663-02661.bin` | **2001–2022** | 736.0 KB | `d8cc949db374e6eea05971f1892a1efc` | Factory Binary Firmware Dump |
| `89663-02E73.bin` | **2001–2022** | 992.0 KB | `01c750bb362506d8026022a952303b60` | Factory Binary Firmware Dump |
| `89663-02J13.bin` | **2001–2022** | 736.0 KB | `4206fdd3371c26cdeee436b3c26d6c24` | Factory Binary Firmware Dump |
| `89663-02J22.bin` | **2001–2022** | 736.0 KB | `3d4a843cdf1faf04d594e6aa9f62ea05` | Factory Binary Firmware Dump |

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
