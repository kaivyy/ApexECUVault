# INTEGRA TYPE R - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: INTEGRA TYPE R
- **Model Year Coverage**: 1995–2006
- **Total Calibration Assets**: 25 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `int233stock.bin` | **1995–2006** | 32.0 KB | `d8162fe1dd0efd3b8c86187fc8d41517` | Factory Binary Firmware Dump |
| `Int338gr.bin` | **1995–2006** | 48.0 KB | `264e10128d8b21727ca37801b08c56cc` | Factory Binary Firmware Dump |
| `Int340ls.bin` | **1995–2006** | 48.0 KB | `575deaa0e55e51431bd31fe795ab1259` | Factory Binary Firmware Dump |
| `Int359tr.bin` | **1995–2006** | 48.0 KB | `0a79ba65e11c63beee11a8e0b46a5b33` | Factory Binary Firmware Dump |
| `Int422gr.bin` | **1995–2006** | 48.0 KB | `429dae21e8e7c68468ad8be82f94992b` | Factory Binary Firmware Dump |
| `Int474gr.bin` | **1995–2006** | 48.0 KB | `f7f01f2db5d9ee7ffba18edf3c13eca2` | Factory Binary Firmware Dump |
| `Int475ls.bin` | **1995–2006** | 48.0 KB | `68613a835f5e6ac68b92ad40dc837ec6` | Factory Binary Firmware Dump |
| `Int497tr.bin` | **1995–2006** | 48.0 KB | `4ca311f462f1d35847b9754ffc567b8b` | Factory Binary Firmware Dump |
| `Int712gr.bin` | **1995–2006** | 48.0 KB | `f4bb112e8924b2354f8409bb06a38930` | Factory Binary Firmware Dump |
| `p2p_p75-rom.bin` | **1995–2006** | 32.0 KB | `92eb7bead98f2a7b92f4c934a6f2d065` | Factory Binary Firmware Dump |
| `P73_M66507-715.bin` | **1995–2006** | 48.0 KB | `7abb209ca071708c7f96fee40af640dd` | Factory Binary Firmware Dump |
| `P74-USDM-214.bin` | **1995–2006** | 32.0 KB | `1c7b48c6dd70e23771a9a8c73f7a5cb4` | Factory Binary Firmware Dump |
| `p75-q01-270.bin` | **1995–2006** | 32.0 KB | `1786d82785ae4835093db38aa3bff6b5` | Factory Binary Firmware Dump |
| `PR3-900-93.bin` | **1995–2006** | 32.0 KB | `37a1d2d4585cff0dde8e3a9e76e2bbbc` | Factory Binary Firmware Dump |
| `pr3-901-58.bin` | **1995–2006** | 32.0 KB | `42f24a6afb95f4568e63bc5b20e98b07` | Factory Binary Firmware Dump |
| `pr3-j01-205.bin` | **1995–2006** | 32.0 KB | `3e40bf6b2821e513bdde2e9ce64260df` | Factory Binary Firmware Dump |
| `pr3-j51-219.bin` | **1995–2006** | 32.0 KB | `b1a63fc1a7796f6414bbbfc72c828f60` | Factory Binary Firmware Dump |
| `PR3GSR.bin` | **1995–2006** | 32.0 KB | `7da9829e2865e9bb9d38a662a46b0ddc` | Factory Binary Firmware Dump |
| `pr4-a02.bin.bin` | **1995–2006** | 32.0 KB | `146bdfb053ff2d90612ec9e33e9a74d4` | Factory Binary Firmware Dump |
| `pr4-q02-54.rom` | **1995–2006** | 32.0 KB | `50fc882709993c8b9684de395cf4b81e` | Factory Binary Firmware Dump |
| `pr4-q51-33.bin` | **1995–2006** | 32.0 KB | `c3f4edc311f96aff3d86c19f4694662f` | Factory Binary Firmware Dump |
| `pr4-q60-92.bin` | **1995–2006** | 32.0 KB | `f7cd387a42778e07a1de54b9fe08e105` | Factory Binary Firmware Dump |
| `pr4-q61-235.bin` | **1995–2006** | 32.0 KB | `b9b35ec946dbb080f7c06d95acdb3692` | Factory Binary Firmware Dump |
| `pr4-USDM-232.bin` | **1995–2006** | 32.0 KB | `33469c6ffe8b506a0c1a8cfbca743a49` | Factory Binary Firmware Dump |
| `STOCK-PR3.bin` | **1995–2006** | 32.0 KB | `5490eff6ba0981a520ffe499ff0d19f5` | Factory Binary Firmware Dump |

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
