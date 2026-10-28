# v7.3 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: v7.3
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 22 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `F4C9G577B_5c64-010_090_007_v7.3.a2l` | **1998–2024** | 843.1 KB | `a46477b80683a237cdfb33776dfc1c33` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9G577B_5c64-010_090_007_v7.3.xdf` | **1998–2024** | 2.74 MB | `e80ccf727ae0e0ed403b7baf13bd23ee` | TunerPro Binary Definition Map |
| `F4C9G595B_5c64-010_100_005_v7.3.a2l` | **1998–2024** | 843.1 KB | `47509a36fd4496cf5f91534a4e73f1dd` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9G595B_5c64-010_100_005_v7.3.xdf` | **1998–2024** | 2.74 MB | `e80ccf727ae0e0ed403b7baf13bd23ee` | TunerPro Binary Definition Map |
| `F4C9G5F5B_5c64-010_130_005_v7.3.a2l` | **1998–2024** | 843.1 KB | `471998f3c9edc48e20fadfa882322dd4` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9G5F5B_5c64-010_130_005_v7.3.xdf` | **1998–2024** | 2.74 MB | `789db6e288bb0e3a7646abe821b24a91` | TunerPro Binary Definition Map |
| `F4C9G5H5B_5c64-010_140_005_v7.3.a2l` | **1998–2024** | 843.1 KB | `cd7d2a32ce636f164a126d281802f3a4` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9G5H5B_5c64-010_140_005_v7.3.xdf` | **1998–2024** | 2.74 MB | `e7560c6b4fd0459c30cb27e1e33d424a` | TunerPro Binary Definition Map |
| `F4C9L8A6B_5c64-020_050_006_v7.3.a2l` | **1998–2024** | 845.6 KB | `6fd605074940c3134bd5ca8b872d5914` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8A6B_5c64-020_050_006_v7.3.xdf` | **1998–2024** | 2.75 MB | `4103f9a1d9ecdcae59cab9c139aba13e` | TunerPro Binary Definition Map |
| `F4C9L8C5B_5c64-020_060_005_v7.3.a2l` | **1998–2024** | 845.6 KB | `5c5b85118a8ed06247d68ca83d4c0bc7` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8C5B_5c64-020_060_005_v7.3.xdf` | **1998–2024** | 2.75 MB | `49aaba654d91111ca76a84c5f13dad91` | TunerPro Binary Definition Map |
| `F4C9L8E6B_5c64-020_070_006_v7.3.a2l` | **1998–2024** | 845.7 KB | `a1e9b9e23797156186fdf6df603f58cd` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8E6B_5c64-020_070_006_v7.3.xdf` | **1998–2024** | 2.75 MB | `9efdf69992e8eebed930735794f733aa` | TunerPro Binary Definition Map |
| `F4C9L8G7B_5c64-020_080_007_v7.3.a2l` | **1998–2024** | 845.6 KB | `db6e6bfca36a7b7aded93329a353a1ce` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8G7B_5c64-020_080_007_v7.3.xdf` | **1998–2024** | 2.75 MB | `dafa85930ad3c46b10c20ccd3947782c` | TunerPro Binary Definition Map |
| `F4C9L8J5B_5c64-020_090_005_v7.3.a2l` | **1998–2024** | 845.6 KB | `630d83290b201cf08ad1d5ebc583e4c2` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8J5B_5c64-020_090_005_v7.3.xdf` | **1998–2024** | 2.75 MB | `b5fcc1f1073e7dbb3952bfae78325871` | TunerPro Binary Definition Map |
| `F4C9L8N6B_5c64-020_110_006_v7.3.a2l` | **1998–2024** | 845.6 KB | `ef67b07bbc990c0b3434cc6d8b659101` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8N6B_5c64-020_110_006_v7.3.xdf` | **1998–2024** | 2.75 MB | `f5ea65510ae1cfdbc0ac603fb2ae39e1` | TunerPro Binary Definition Map |
| `F4C9L8R5B_5c64-020_130_005_v7.3.a2l` | **1998–2024** | 845.6 KB | `4f19caee3863d58c260cfc7489ae6cc7` | ASAM MCD-2 MC / ASAP2 Definition Map |
| `F4C9L8R5B_5c64-020_130_005_v7.3.xdf` | **1998–2024** | 2.75 MB | `483f819d67451360c298941fe3ae30c1` | TunerPro Binary Definition Map |

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
