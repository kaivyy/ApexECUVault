# HONDA TRAIL CRF SERIES - ECU Calibration Suite

**Repository Path**: `01_MOTORCYCLES/HONDA/TRAIL_CRF150L_CRF250L`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `23 files` (6 binary/calibration dumps, 17 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `TRAIL_CRF150L_CRF250L` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Dual-Sport, Trail & Motocross Fleet (CRF110F, CRF150L, CRF250L/Rally, CRF450R/HRC) Keihin ECU. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

* **Rentang Tahun / Model Year**: 2012–2024

---

## 2. Manifest Fisik Kalibrasi & Definisi Terverifikasi

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini dengan verifikasi Model Year (Tahun Produksi), ukuran, MD5 checksum, dan tipe platform:

| Filename | Tahun / Model Year | Size | MD5 Checksum | Type / Target Platform |
| :--- | :---: | :--- | :--- | :--- |
| `38770-EKCJ-J000.bin` | **2012–2024** | 256.0 KB | `90d0757c5dbbf71f18c332778f7435df` | Factory Binary Firmware Dump |
| `38770-KYK-D12.bin` | **2012–2024** | 64.0 KB | `f9e963fd1886a39d46f9a8a708b7d320` | Factory Binary Firmware Dump |
| `38770-KYK-D12.xdf` | **2012–2024** | 18.2 KB | `22f4b2a539194b14bc79c4376bf8482b` | TunerPro Binary Definition Map |
| `38770-MEN-E21.bin` | **2012–2024** | 256.0 KB | `796970fd1cdc559a93f9863b2d4e6a5e` | Factory Binary Firmware Dump |
| `38770-MKE-DataSettings.xdf` | **2012–2024** | 23.0 KB | `dc932d513d0e1b3e0bd4c7e5bf3d8ec3` | TunerPro Binary Definition Map |
| `GENERATIONAL_38770-K84-901_Honda_CRF150L_Trail_Dual_Purpose_2017_2025.xdf` | **2017–2025** | 2.5 KB | `281906d4fe2145ce8d4bb1a8e98a99f7` | TunerPro Binary Definition Map |
| `HONDA_38770-K1T-A11_CRF300L___CRF300_Rally_(2021-2024).xdf` | **2021–2024** | 16.3 KB | `5555f7e3491381f5b2da174c0cc328fa` | TunerPro Binary Definition Map |
| `HONDA_38770-K1T-T01_CRF300L___CRF300_Rally_(2021-2024).xdf` | **2021–2024** | 16.3 KB | `1bf812d0211d69f5d7266acd5d5fa8af` | TunerPro Binary Definition Map |
| `HONDA_38770-K84-901_Honda_Generic_ECM.xdf` | **2017–2024** | 16.3 KB | `fafe71a3b36e3b40449ef7de30b5f4b3` | TunerPro Binary Definition Map |
| `HONDA_38770-KYK-D12_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `470af66dd467f5e9135c1d10b0081ab3` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-902_CRF250L___CRF250M___CRF250_Rally.xdf` | **2012–2024** | 16.3 KB | `7c0b752becaaea655c79c35ea353e6ca` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-914_CRF250L___CRF250M___CRF250_Rally.xdf` | **2012–2024** | 16.3 KB | `fd41ef963a87f312870849bd47ba0929` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-A22_CRF250L___CRF250M___CRF250_Rally.xdf` | **2012–2024** | 16.3 KB | `6bbd654e4f10bfa9ed7c178049fe1f20` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-J01_CRF250L___CRF250M___CRF250_Rally.xdf` | **2012–2024** | 16.3 KB | `29d5b844401cc8f7468f1fd0b7351ad0` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-J81_CRF250L___CRF250M___CRF250_Rally.xdf` | **2012–2024** | 16.3 KB | `039593a7dfddead0fc5b5e1d37ea5902` | TunerPro Binary Definition Map |
| `HONDA_38770-KZZ-L41_CRF250L___CRF250M___CRF250_Rally.xdf` | **2012–2024** | 16.3 KB | `dc06414e9651aae93153fa7ca4eab159` | TunerPro Binary Definition Map |
| `HONDA_38770-MKE-A71_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `5f958feddae1be6e2e47b492de506851` | TunerPro Binary Definition Map |
| `HONDA_38770-MKE-A81_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `6479e76f00cea594902c916304c67a97` | TunerPro Binary Definition Map |
| `HONDA_38770-MKE-AF3_Honda_Generic_ECM.xdf` | **2012–2024** | 16.3 KB | `edfa56a9536ba1a751127bae40f861cb` | TunerPro Binary Definition Map |
| `HONDA_38770-MKK-D02_Africa_Twin_CRF1000L___CRF1100L.xdf` | **2011–2016** | 16.3 KB | `1648af151049c525c7824cd80cfc0a34` | TunerPro Binary Definition Map |
| `HONDA_CRF110F_38770_KYK_D12_64KB_ORI.bin` | **2012–2024** | 64.0 KB | `f9e963fd1886a39d46f9a8a708b7d320` | Factory Binary Firmware Dump |
| `HONDA_CRF450R_38770_MEN_E21_256KB_ORI.bin` | **2012–2024** | 256.0 KB | `796970fd1cdc559a93f9863b2d4e6a5e` | Factory Binary Firmware Dump |
| `HONDA_CRF450R_HRC_38770_EKCJ_J000_256KB_ORI.bin` | **2012–2024** | 256.0 KB | `90d0757c5dbbf71f18c332778f7435df` | Factory Binary Firmware Dump |

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 12.5V – 14.0V selama proses penulisan firmware.
