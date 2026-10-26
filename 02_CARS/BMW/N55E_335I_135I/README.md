# BMW N55E E-Series MEVD17.2 Powertrain Suite

## 1. Ikhtisar Teknis & Arsitektur
Koleksi biner pabrikan asli OEM dan definisi TunerPro XDF untuk mesin N55 TwinPower Turbo pada sasis E-Series (BMW E90/E92 LCI 335i, E82 135i, E84 X1 35i). Didukung oleh DME Bosch MEVD17.2 (Infineon TriCore TC1797, 4MB ROM).

* **Hardware / ECU**: Bosch MEVD17.2 (Infineon TriCore TC1797, 4MB Flash ROM)
* **Metode Flashing & Antarmuka**: OBD ENET / K+DCAN flashing via MHD N55E atau Bootmod3.
* **Total File Terdaftar**: 6 file (100% fisik terverifikasi, Zero Synthetic)

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

| Filename | Size | MD5 Checksum | Type / Target |
| :--- | :--- | :--- | :--- |
| `98G0B.xdf` | 1.27 MB | `9e41bd8444a21ba82643d2e21489f921` | TunerPro Definition Map |
| `98G0B_MapSwitchBase.bin` | 4.00 MB | `9e8e719ce7428ed61fdf8a9a6aca81ed` | Raw Binary Firmware / Dump |
| `98G0B_original.bin` | 4.00 MB | `94b95fff769240c83d17d24d774f2534` | Raw Binary Firmware / Dump |
| `9E60B.xdf` | 1.28 MB | `d1ece6213353ac9dae67a6d8eea00e3d` | TunerPro Definition Map |
| `9E60B_MapSwitchBase.bin` | 4.00 MB | `a53aafef8d15a6f13cc1115a3feb2565` | Raw Binary Firmware / Dump |
| `9E60B_original.bin` | 4.00 MB | `11e4adddd6070a6ae21626aadb5a8619` | Raw Binary Firmware / Dump |

---

## 3. Panduan Penggunaan & Integritas
1. **Verifikasi Checksum**: Selalu bandingkan hash MD5 file sebelum melakukan flashing ke modul kontrol kendaraan.
2. **Standard Tuning**: Gunakan software TunerPro RT v5.00+ untuk memuat file biner (`.bin`) bersama file definisi (`.xdf`) yang sesuai.
3. **Peringatan Keselamatan**: Pemetaan injeksi bahan bakar dan sudut pengapian harus selalu dipantau dengan wideband AFR gauge dan audio knock detection pada dyno controller berbeban.
