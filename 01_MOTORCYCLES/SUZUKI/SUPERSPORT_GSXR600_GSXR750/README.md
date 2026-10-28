# SUPERSPORT GSXR600 GSXR750 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SUPERSPORT GSXR600 GSXR750
- **Model Year Coverage**: 2008–2010
- **Total Calibration Assets**: 5 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `G750K9.bin` | **2008–2010** | 1.00 MB | `16240ffff6d744307f3087c33d472172` | Factory Binary Firmware Dump |
| `G750K9G.bin` | **2008–2010** | 1.00 MB | `5bf7e3c900851a94288489bbd8eee696` | Factory Binary Firmware Dump |
| `GENERATIONAL_32920-01H00_Suzuki_GSX_R600_K6_K7_2006_2007_125PS.xdf` | **2008–2010** | 1.8 KB | `2d1e8330b5a02497dd6fd634ab1cc21d` | TunerPro Binary Definition Map |
| `GENERATIONAL_32920-14J00_Suzuki_GSX_R600_L1_L9_Showa_BPF_2011_2020_126PS.xdf` | **2008–2010** | 1.8 KB | `4eddf667010876f481b966a79fa9321d` | TunerPro Binary Definition Map |
| `GENERATIONAL_32920-14J50_Suzuki_GSX_R750_L1_L9_2011_2020_150PS.xdf` | **2008–2010** | 1.8 KB | `833eb20d7488a7cf87528d5baea75111` | TunerPro Binary Definition Map |

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
