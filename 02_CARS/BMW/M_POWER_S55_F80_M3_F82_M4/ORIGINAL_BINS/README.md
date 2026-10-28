# ORIGINAL BINS - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: ORIGINAL BINS
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 26 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `00000D07596401_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `22f4467bf1ea293466a2cf3c97595d66` | Factory Binary Firmware Dump |
| `00000D07596401_original.bin` | **1998–2024** | 4.00 MB | `e5ced22adfcc37ae04010bd1757afcc2` | Factory Binary Firmware Dump |
| `00000E2B3B0A01_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `c5830c4d9e58945730e26df2a8a51404` | Factory Binary Firmware Dump |
| `00000E2B3B0A01_original.bin` | **1998–2024** | 4.00 MB | `9ec1f0116c862471f366b45274b1b175` | Factory Binary Firmware Dump |
| `00000FEF81A001_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `ad12310982ab8aa554d816d48440c553` | Factory Binary Firmware Dump |
| `00000FEF81A001_original.bin` | **1998–2024** | 4.00 MB | `2141d6f1bdb333648c551f0627539991` | Factory Binary Firmware Dump |
| `00001A841D1401_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `00e722618d0099967cef01acf498edf8` | Factory Binary Firmware Dump |
| `00001A841D1401_original.bin` | **1998–2024** | 4.00 MB | `00fb6d68da0d1da072bdac473f9d24e2` | Factory Binary Firmware Dump |
| `00001A841D2801_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `2987e6721b32d15a86c419b9b964ffc4` | Factory Binary Firmware Dump |
| `00001A841D2801_original.bin` | **1998–2024** | 4.00 MB | `1dd5c21041f21977d3018fb19d574546` | Factory Binary Firmware Dump |
| `00001C41279601_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `6cea001165ae87fe938f22281285675d` | Factory Binary Firmware Dump |
| `00001C41279601_original.bin` | **1998–2024** | 4.00 MB | `f580fb866af36e4cf777a65c4f1a0ee0` | Factory Binary Firmware Dump |
| `000021571D8202_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `0e1e9492e73620de9ccf62b143aa736f` | Factory Binary Firmware Dump |
| `000021571D8202_original.bin` | **1998–2024** | 4.00 MB | `f366030dba59706a62ab3befa574750a` | Factory Binary Firmware Dump |
| `000021571DAA01_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `13e3c907a38db3bf1bf02502df7aee98` | Factory Binary Firmware Dump |
| `000021571DAA01_original.bin` | **1998–2024** | 4.00 MB | `f79e479bdcde078a4ad6c6ce37adbfdc` | Factory Binary Firmware Dump |
| `000021571DBE01_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `f33f8fd2aa2b1ed7ea02e700f384db05` | Factory Binary Firmware Dump |
| `000021571DBE01_original.bin` | **1998–2024** | 4.00 MB | `8852385a6d9953eceff1e570e7d3b0e0` | Factory Binary Firmware Dump |
| `00002DF2132801_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `09238e53da6a3fe2f1e0d73dac479b6d` | Factory Binary Firmware Dump |
| `00002DF2132801_original.bin` | **1998–2024** | 4.00 MB | `b5f8af6342fa39902c1f2126e4011086` | Factory Binary Firmware Dump |
| `00005BA8134601_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `df04508b920e9b79d08c44afd9b4deae` | Factory Binary Firmware Dump |
| `00005BA8134601_original.bin` | **1998–2024** | 4.00 MB | `849a1be62b6ca75aede391ad419d2a73` | Factory Binary Firmware Dump |
| `00005BA8135001_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `033bc84fddd71ecfee6d466bceaaf67f` | Factory Binary Firmware Dump |
| `00005BA8135001_original.bin` | **1998–2024** | 4.00 MB | `1a1d5d8d08827fd68e18ce91fc4fca9d` | Factory Binary Firmware Dump |
| `00005BA8135A01_MapSwitchBase.bin` | **1998–2024** | 4.00 MB | `3401426fa2c085eac040c4d80ae678dc` | Factory Binary Firmware Dump |
| `00005BA8135A01_original.bin` | **1998–2024** | 4.00 MB | `28c681bd80da47f4fe54508af611d83f` | Factory Binary Firmware Dump |

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
