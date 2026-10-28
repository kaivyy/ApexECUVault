# EDC17 CP02 CP09 330D 530D X5D - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: EDC17 CP02 CP09 330D 530D X5D
- **Model Year Coverage**: 2008–2014
- **Total Calibration Assets**: 8 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `4P1C2558.a2l` | **2008–2014** | 6.30 MB | `f304445ecad41d5643226a659e5b7bfe` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `4P1C2558L.a2l` | **2008–2014** | 6.79 MB | `3a7e356b8b2eaff4deb3ce92cf25bda5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `6P8KB574_a.a2l` | **2008–2014** | 14.99 MB | `1c512c2a9dc0721b8a86793dc28979c3` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `BMW EDC17CP09 530D.ols` | **2008–2014** | 15.95 MB | `0940ecf981508861e8d4137388bae7eb` | WinOLS Project Workspace & Calibration |
| `mpc_full.bin` | **2008–2014** | 2.00 MB | `435f9a3e44d952946e611bed880aee8c` | Factory Binary Firmware Dump |
| `X5d_Stock_ImmoOff.bin` | **2008–2014** | 2.00 MB | `32ab592612d5e218eff2312d4a08792f` | Factory Binary Firmware Dump |
| `X5d_Stock_ImmoOff_CSFixed.bin` | **2008–2014** | 2.00 MB | `383de6b8d3b45acc2d1294552f354119` | Factory Binary Firmware Dump |
| `X_78KBMN022A.hex` | **2008–2014** | 4.81 MB | `4649963aeca1ce362d332c7476612b0e` | Intel HEX Calibration Firmware |

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
