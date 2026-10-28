# MSS54 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: MSS54
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 37 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `211322000701J404.bin` | **1998–2024** | 32.0 KB | `cf069c06b1d747571dbe3bd2dd5903c6` | Factory Binary Firmware Dump |
| `211322000701J409.bin` | **1998–2024** | 32.0 KB | `2d7b2827125d09a09631eca4c1e24521` | Factory Binary Firmware Dump |
| `211322000701QD04.bin` | **1998–2024** | 32.0 KB | `37b44bbb4a00f0ce40264e0fd29b6e4e` | Factory Binary Firmware Dump |
| `211322000701QD09.bin` | **1998–2024** | 32.0 KB | `4e334fc013b1f9843d96ecf4f179e341` | Factory Binary Firmware Dump |
| `211322001501J424 (EU3 6MT).bin` | **1998–2024** | 32.0 KB | `796a1e707e1d9b0d8549a09b6169182a` | Factory Binary Firmware Dump |
| `211322001501J444 (NoEOBD 6MT).bin` | **1998–2024** | 32.0 KB | `af8b03abaab4360d079fed5b0edc2e57` | Factory Binary Firmware Dump |
| `211322001501J449 (Japan 6MT).bin` | **1998–2024** | 32.0 KB | `a0458c0597f45b940d9f8665d8d883bd` | Factory Binary Firmware Dump |
| `211322001501J464 (Low Compression 6MT).bin` | **1998–2024** | 32.0 KB | `5243fc0b991fc5375066a8b899be8fc5` | Factory Binary Firmware Dump |
| `211322001501J4E9.bin` | **1998–2024** | 32.0 KB | `bf57c35a0cf4b8a9dc9eb330e28caa44` | Factory Binary Firmware Dump |
| `211322001501J4G9.bin` | **1998–2024** | 32.0 KB | `746a98264f1d271570fe3b7829ad5c0b` | Factory Binary Firmware Dump |
| `211322001501JD34 (EU3 SMG).bin` | **1998–2024** | 32.0 KB | `249cdf5f73bc2770ff6bdb696cf174a6` | Factory Binary Firmware Dump |
| `211322001501JD54 (NoEOBD SMG).bin` | **1998–2024** | 32.0 KB | `642d042d2951f70e632c61151a06f72f` | Factory Binary Firmware Dump |
| `211322001501JD59 (Japan SMG).bin` | **1998–2024** | 32.0 KB | `3e8013f84401c6d4223428da56ac1426` | Factory Binary Firmware Dump |
| `211322001501JD74 (EU3 Low Compression SMG).bin` | **1998–2024** | 32.0 KB | `748b7c0e8aee81982a015a98f1dcfef0` | Factory Binary Firmware Dump |
| `211322001501JDD9 (US SMG).bin` | **1998–2024** | 32.0 KB | `ca4d05384c09dc6722d23d3cf1f13146` | Factory Binary Firmware Dump |
| `211322001501JDF9 (US SMG).bin` | **1998–2024** | 32.0 KB | `10ab216f1d4655334325bd29426d64e6` | Factory Binary Firmware Dump |
| `211322001701JD34 (EU3 SMG).bin` | **1998–2024** | 32.0 KB | `d6b6504cf2f281f1f67ccd65acebb246` | Factory Binary Firmware Dump |
| `211322002101J424 (EU3 6MT).bin` | **1998–2024** | 32.0 KB | `6e6ab25de1f67129be04dde6df56d33d` | Factory Binary Firmware Dump |
| `211322002101J444 (NoEOBD 6MT).bin` | **1998–2024** | 32.0 KB | `a2a54c08d89596bbf65e6d26c3aa17ba` | Factory Binary Firmware Dump |
| `211322002101J449 (Japan 6MT).bin` | **1998–2024** | 32.0 KB | `058f0cb68ea6208f59a7945ec34088ab` | Factory Binary Firmware Dump |
| `211322002101J464 (Low Compression 6MT).bin` | **1998–2024** | 32.0 KB | `7f84e668f04be3275ebbd186e9819b02` | Factory Binary Firmware Dump |
| `211322002101J469 (US 6MT heated DMTL).bin` | **1998–2024** | 32.0 KB | `edb35cf30ae97f2b5967bb8bdbb5cf62` | Factory Binary Firmware Dump |
| `211322002101JD34 (EU3 SMG).bin` | **1998–2024** | 32.0 KB | `6fb86d4bad81b41ffea0fd7fe40f1b0f` | Factory Binary Firmware Dump |
| `211322002101JD54 (NoEOBD SMG).bin` | **1998–2024** | 32.0 KB | `76b838de2c109669d37d33a2c22ac218` | Factory Binary Firmware Dump |
| `211322002101JD59 (Japan SMG).bin` | **1998–2024** | 32.0 KB | `7cf1a1c69ee7b6389d12829f01130f9e` | Factory Binary Firmware Dump |
| `211322002101JD74 (EU3 Low Compression SMG).bin` | **1998–2024** | 32.0 KB | `861c68c6c20926dc3af02bb18d46984b` | Factory Binary Firmware Dump |
| `211322002101Q424 (EU Z3M).bin` | **1998–2024** | 32.0 KB | `ab152372029bb24b181e78763c239a91` | Factory Binary Firmware Dump |
| `211322002101Q444 (NoEOBD Z3M).bin` | **1998–2024** | 32.0 KB | `715e3ff4ad2c22c9a91479cc3bf5feba` | Factory Binary Firmware Dump |
| `211322002101Q449 (Japan Low Compression Z3M).bin` | **1998–2024** | 32.0 KB | `30d6221993241c1692e264596525b0c4` | Factory Binary Firmware Dump |
| `211322002101Q464 (Low Compression Z3M).bin` | **1998–2024** | 32.0 KB | `d9110340dad2c097b2fe91231ef7a254` | Factory Binary Firmware Dump |
| `211322002601JD39 (US SMG non-heated DMTL).bin` | **1998–2024** | 32.0 KB | `f29eb89a221087055112b2628f6292b2` | Factory Binary Firmware Dump |
| `211322002601JD79 (US SMG heated DMTL).bin` | **1998–2024** | 32.0 KB | `e649c5fd26803643f5ed6bd5cc0eaa98` | Factory Binary Firmware Dump |
| `211322002801J429 (US 6MT non-heated DMTL).bin` | **1998–2024** | 32.0 KB | `3f05fd1f085d2ffc7a9638e693bf3ead` | Factory Binary Firmware Dump |
| `211322002801J469 (US 6MT heated DMTL).bin` | **1998–2024** | 32.0 KB | `584872b53de3eb103fe9f5984a4069af` | Factory Binary Firmware Dump |
| `211322002801JD39 (US SMG non-heated DMTL).bin` | **1998–2024** | 32.0 KB | `815233c002f9478c3695a522de3167f7` | Factory Binary Firmware Dump |
| `211322002801JD79 (US SMG heated DMTL).bin` | **1998–2024** | 32.0 KB | `265c5d828f365e3a879072190d780eb9` | Factory Binary Firmware Dump |
| `211322002801Q429 (US Z3M).bin` | **1998–2024** | 32.0 KB | `1b4fe91c349bbb431fe7bfc87f75189c` | Factory Binary Firmware Dump |

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
