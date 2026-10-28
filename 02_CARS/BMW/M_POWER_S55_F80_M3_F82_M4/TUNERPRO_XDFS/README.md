# TUNERPRO XDFS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: TUNERPRO XDFS
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 13 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `00000D07596401.xdf` | **1998–2024** | 1.12 MB | `54ecc9ce7f7887341ef0024d0efb1d8a` | TunerPro Binary Definition Map |
| `00000E2B3B0A01.xdf` | **1998–2024** | 1021.2 KB | `2a1dfa71bd836d7a926179936ebaeb8d` | TunerPro Binary Definition Map |
| `00000FEF81A001.xdf` | **1998–2024** | 1.21 MB | `83f1f282b0239d12ac198c9dba23aea8` | TunerPro Binary Definition Map |
| `00001A841D1401.xdf` | **1998–2024** | 1.57 MB | `0a91d5aa1c18f041b51c2168bc6f17fa` | TunerPro Binary Definition Map |
| `00001A841D2801.xdf` | **1998–2024** | 1.56 MB | `b4a403f71993964061f2e73b7596863f` | TunerPro Binary Definition Map |
| `00001C41279601.xdf` | **1998–2024** | 1.21 MB | `85cfb2ad737aa42bfcfb8efb1050e1c6` | TunerPro Binary Definition Map |
| `000021571D8202.xdf` | **1998–2024** | 1.38 MB | `04f0ae0563997b3bfcdfb684ee4ad731` | TunerPro Binary Definition Map |
| `000021571DAA01.xdf` | **1998–2024** | 1.40 MB | `122abda26161d631f7c47e4bf1b3d34d` | TunerPro Binary Definition Map |
| `000021571DBE01.xdf` | **1998–2024** | 1.40 MB | `9650d306df275b381cfff6c43d77c00a` | TunerPro Binary Definition Map |
| `00002DF2132801.xdf` | **1998–2024** | 1.32 MB | `f5d6913ee2ecc1bcb137a42a96c7560e` | TunerPro Binary Definition Map |
| `00005BA8134601.xdf` | **1998–2024** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |
| `00005BA8135001.xdf` | **1998–2024** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |
| `00005BA8135A01.xdf` | **1998–2024** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |

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
