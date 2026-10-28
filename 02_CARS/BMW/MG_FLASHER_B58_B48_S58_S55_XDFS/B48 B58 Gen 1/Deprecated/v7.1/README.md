# v7.1 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: v7.1
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 25 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `R0C9J8B2B_3081-080_017_002_v7.1.a2l` | **1998–2024** | 176.7 KB | `3e2ff06abf51164703c95d7b36036acb` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9J8D2B_3081-080_021_002_v7.1.a2l` | **1998–2024** | 176.7 KB | `56c2a671fbb8e126d18bb41059581bde` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9J8I2B_3081-080_029_002_v7.1.a2l` | **1998–2024** | 176.7 KB | `7de9b79bef1b7f182c2e1fbdc9ac7a60` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9J8I3B_3081-080_029_003_v7.1.a2l` | **1998–2024** | 176.7 KB | `a6834840c382691c79946ba49882ed6c` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9J8I4B_3081-080_029_004_v7.1.a2l` | **1998–2024** | 176.7 KB | `1ac54017e77e50792cfaa82f435e6746` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9J962B_3081-090_010_002_v7.1.a2l` | **1998–2024** | 176.7 KB | `0b30b8471eecd2259b06e2c7270965e5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9J9E3B_3081-090_020_003_v7.1.a2l` | **1998–2024** | 176.7 KB | `e9f718e1e725c69d27205e7bc0049bcc` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9J9E4B_3081-090_020_004_v7.1.a2l` | **1998–2024** | 176.7 KB | `d532a8f779245831473bd5faeacb26c5` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9JA05B_3081-090_025_005_v7.1.a2l` | **1998–2024** | 176.7 KB | `2883fd530d4c86149e981fd60d736583` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9JA15B_3081-090_030_005_v7.1.a2l` | **1998–2024** | 176.7 KB | `7f1b16fa6b6ca7fdf31d0022159f8fd9` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9JC05B_3081-090_050_005_v7.1.a2l` | **1998–2024** | 176.7 KB | `e65874921dc7442fb5ae5b18bfdb6e7b` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R0C9JD06B_3081-090_060_006_v7.1.a2l` | **1998–2024** | 176.7 KB | `58af158a8dc45de18d36e9e6f896a688` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9I562B_3076-050_006_002_v7.1.a2l` | **1998–2024** | 175.9 KB | `e59fbb90b8be637f5f877efb254b5210` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9J8B2B_3076-080_017_002_v7.1.a2l` | **1998–2024** | 176.9 KB | `fece732d66c65575d7e8e71e04368575` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9J8B3B_3076-080_017_003_v7.1.a2l` | **1998–2024** | 176.9 KB | `ffd50d6e74a8073bb941b4728aee155d` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9J8I2B_3076-080_029_002_v7.1.a2l` | **1998–2024** | 176.9 KB | `2c4577f01a3cf4e679c805ed4da88aef` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9J8I7B_3076-080_029_007_v7.1.a2l` | **1998–2024** | 176.9 KB | `b2d620472b6ee6b0c9d80375d5cf73d6` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9J962B_3076-090_010_002_v7.1.a2l` | **1998–2024** | 176.9 KB | `7815e6b0550dbf3e7e8a5f25a9fe7404` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9J9E3B_3076-090_020_003_v7.1.a2l` | **1998–2024** | 176.9 KB | `282d7baf17894489e180f9e41a00dab9` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9J9E5B_3076-090_020_005_v7.1.a2l` | **1998–2024** | 176.9 KB | `815624d6b9a5073b96cfd8bce2289daf` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9J9E7B_3076-090_020_007_v7.1.a2l` | **1998–2024** | 176.9 KB | `f82feca39f46ae6592d32ba92f4d9e3e` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9JA05B_3076-090_025_005_v7.1.a2l` | **1998–2024** | 176.9 KB | `b6c06686e9ce676055a3136d61a6e608` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9JC05B_3076-090_050_005_v7.1.a2l` | **1998–2024** | 176.9 KB | `523684688d2094dd245049a853f7ff8d` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9JD06B_3076-090_060_006_v7.1.a2l` | **1998–2024** | 176.9 KB | `2a9c4403829ab203d345a6ac0837a30e` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `R1C9JE15B_3076-090_080_005_v7.1.a2l` | **1998–2024** | 176.9 KB | `261d649f9d0de31d21e7bb07f9ad5800` | ASAM MCD-2 MC / ASAP2 Definition Map |

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
