# SIM2K 250 260 HYUNDAI KIA N PERFORMANCE - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SIM2K 250 260 HYUNDAI KIA N PERFORMANCE
- **Model Year Coverage**: 2017–2024
- **Total Calibration Assets**: 18 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `CNNKKM___TAA.xdf` | **2017–2024** | 2.32 MB | `b91db0175f30c69b20bad65bc33760be` | TunerPro Binary Definition Map |
| `CNPNKM___T3A.xdf` | **2017–2024** | 4.72 MB | `5e1296d84d3e336eb14880cef1dfc2ce` | TunerPro Binary Definition Map |
| `CNPNKM__FT5A.xdf` | **2017–2024** | 9.08 MB | `74b075e1bb7259c6bce0a4b55cf1b935` | TunerPro Binary Definition Map |
| `CPQDDGMCXXXSDU50.xdf` | **2017–2024** | 4.70 MB | `978a94a28612493d48c962bdc4db44f9` | TunerPro Binary Definition Map |
| `CPQWDEMCXXXSDU50.xdf` | **2017–2024** | 4.84 MB | `db9416720eb6f49ce1b8973e91649570` | TunerPro Binary Definition Map |
| `CPQWDGMCXXXSDU50D.xdf` | **2017–2024** | 4.81 MB | `386b0ebd0b39d554b700c69393d28de1` | TunerPro Binary Definition Map |
| `JSNNJMK__S2A.xdf` | **2017–2024** | 2.68 MB | `094bdbdd1eebfc3e45b68e0ddd0f787a` | TunerPro Binary Definition Map |
| `JSNNKMK__S2A.xdf` | **2017–2024** | 2.68 MB | `094bdbdd1eebfc3e45b68e0ddd0f787a` | TunerPro Binary Definition Map |
| `Original [CNNKKM___TAA].bin` | **2017–2024** | 2.50 MB | `18b3a80d4ee30a72359024cc04e7dc3d` | Factory Binary Firmware Dump |
| `Original [CNPNKM___T3A].bin` | **2017–2024** | 2.50 MB | `5fc637fa118a2c7cba3cd9a839ffbe15` | Factory Binary Firmware Dump |
| `Original [CNPNKM__FT5A].bin` | **2017–2024** | 2.50 MB | `fa8e82f5c93e7093a84989fdce923d85` | Factory Binary Firmware Dump |
| `Original [CPQDDGMCXXXSDU50].bin` | **2017–2024** | 2.63 MB | `cea0ee75701130e02dd265290459efaf` | Factory Binary Firmware Dump |
| `Original [CPQWDEMCXXXSDU50].bin` | **2017–2024** | 2.50 MB | `d5acf9672f8db1d797a58837b32d8985` | Factory Binary Firmware Dump |
| `Original [CPQWDGMCXXXSDU50D].bin` | **2017–2024** | 2.50 MB | `f412645ab38dbbbd17cdbde2f9fbb74a` | Factory Binary Firmware Dump |
| `Original [JSNNJMK__S2A].bin` | **2017–2024** | 2.50 MB | `b98d26833e8873b4c0850a671e05e511` | Factory Binary Firmware Dump |
| `Original [JSNNKMK__S2A].bin` | **2017–2024** | 2.50 MB | `9df768ad6214d2ef1ed54dfe25ecce1a` | Factory Binary Firmware Dump |
| `Original [OSPNKM___T3A].bin` | **2017–2024** | 2.50 MB | `df6d746810819071b0a64c89c80ddf2a` | Factory Binary Firmware Dump |
| `OSPNKM___T3A.xdf` | **2017–2024** | 5.06 MB | `e792e43e5063fe2547db12e291eaa9a8` | TunerPro Binary Definition Map |

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
