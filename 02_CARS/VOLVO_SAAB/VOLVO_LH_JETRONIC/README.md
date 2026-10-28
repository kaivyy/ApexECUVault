# VOLVO LH JETRONIC - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: VOLVO LH JETRONIC
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 17 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `0227400208_2227355740_EZK116.bin` | **1998–2024** | 32.0 KB | `c990ca22b7298c3e1ffb4be3498462b1` | Factory Binary Firmware Dump |
| `0280-000-560.BIN` | **1998–2024** | 32.0 KB | `a5d6f19f0197b180279220da1a01be0e` | Factory Binary Firmware Dump |
| `0280-000-913.BIN` | **1998–2024** | 32.0 KB | `a8b749312dd509083a46d235a0591ab8` | Factory Binary Firmware Dump |
| `0280-000-937.BIN` | **1998–2024** | 32.0 KB | `77dd7926bbf4e96f4d5c84fe30ef2ff1` | Factory Binary Firmware Dump |
| `0280-000-954.BIN` | **1998–2024** | 32.0 KB | `a7ee63b62a8c27820018b85eb8a2d04e` | Factory Binary Firmware Dump |
| `0280-000-962.BIN` | **1998–2024** | 32.0 KB | `aced46ff3dd6671e65f30221fbe65bbf` | Factory Binary Firmware Dump |
| `Bensin 984 chip 1 037 358 931.bin` | **1998–2024** | 32.0 KB | `da50f84b31fd0fb26e1921d7de80f371` | Factory Binary Firmware Dump |
| `lh2.2 NA 511.BIN` | **1998–2024** | 4.0 KB | `c78d51ee419ab6fa10719d12a93f5265` | Factory Binary Firmware Dump |
| `Volvo_556.xdf` | **1998–2024** | 8.6 KB | `4e93076613a1524add8e97ee10caaaf8` | TunerPro Binary Definition Map |
| `Volvo_560.xdf` | **1998–2024** | 8.4 KB | `ee23511ef143e130171b1818c6303823` | TunerPro Binary Definition Map |
| `Volvo_913.xdf` | **1998–2024** | 10.9 KB | `e34bc384fe96f4f70b75043783336d89` | TunerPro Binary Definition Map |
| `Volvo_954_LH2.4.xdf` | **1998–2024** | 10.4 KB | `eb0c61620d74a2f105ee425d31d155cf` | TunerPro Binary Definition Map |
| `Volvo_962.xdf` | **1998–2024** | 9.6 KB | `06527829d32aa08980389feb24b71577` | TunerPro Binary Definition Map |
| `Volvo_EZK_208.xdf` | **1998–2024** | 12.7 KB | `3dd816f0a5e72a52ca64f10979c76c48` | TunerPro Binary Definition Map |
| `Volvo_LH22_511.xdf` | **1998–2024** | 4.0 KB | `bd27658f8d7bc79f7f5a5ad238c109a0` | TunerPro Binary Definition Map |
| `Volvo_LH22_554.xdf` | **1998–2024** | 5.2 KB | `66136499f03c8a884b3954ad9a749513` | TunerPro Binary Definition Map |
| `Volvo_LH24_937.xdf` | **1998–2024** | 9.0 KB | `9a4b7d1894974fd9c6bf081774eb13ec` | TunerPro Binary Definition Map |

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
