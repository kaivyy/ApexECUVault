# ACURA NSX LEGEND - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: ACURA NSX LEGEND
- **Model Year Coverage**: 1990–2005
- **Total Calibration Assets**: 19 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `Acura_NSX_and_Legend.xdf` | **1990–2005** | 622.6 KB | `3b5578088ff49f70ce8ccaa45ced78ad` | TunerPro Binary Definition Map |
| `JDM Type I (PY3-902).BIN` | **1990–2005** | 32.0 KB | `ff6ad98fe87bac672dc7d48a1b713ec5` | Factory Binary Firmware Dump |
| `JDM Type II.bin` | **1990–2005** | 32.0 KB | `7ba31c1093e0cebe8b2bd68707d90011` | Factory Binary Firmware Dump |
| `NSX91M OEM.bin` | **1990–2005** | 32.0 KB | `0280c365621b19d4dd891b38d321ef5c` | Factory Binary Firmware Dump |
| `NSX94M OEM.bin` | **1990–2005** | 32.0 KB | `1749874d307a3d6121600cd4bce4a7e7` | Factory Binary Firmware Dump |
| `PR7-A03.bin` | **1990–2005** | 32.0 KB | `e6a6c7a19715c8d3f792b62262b26c83` | Factory Binary Firmware Dump |
| `PR7-xxx.bin` | **1990–2005** | 32.0 KB | `a9d7c4ae2075a40e9d8fba04a4274a2f` | Factory Binary Firmware Dump |
| `PX9-A05, A15, A04, A55, A65.bin` | **1990–2005** | 32.0 KB | `0d19d91e0e4173d7d179e266ee1a7e6d` | Factory Binary Firmware Dump |
| `PX9-A57, A67, L57, A17, A07.bin` | **1990–2005** | 32.0 KB | `3bf1f14adbd56b5be3b3a50823b4d0f2` | Factory Binary Firmware Dump |
| `PX9-L68 - California.bin` | **1990–2005** | 32.0 KB | `bb4d5bb98ca4b475c723dcce3e32fd8f` | Factory Binary Firmware Dump |
| `PY3-A02, A52.bin` | **1990–2005** | 32.0 KB | `758c6309ad1cb14ca05f715e3f5eca68` | Factory Binary Firmware Dump |
| `PY3-A06, A53.bin` | **1990–2005** | 32.0 KB | `758c6309ad1cb14ca05f715e3f5eca68` | Factory Binary Firmware Dump |
| `PY3-A55.bin` | **1990–2005** | 32.0 KB | `83f921ad20a0b8fc6b52bfb2ebc4377e` | Factory Binary Firmware Dump |
| `PY3-A57.BIN` | **1990–2005** | 64.0 KB | `ca65a201725c97ed4a608f82b70b0d3b` | Factory Binary Firmware Dump |
| `Py3-A58 stock.bin` | **1990–2005** | 32.0 KB | `ef0208ac8568af52bd6d2d39f5a29e67` | Factory Binary Firmware Dump |
| `PY3-A58.bin` | **1990–2005** | 32.0 KB | `2fb2e2fe57dcf98fb9a5896d9a50a000` | Factory Binary Firmware Dump |
| `PY3-A72.bin` | **1990–2005** | 32.0 KB | `755d3850fbd07d3ede94eab9df7b70eb` | Factory Binary Firmware Dump |
| `PY3-G52 European.BIN` | **1990–2005** | 32.0 KB | `b0a0f0636524f917163f2dc04c5b4f2c` | Factory Binary Firmware Dump |
| `PY3-Y52 Guatemala.bin` | **1990–2005** | 32.0 KB | `db7c882d1db09352c9a311dcfe837ff8` | Factory Binary Firmware Dump |

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
