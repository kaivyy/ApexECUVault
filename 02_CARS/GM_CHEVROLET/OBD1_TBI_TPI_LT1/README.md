# General Motors OBD1 TBI / TPI / LT1 Master Factory BCC Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi biner kalibrasi Broadcast Code (BCC) asli pabrikan General Motors untuk ECU OBD1 (1227747, 1227165, 16197427, 16188051) pada mesin Chevrolet 4.3L V6, 5.0L V8 305, 5.7L V8 350 Small Block TBI/TPI, serta 5.7L LT1. Dilengkapi file definisi TunerPro XDF ($42, $6E, $8D, $DA, $EE).

* **Hardware / ECU**: GM Delco OBD1 ECM/PCM (2732A 4KB, 27C128 16KB, 27C256 32KB, 27C512 64KB EPROM)
* **Metode Flashing & Antarmuka**: EPROM burner / Moates AutoProm / TunerPro RT ALDL cable.
* **Total File Terdaftar**: 28 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

| Filename | Size | MD5 Checksum | Type / Target |
| :--- | :--- | :--- | :--- |
| `2240AYFP.BIN` | 64.0 KB | `0b4b86ec7594e0183ebfc9e1b529a857` | Raw Binary Firmware / Dump |
| `ANZA.bin` | 16.0 KB | `bac00c6ed052846369efa5c632a1b0c4` | Raw Binary Firmware / Dump |
| `APYP.bin` | 16.0 KB | `dc9f6c758832e709320553b96b3f6fb8` | Raw Binary Firmware / Dump |
| `ARAP.bin` | 16.0 KB | `85c39ceefcee8f26ce8f41168ed6992c` | Raw Binary Firmware / Dump |
| `AYCF6730 88.BIN` | 32.0 KB | `a49fcfe4b2c67b24256328cf5fd3cf76` | Raw Binary Firmware / Dump |
| `Abyr4326 88.bin` | 32.0 KB | `156f5391abed9852f2a7999a301135bf` | Raw Binary Firmware / Dump |
| `Arpl 88.bin` | 32.0 KB | `b6293a0cc5a7c513ffd8fe82d0fa6485` | Raw Binary Firmware / Dump |
| `Atj9188 88.bin` | 32.0 KB | `65fe2a269b4b7cbac400bd0118ffdf64` | Raw Binary Firmware / Dump |
| `Atmf5241 88.bin` | 32.0 KB | `65e7e153b933d7b9af566dfa6770422b` | Raw Binary Firmware / Dump |
| `Atta6656 88.bin` | 32.0 KB | `8e646d563a32dfd713155e9b3959a0ee` | Raw Binary Firmware / Dump |
| `BCKC 11.BIN` | 64.0 KB | `52d88f2ffcf9630c4560d92f47604474` | Raw Binary Firmware / Dump |
| `BDJZ.bin` | 64.0 KB | `31cbe8ad8ccbab03a24787928f762ecc` | Raw Binary Firmware / Dump |
| `BFFK1287.BIN` | 64.0 KB | `a8c2ab8e49fd0402164819f4807c7734` | Raw Binary Firmware / Dump |
| `BFPL2416.BIN` | 64.0 KB | `c9a80d556704e96fa2b06663eb78d85b` | Raw Binary Firmware / Dump |
| `BFPM 12.BIN` | 32.0 KB | `28e6ab94694bad544b53d6d68e9f2dd9` | Raw Binary Firmware / Dump |
| `BFUZ.BIN` | 32.0 KB | `5a7cdbc25d430724d61906c7f2834b2f` | Raw Binary Firmware / Dump |
| `BJKT8015.BIN` | 64.0 KB | `1c9d1937ba86908b182d468216860cf8` | Raw Binary Firmware / Dump |
| `BJLK.bin` | 64.0 KB | `f14dc08de58013df597011e4f0f4b46d` | Raw Binary Firmware / Dump |
| `BJWN.Bin` | 64.0 KB | `fb048a75993bb5b969b078de9dd3ca26` | Raw Binary Firmware / Dump |
| `BJYM 0D.bin` | 64.0 KB | `425f3fe075126c6b7b69356995a7c58e` | Raw Binary Firmware / Dump |
| `BLCH5094.BIN` | 64.0 KB | `bf1c366592be7e6b161b258c6d293cf8` | Raw Binary Firmware / Dump |
| `BLYN8253.BIN` | 64.0 KB | `bfbfc78db8684b70c6e02dcfbee29a5b` | Raw Binary Firmware / Dump |
| `Bawx 88.bin` | 32.0 KB | `3d57b6b1ff7239945502b15e6044e03f` | Raw Binary Firmware / Dump |
| `Cld4324 88.bin` | 32.0 KB | `c58fa5f508ebb77a6383f984cfc448ff` | Raw Binary Firmware / Dump |
| `atds 88.bin` | 32.0 KB | `93b872e21e2a286e8145314d1c2086ef` | Raw Binary Firmware / Dump |
| `azty1407 88.bin` | 32.0 KB | `d665d66733b1379580f17fbeebee6788` | Raw Binary Firmware / Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
