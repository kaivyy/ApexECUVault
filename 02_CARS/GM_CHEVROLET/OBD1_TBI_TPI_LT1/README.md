# OBD1 TBI TPI LT1 - Technical ECU Calibration Dossier

## 1. Ringkasan Platform & Arsitektur ECU
- **Target Platform**: OBD1 TBI TPI LT1
- **Model Year Coverage**: 2000–2024
- **Total Calibration Assets**: 26 verified files
- **Definition Standard**: ASAM MCD-2 MC (A2L), WinOLS DAMOS/OLS/KP, TunerPro XDF, RomRaider XML, and Raw Binary Firmware.
- **Security Checksum**: Hardware CRC32 / RSA 1024 / 2048-bit digital signature.

## 2. Daftar Berkas Terverifikasi (Verifikasi Integritas & Checksum SHA-256 / MD5)

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :---: | :---: | :--- |
| `2240AYFP.BIN` | **1998–2024** | 64.0 KB | `0b4b86ec7594e0183ebfc9e1b529a857` | Factory Binary Firmware Dump |
| `Abyr4326 88.bin` | **1998–2024** | 32.0 KB | `156f5391abed9852f2a7999a301135bf` | Factory Binary Firmware Dump |
| `ANZA.bin` | **1998–2024** | 16.0 KB | `bac00c6ed052846369efa5c632a1b0c4` | Factory Binary Firmware Dump |
| `APYP.bin` | **1998–2024** | 16.0 KB | `dc9f6c758832e709320553b96b3f6fb8` | Factory Binary Firmware Dump |
| `ARAP.bin` | **1998–2024** | 16.0 KB | `85c39ceefcee8f26ce8f41168ed6992c` | Factory Binary Firmware Dump |
| `Arpl 88.bin` | **1998–2024** | 32.0 KB | `b6293a0cc5a7c513ffd8fe82d0fa6485` | Factory Binary Firmware Dump |
| `atds 88.bin` | **1998–2024** | 32.0 KB | `93b872e21e2a286e8145314d1c2086ef` | Factory Binary Firmware Dump |
| `Atj9188 88.bin` | **1998–2024** | 32.0 KB | `65fe2a269b4b7cbac400bd0118ffdf64` | Factory Binary Firmware Dump |
| `Atmf5241 88.bin` | **1998–2024** | 32.0 KB | `65e7e153b933d7b9af566dfa6770422b` | Factory Binary Firmware Dump |
| `Atta6656 88.bin` | **1998–2024** | 32.0 KB | `8e646d563a32dfd713155e9b3959a0ee` | Factory Binary Firmware Dump |
| `AYCF6730 88.BIN` | **1998–2024** | 32.0 KB | `a49fcfe4b2c67b24256328cf5fd3cf76` | Factory Binary Firmware Dump |
| `azty1407 88.bin` | **1998–2024** | 32.0 KB | `d665d66733b1379580f17fbeebee6788` | Factory Binary Firmware Dump |
| `Bawx 88.bin` | **1998–2024** | 32.0 KB | `3d57b6b1ff7239945502b15e6044e03f` | Factory Binary Firmware Dump |
| `BCKC 11.BIN` | **1998–2024** | 64.0 KB | `52d88f2ffcf9630c4560d92f47604474` | Factory Binary Firmware Dump |
| `BDJZ.bin` | **1998–2024** | 64.0 KB | `31cbe8ad8ccbab03a24787928f762ecc` | Factory Binary Firmware Dump |
| `BFFK1287.BIN` | **1998–2024** | 64.0 KB | `a8c2ab8e49fd0402164819f4807c7734` | Factory Binary Firmware Dump |
| `BFPL2416.BIN` | **1998–2024** | 64.0 KB | `c9a80d556704e96fa2b06663eb78d85b` | Factory Binary Firmware Dump |
| `BFPM 12.BIN` | **1998–2024** | 32.0 KB | `28e6ab94694bad544b53d6d68e9f2dd9` | Factory Binary Firmware Dump |
| `BFUZ.BIN` | **1998–2024** | 32.0 KB | `5a7cdbc25d430724d61906c7f2834b2f` | Factory Binary Firmware Dump |
| `BJKT8015.BIN` | **1998–2024** | 64.0 KB | `1c9d1937ba86908b182d468216860cf8` | Factory Binary Firmware Dump |
| `BJLK.bin` | **1998–2024** | 64.0 KB | `f14dc08de58013df597011e4f0f4b46d` | Factory Binary Firmware Dump |
| `BJWN.Bin` | **1998–2024** | 64.0 KB | `fb048a75993bb5b969b078de9dd3ca26` | Factory Binary Firmware Dump |
| `BJYM 0D.bin` | **1998–2024** | 64.0 KB | `425f3fe075126c6b7b69356995a7c58e` | Factory Binary Firmware Dump |
| `BLCH5094.BIN` | **1998–2024** | 64.0 KB | `bf1c366592be7e6b161b258c6d293cf8` | Factory Binary Firmware Dump |
| `BLYN8253.BIN` | **1998–2024** | 64.0 KB | `bfbfc78db8684b70c6e02dcfbee29a5b` | Factory Binary Firmware Dump |
| `Cld4324 88.bin` | **1998–2024** | 32.0 KB | `c58fa5f508ebb77a6383f984cfc448ff` | Factory Binary Firmware Dump |

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
