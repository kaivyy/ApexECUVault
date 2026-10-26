# BMW M-Power S63 4.4L Twin-Turbo V8 F10/F90 M5 & M6 Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi biner OEM hardware dump asli dan definisi TunerPro XDF untuk mesin 4.4L Twin-Turbocharged V8 S63B44 (BMW F10 M5, F90 M5, F06/F12/F13 M6, F85 X5M, F86 X6M). Menggunakan ECU Bosch MEVD17.2.H dual-ECU master/slave architecture.

* **Hardware / ECU**: Bosch MEVD17.2.H Dual DME (Master/Slave Tricore 4MB / 8MB Flash ROM)
* **Metode Flashing & Antarmuka**: OBD ENET Flashing via Bootmod3 / MHD atau Bench Boot Tricore Mode.
* **Total File Terdaftar**: 28 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

| Filename | Size | MD5 Checksum | Type / Target |
| :--- | :--- | :--- | :--- |
| `000010CA3B8C01.xdf` | 637.8 KB | `861268aff0abe27b2e1e1c0a106039aa` | TunerPro Definition Map |
| `000010CA3B8C01_original.bin` | 4.00 MB | `0dd83e918f3df32d04c462b535ea0d9e` | Raw Binary Firmware / Dump |
| `000010CA598C01.xdf` | 630.3 KB | `40b2fb3ad1d325d622f69ae1027eaa8a` | TunerPro Definition Map |
| `000010CA598C01_original.bin` | 4.00 MB | `9cfe95ad86ad74f8151117a24d8f3c7f` | Raw Binary Firmware / Dump |
| `00004ACF0A3204.xdf` | 652.5 KB | `e45669d4d52dc60cb6bcc2d4276c0bd1` | TunerPro Definition Map |
| `00004ACF0A3204_original.bin` | 8.00 MB | `1559258c9e0f7fd228e6efa5a999e9c7` | Raw Binary Firmware / Dump |
| `00004ACF147803.xdf` | 658.1 KB | `597d4bfdc8ad2fb5efc492f2482aa481` | TunerPro Definition Map |
| `00004ACF147803_original.bin` | 8.00 MB | `4503527b93e6ce592a9b8595622830ab` | Raw Binary Firmware / Dump |
| `00004ACF1E6E05.xdf` | 652.7 KB | `2af11ea732261b5db6d559bf829bf15f` | TunerPro Definition Map |
| `00004ACF1E6E05_original.bin` | 8.00 MB | `d0427f59c1135ea4ad7d48258455c94b` | Raw Binary Firmware / Dump |
| `00004ACF1E7805.xdf` | 652.7 KB | `d6dc97ead974b74fd3ccac0d6d8a7934` | TunerPro Definition Map |
| `00004ACF1E7805_original.bin` | 8.00 MB | `7f18fe0e6354407fbdf2b5a7133bd19f` | Raw Binary Firmware / Dump |
| `00004ACF1E9605.xdf` | 652.7 KB | `8169ad83c416affb11fc9e7850783ad2` | TunerPro Definition Map |
| `00004ACF1E9605_original.bin` | 8.00 MB | `d768576241ff96359ae416d0d9d181f5` | Raw Binary Firmware / Dump |
| `00004ACF1EA006.xdf` | 652.7 KB | `81e91047b1b1716abec60567ff716733` | TunerPro Definition Map |
| `00004ACF1EA006_original.bin` | 8.00 MB | `11c6ca46da75524b22523e50ab677bb4` | Raw Binary Firmware / Dump |
| `00004ACF1EAA05.xdf` | 652.7 KB | `4df2808f53aa64558113ba51af40cc51` | TunerPro Definition Map |
| `00004ACF1EAA05_original.bin` | 8.00 MB | `975835652e81499e12b19290df85279a` | Raw Binary Firmware / Dump |
| `00004ACF1EB405.xdf` | 652.7 KB | `722a52dae76eede311b47d0656f023a1` | TunerPro Definition Map |
| `00004ACF1EB405_original.bin` | 8.00 MB | `9aebadd1dc558eb08cfe0998d774af8e` | Raw Binary Firmware / Dump |
| `00004ACF286E05.xdf` | 674.0 KB | `2609741adfc5c4b7d4d2312736597cfa` | TunerPro Definition Map |
| `00004ACF286E05_original.bin` | 8.00 MB | `53973a1ccd7cc1f76a2a62f4ea60c224` | Raw Binary Firmware / Dump |
| `00004ACF287806.xdf` | 674.0 KB | `5ef31f1d7441b1f631707ffee1a08f4e` | TunerPro Definition Map |
| `00004ACF287806_original.bin` | 8.00 MB | `4ba04ce3d33efc8b5778600ead64a118` | Raw Binary Firmware / Dump |
| `00004ACF288205.xdf` | 674.0 KB | `8009651bb5cd1a1471b66ee685baba4b` | TunerPro Definition Map |
| `00004ACF288205_original.bin` | 8.00 MB | `cc01cfde49cb1b81baf5b87bdbafd43e` | Raw Binary Firmware / Dump |
| `00004ACF289605.xdf` | 674.0 KB | `91f1f262280ee2dc0736a85c484b837c` | TunerPro Definition Map |
| `00004ACF289605_original.bin` | 8.00 MB | `4d3d4d8ac5a72be4042a9648e209b05e` | Raw Binary Firmware / Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
