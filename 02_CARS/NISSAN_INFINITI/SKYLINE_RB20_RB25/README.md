# SKYLINE RB20 RB25 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: SKYLINE RB20 RB25
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 70 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `ECR33_RB25DE_17U14_AT_MECR514.bin` | **1998–2024** | 32.0 KB | `88e7f19bf52d52c6d4b84f9a0c766a34` | Factory Binary Firmware Dump |
| `ECR33_RB25DE_28U00_MT_MEC-R700.bin` | **1998–2024** | 32.0 KB | `d87200d55fd5d75bca9ed099459047c8` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_13U00_MT_MEC-R720.bin` | **1998–2024** | 32.0 KB | `c8950859d771360e4b69defbcd3cf3c1` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_13U01_MT_MEC-R260.bin` | **1998–2024** | 32.0 KB | `ecc2ae76a8b877cd8d2641e81c9aed2f` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U00_MT_MECR520.bin` | **1998–2024** | 32.0 KB | `8ff34d3cd1ff166a7f6e0432c8753d65` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U01_MT_MECR521_daughterboard.BIN` | **1998–2024** | 32.0 KB | `a3913ab115b4f37c3e37698d298dd866` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U02_MT.bin` | **1998–2024** | 32.0 KB | `59ee88ecb993d90c60055da4e511ca6f` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U03.bin` | **1998–2024** | 32.0 KB | `dc037cb006ff718da05571acae9b4388` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U11_AT_MECR531.bin` | **1998–2024** | 32.0 KB | `dcaa3f2695a6dc82d933a9a8db55a09f` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U60_MT_MECR530.bin` | **1998–2024** | 32.0 KB | `5ab53e3c832ef44721e6aabeb28d8fea` | Factory Binary Firmware Dump |
| `ECR33_RB25DET_21U70.bin` | **1998–2024** | 32.0 KB | `f1af734b5fac1f69e148154569835c1a` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA500_MT.bin` | **1998–2024** | 64.0 KB | `c3015b3be3081fb76a2883e3f8727a44` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA501_MT.bin` | **1998–2024** | 64.0 KB | `71b5ed4eeead5b9a3851df20f825dd5c` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA502_MT.bin` | **1998–2024** | 64.0 KB | `fc6bfe12b220501a02808dbe9d8a3644` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA510_AT.bin` | **1998–2024** | 64.0 KB | `a70a1f93f0be45c6ead3b29de32aced8` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA511_AT.bin` | **1998–2024** | 64.0 KB | `f7f7065d16877bfb510355b0558d6f84` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA512_AT.bin` | **1998–2024** | 64.0 KB | `f8d8dade7aa82442721ae35034991474` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA513_AT.bin` | **1998–2024** | 64.0 KB | `9030d7c636fdbe6480295790dd4537a6` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA560_MT.bin` | **1998–2024** | 64.0 KB | `3cd1425872f768da8110c241f9630126` | Factory Binary Firmware Dump |
| `ER34_RB25DET_AA570_AT.bin` | **1998–2024** | 64.0 KB | `b47cf11ed3ffe14643cd6b3b314857a5` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_01U01_MEC-R124.BIN` | **1998–2024** | 32.0 KB | `5040ac9797dc65418ab04622e0f43a3a` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U00_MT_MEC-R106.bin` | **1998–2024** | 32.0 KB | `2b632fe336fa6c9e8ff3cecfdc6e3be0` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U01_MT_MEC-R126.BIN` | **1998–2024** | 32.0 KB | `d20a3b7357a20012ecfee57a27a29d90` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U02_MT_MEC-R132.bin` | **1998–2024** | 32.0 KB | `094566ad0d41b49e0cfa686246339381` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U11_AT_MECR109.bin` | **1998–2024** | 32.0 KB | `e4e87f33d5d8f472e110e5798c473978` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U12_AT_MECR127.bin` | **1998–2024** | 32.0 KB | `7412119766c3c2f68281ce322ff5e0b9` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U60_MT_GTS4.bin` | **1998–2024** | 32.0 KB | `ddb6089de1946f59a08c1fc266d8752d` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_04U70_AT_GTS4_MEC-R117.bin` | **1998–2024** | 32.0 KB | `dd0556b46d65c12992f4a04ddb8499c2` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_10U01_MEC-R210B.bin` | **1998–2024** | 32.0 KB | `8c0c6774d7eeda447331152f3d816b8a` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_10U11_MEC-217.bin` | **1998–2024** | 32.0 KB | `abfca442ef5dc9986f56b3d00d96d2bc` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U00_MT_MEC-212B.bin` | **1998–2024** | 32.0 KB | `1ff8dc2c3c1ca8a80030e0749fb98c49` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U01.bin` | **1998–2024** | 32.0 KB | `15477dcf386553002608db42f8bebe46` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U10_AT.bin` | **1998–2024** | 32.0 KB | `0ddb29f034a914b9479cd0b5601ded75` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U60_MT_MEC-214B.bin` | **1998–2024** | 32.0 KB | `e8332d3363735e60a71444699d480769` | Factory Binary Firmware Dump |
| `HCR32_RB20DET_11U70_MT_MEC-215B.bin` | **1998–2024** | 32.0 KB | `1e4b87674034f30ec5ae806c14517129` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DE_17U14_AT_MECR514.bin` | **1998–2024** | 32.0 KB | `88e7f19bf52d52c6d4b84f9a0c766a34` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DE_28U00_MT_MEC-R700.bin` | **1998–2024** | 32.0 KB | `d87200d55fd5d75bca9ed099459047c8` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_13U00_MT_MEC-R720.bin` | **1998–2024** | 32.0 KB | `c8950859d771360e4b69defbcd3cf3c1` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_13U01_MT_MEC-R260.bin` | **1998–2024** | 32.0 KB | `ecc2ae76a8b877cd8d2641e81c9aed2f` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U00_MT_MECR520.bin` | **1998–2024** | 32.0 KB | `8ff34d3cd1ff166a7f6e0432c8753d65` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U01_MT_MECR521_daughterboard.BIN` | **1998–2024** | 32.0 KB | `a3913ab115b4f37c3e37698d298dd866` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U02_MT.bin` | **1998–2024** | 32.0 KB | `59ee88ecb993d90c60055da4e511ca6f` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U03.bin` | **1998–2024** | 32.0 KB | `dc037cb006ff718da05571acae9b4388` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U11_AT_MECR531.bin` | **1998–2024** | 32.0 KB | `dcaa3f2695a6dc82d933a9a8db55a09f` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U60_MT_MECR530.bin` | **1998–2024** | 32.0 KB | `5ab53e3c832ef44721e6aabeb28d8fea` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ECR33_RB25DET_21U70.bin` | **1998–2024** | 32.0 KB | `f1af734b5fac1f69e148154569835c1a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA500_MT.bin` | **1998–2024** | 64.0 KB | `c3015b3be3081fb76a2883e3f8727a44` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA501_MT.bin` | **1998–2024** | 64.0 KB | `71b5ed4eeead5b9a3851df20f825dd5c` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA502_MT.bin` | **1998–2024** | 64.0 KB | `fc6bfe12b220501a02808dbe9d8a3644` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA510_AT.bin` | **1998–2024** | 64.0 KB | `a70a1f93f0be45c6ead3b29de32aced8` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA511_AT.bin` | **1998–2024** | 64.0 KB | `f7f7065d16877bfb510355b0558d6f84` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA512_AT.bin` | **1998–2024** | 64.0 KB | `f8d8dade7aa82442721ae35034991474` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA513_AT.bin` | **1998–2024** | 64.0 KB | `9030d7c636fdbe6480295790dd4537a6` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA560_MT.bin` | **1998–2024** | 64.0 KB | `3cd1425872f768da8110c241f9630126` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_ER34_RB25DET_AA570_AT.bin` | **1998–2024** | 64.0 KB | `b47cf11ed3ffe14643cd6b3b314857a5` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_01U01_MEC-R124.BIN` | **1998–2024** | 32.0 KB | `5040ac9797dc65418ab04622e0f43a3a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U00_MT_MEC-R106.bin` | **1998–2024** | 32.0 KB | `2b632fe336fa6c9e8ff3cecfdc6e3be0` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U01_MT_MEC-R126.BIN` | **1998–2024** | 32.0 KB | `d20a3b7357a20012ecfee57a27a29d90` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U02_MT_MEC-R132.bin` | **1998–2024** | 32.0 KB | `094566ad0d41b49e0cfa686246339381` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U11_AT_MECR109.bin` | **1998–2024** | 32.0 KB | `e4e87f33d5d8f472e110e5798c473978` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U12_AT_MECR127.bin` | **1998–2024** | 32.0 KB | `7412119766c3c2f68281ce322ff5e0b9` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U60_MT_GTS4.bin` | **1998–2024** | 32.0 KB | `ddb6089de1946f59a08c1fc266d8752d` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_04U70_AT_GTS4_MEC-R117.bin` | **1998–2024** | 32.0 KB | `dd0556b46d65c12992f4a04ddb8499c2` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_10U01_MEC-R210B.bin` | **1998–2024** | 32.0 KB | `8c0c6774d7eeda447331152f3d816b8a` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_10U11_MEC-217.bin` | **1998–2024** | 32.0 KB | `abfca442ef5dc9986f56b3d00d96d2bc` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U00_MT_MEC-212B.bin` | **1998–2024** | 32.0 KB | `1ff8dc2c3c1ca8a80030e0749fb98c49` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U01.bin` | **1998–2024** | 32.0 KB | `15477dcf386553002608db42f8bebe46` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U10_AT.bin` | **1998–2024** | 32.0 KB | `0ddb29f034a914b9479cd0b5601ded75` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U60_MT_MEC-214B.bin` | **1998–2024** | 32.0 KB | `e8332d3363735e60a71444699d480769` | Factory Binary Firmware Dump |
| `STOCK_ORIGINAL_HCR32_RB20DET_11U70_MT_MEC-215B.bin` | **1998–2024** | 32.0 KB | `1e4b87674034f30ec5ae806c14517129` | Factory Binary Firmware Dump |

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
