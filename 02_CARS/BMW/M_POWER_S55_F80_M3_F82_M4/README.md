# BMW M-Power S55 & N55 F-Series Master Calibration Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi biner OEM factory flash dan TunerPro XDF untuk jajaran performa BMW M-Power S55B30 (F80 M3, F82/F83 M4, F87 M2 Competition / CS) serta mesin N55/N13 F-Series (F30 335i, F20 M135i, 118i). Menggunakan ECU Bosch MEVD17.2.G / MEVD17.2.4 (TriCore TC1797, 4MB Flash ROM).

* **Hardware / ECU**: Bosch MEVD17.2.G / MEVD17.2.4 / MEVD17.2 (Infineon TriCore TC1797 32-bit MCU, 4MB Flash)
* **Metode Flashing & Antarmuka**: OBD2 ENET Flashing via Bootmod3, MHD, atau Kess/K-Tag via Tricore Boot Password mode.
* **Rentang Tahun / Model Year**: 2014–2020
* **Total File Terdaftar**: 41 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `00000D07596401.xdf` | **2014–2020** | 1.12 MB | `54ecc9ce7f7887341ef0024d0efb1d8a` | TunerPro Binary Definition Map |
| `00000D07596401_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `22f4467bf1ea293466a2cf3c97595d66` | Factory Binary Firmware Dump |
| `00000D07596401_original.bin` | **2014–2020** | 4.00 MB | `e5ced22adfcc37ae04010bd1757afcc2` | Factory Binary Firmware Dump |
| `00000E2B3B0A01.xdf` | **2014–2020** | 1021.2 KB | `2a1dfa71bd836d7a926179936ebaeb8d` | TunerPro Binary Definition Map |
| `00000E2B3B0A01_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `c5830c4d9e58945730e26df2a8a51404` | Factory Binary Firmware Dump |
| `00000E2B3B0A01_original.bin` | **2014–2020** | 4.00 MB | `9ec1f0116c862471f366b45274b1b175` | Factory Binary Firmware Dump |
| `00000FEF81A001.xdf` | **2014–2020** | 1.21 MB | `83f1f282b0239d12ac198c9dba23aea8` | TunerPro Binary Definition Map |
| `00000FEF81A001_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `ad12310982ab8aa554d816d48440c553` | Factory Binary Firmware Dump |
| `00000FEF81A001_original.bin` | **2014–2020** | 4.00 MB | `2141d6f1bdb333648c551f0627539991` | Factory Binary Firmware Dump |
| `00001A841D1401.xdf` | **2014–2020** | 1.57 MB | `0a91d5aa1c18f041b51c2168bc6f17fa` | TunerPro Binary Definition Map |
| `00001A841D1401_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `00e722618d0099967cef01acf498edf8` | Factory Binary Firmware Dump |
| `00001A841D1401_original.bin` | **2014–2020** | 4.00 MB | `00fb6d68da0d1da072bdac473f9d24e2` | Factory Binary Firmware Dump |
| `00001A841D2801.xdf` | **2014–2020** | 1.56 MB | `b4a403f71993964061f2e73b7596863f` | TunerPro Binary Definition Map |
| `00001A841D2801_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `2987e6721b32d15a86c419b9b964ffc4` | Factory Binary Firmware Dump |
| `00001A841D2801_original.bin` | **2014–2020** | 4.00 MB | `1dd5c21041f21977d3018fb19d574546` | Factory Binary Firmware Dump |
| `00001C41279601.xdf` | **2014–2020** | 1.21 MB | `85cfb2ad737aa42bfcfb8efb1050e1c6` | TunerPro Binary Definition Map |
| `00001C41279601_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `6cea001165ae87fe938f22281285675d` | Factory Binary Firmware Dump |
| `00001C41279601_original.bin` | **2014–2020** | 4.00 MB | `f580fb866af36e4cf777a65c4f1a0ee0` | Factory Binary Firmware Dump |
| `000021571D8202.xdf` | **2014–2020** | 1.38 MB | `04f0ae0563997b3bfcdfb684ee4ad731` | TunerPro Binary Definition Map |
| `000021571D8202_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `0e1e9492e73620de9ccf62b143aa736f` | Factory Binary Firmware Dump |
| `000021571D8202_original.bin` | **2014–2020** | 4.00 MB | `f366030dba59706a62ab3befa574750a` | Factory Binary Firmware Dump |
| `000021571DAA01.xdf` | **2014–2020** | 1.40 MB | `122abda26161d631f7c47e4bf1b3d34d` | TunerPro Binary Definition Map |
| `000021571DAA01_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `13e3c907a38db3bf1bf02502df7aee98` | Factory Binary Firmware Dump |
| `000021571DAA01_original.bin` | **2014–2020** | 4.00 MB | `f79e479bdcde078a4ad6c6ce37adbfdc` | Factory Binary Firmware Dump |
| `000021571DBE01.xdf` | **2014–2020** | 1.40 MB | `9650d306df275b381cfff6c43d77c00a` | TunerPro Binary Definition Map |
| `000021571DBE01_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `f33f8fd2aa2b1ed7ea02e700f384db05` | Factory Binary Firmware Dump |
| `000021571DBE01_original.bin` | **2014–2020** | 4.00 MB | `8852385a6d9953eceff1e570e7d3b0e0` | Factory Binary Firmware Dump |
| `00002DF2132801.xdf` | **2014–2020** | 1.32 MB | `f5d6913ee2ecc1bcb137a42a96c7560e` | TunerPro Binary Definition Map |
| `00002DF2132801_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `09238e53da6a3fe2f1e0d73dac479b6d` | Factory Binary Firmware Dump |
| `00002DF2132801_original.bin` | **2014–2020** | 4.00 MB | `b5f8af6342fa39902c1f2126e4011086` | Factory Binary Firmware Dump |
| `00005BA8134601.xdf` | **2014–2020** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |
| `00005BA8134601_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `df04508b920e9b79d08c44afd9b4deae` | Factory Binary Firmware Dump |
| `00005BA8134601_original.bin` | **2014–2020** | 4.00 MB | `849a1be62b6ca75aede391ad419d2a73` | Factory Binary Firmware Dump |
| `00005BA8135001.xdf` | **2014–2020** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |
| `00005BA8135001_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `033bc84fddd71ecfee6d466bceaaf67f` | Factory Binary Firmware Dump |
| `00005BA8135001_original.bin` | **2014–2020** | 4.00 MB | `1a1d5d8d08827fd68e18ce91fc4fca9d` | Factory Binary Firmware Dump |
| `00005BA8135A01.xdf` | **2014–2020** | 1.60 MB | `b40b2d66c96ec5f8d8a69cdaebd22dc9` | TunerPro Binary Definition Map |
| `00005BA8135A01_MapSwitchBase.bin` | **2014–2020** | 4.00 MB | `3401426fa2c085eac040c4d80ae678dc` | Factory Binary Firmware Dump |
| `00005BA8135A01_original.bin` | **2014–2020** | 4.00 MB | `28c681bd80da47f4fe54508af611d83f` | Factory Binary Firmware Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
