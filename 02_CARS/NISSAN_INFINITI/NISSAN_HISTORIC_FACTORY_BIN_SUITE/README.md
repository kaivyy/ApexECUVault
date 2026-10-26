# NISSAN & INFINITI - Historic Factory Binary Master Suite (RB26, SR20, VG30, VQ30, CA18, TB45)

**Repository Path**: `02_CARS/NISSAN_INFINITI/NISSAN_HISTORIC_FACTORY_BIN_SUITE`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `453 files` (453 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Koleksi master bersejarah terlengkap 453 berkas biner firmware pabrikan asli (.bin/.ori/.hex) untuk jajaran mesin performa dan komersial legendaris Nissan dan Infiniti: RB-Series (Skyline GT-R BNR32/BCNR33/BNR34 RB26DETT, ECR33/ER34 RB25DET, HCR32 RB20DET), SR-Series (Silvia S13/S14/S15 SR20DET, Pulsar GTi-R RNN14, Primera P10/P11 SR20DE), VG/VQ-Series (Fairlady Z 300ZX Z31/Z32 VG30DETT, Cefiro A31/A32 VQ30DE, Cedric/Gloria Y32/Y33 VQ30DET), CA-Series (Silvia S12/S13 CA18DET, Bluebird U12), dan Patrol/Safari (Y60 TB42E, Y62 TB45E, Q45 VH45DE V8). Setiap berkas merefleksikan pembacaan hardware murni untuk verifikasi checksum Consult dan modifikasi peta EPROM.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Nissan / JECS / Hitachi M-Series Engine Control Module`
- **Arsitektur MCU & Memori**: `Hitachi 6303 / 68HC11 / H8/534 / H8/536 / SuperH SH7055 (32KB / 64KB / 512KB ROM)`
- **Protokol Diagnostik & Flashing**: `Nissan Consult I (DDL 9600 bps K-Line) / Consult II (ISO 14230 KWP2000) / Direct EPROM Read`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **OEM Part Numbers** (misal `0261xxxxxx`, `12587603`, `38770-xxx`, `23710-xxxxx`): Standar identifikasi universal pabrikan untuk ECU dan nomor perakitan modul.
- **Operating System / Software IDs** (misal `52373027`, `12592618`, `BG11_ECE_HS_008`, `PY3-A02`): Alamat dan software baseline pabrik yang tertanam di blok memori ROM.
- **TunerPro XDF Maps & A2L Definitions**: File deskriptor matematis yang memetakan offset memori hex ke unit engineering nyata (RPM, ms injeksi, derajat pengapian, kPa, persen bukaan katup).

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **EcuFlash**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `92Pathfinder.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A31_RB20DET_5L210_MEC-R330_AT.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A31_RB20DET_73L00_R102D_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A31_RB20DET_73L10_MEC-R103D_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A31_RB20DET_94L10_MEC113_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A31_RB20DE_72L00_MEC-R100d_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A31_RB20DE_72L10_MEC-R101D_MT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_0L701_MT_1997.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_40U01_1995_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_40U03_1995_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_40U11_1995_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_40U11_1995_AT_maps.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_40U13_1995_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_40U13_1995_AT_maps.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_49U10_1995_AT_consult.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_54U00_1996_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_54U01_1996_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_54U03_1996_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_54U11_1996_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `A32_VQ30DE_54U13_1996_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_E16E_79Y05_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_GA16DE_73Y05_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_GA16DE_81R00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_GA16DE_81R05_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_64Y00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_64Y01_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_64Y02.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_64Y15_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_67Y00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_70Y05_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_71Y00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_71Y05_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_78C20.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B13_SR20DE_94Y00.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_GA16DE_0M201_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_GA16DE_0M272_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_GA16DE_2M000_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_0M761_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_0M765_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_1M860_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_1M861_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_1M871_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_1M876_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_2M080.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_4M201.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `B14_SR20DE_xxxxx.BIN` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `BNCR33_RB26DETT_24U00.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `BNR32_RB26DETT_05U02_MT_MECR128.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `BNR32_RB26DETT_05U03_MT_MEC-R138.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `BNR32_RB26DETT_05U60_MT_MECR280.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `BNR32_RB26DETT_05U61_MT_MECR281.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `BNR32_RB26DETT_05U62_MT_MECR282A.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `C23_SR20DE_2C000_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `C33_RB20DE_71L60_ MT_DEB7.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `C33_RB20DE_72L70_AT_MEC-R201B.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `C35_RB25DET_8L302.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `CR31_RB30E_J7100_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `CR31_RB30E_J7110_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `D21_KA24DE_1993_MT_FED.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `D21_KA24E_76P00_MECMT113.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `D21_KA24E_86G01_MECMT110.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `D21_KA24E_MECMT122.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `D21_VG30E_MECM-V131.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR32_FOR_RB25_08U01_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR32_RB25DE_08U01_MT_MEC-R232.Bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR32_RB25DE_08U02_MT.Bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR32_RB25DE_08U11_AT.Bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_13U00_MT_MEC-R720.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_13U01_MT_MEC-R260.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_21U00_MT_MECR520.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_21U01_MT_MECR521_daughterboard.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_21U02_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_21U03.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_21U11_AT_MECR531.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_21U60_MT_MECR530.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DET_21U70.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DE_17U14_AT_MECR514.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ECR33_RB25DE_28U00_MT_MEC-R700.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `EFK10_MA09ET_37B10.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `EK10_MA09ERT_21B00_MT_T104ADM6.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `EK10_MA09ERT_Nismo.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `EK10_MA09ERT_STOCK_EK10009518.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ENR33_RB20E_29U10_MECR750_1997.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ENY34_VQ30DE_AG500.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA500_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA501_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA502_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA510_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA511_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA512_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA513_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA560_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `ER34_RB25DET_AA570_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `F31_VG20DET_F6371_MECE55.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `G20_P10_SR20DE_0J200_MT_1994.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `G20_P10_SR20DE_0J202_MT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `G20_P10_SR20DE_0J203_MT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `G20_P10_SR20DE_0J212_AT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `G20_P10_SR20DE_0J600_MT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `G20_P10_SR20DE_0J610_AT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HB14_SR18DE_0M801.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HB14_SR18DE_0M811.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_01U01_MEC-R124.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_04U00_MT_MEC-R106.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_04U01_MT_MEC-R126.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_04U02_MT_MEC-R132.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_04U11_AT_MECR109.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_04U12_AT_MECR127.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_04U60_MT_GTS4.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_04U70_AT_GTS4_MEC-R117.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_10U01_MEC-R210B.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_10U11_MEC-217.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_11U00_MT_MEC-212B.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_11U01.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_11U10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_11U60_MT_MEC-214B.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HCR32_RB20DET_11U70_MT_MEC-215B.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_45L70_AT_MEC-R50C.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_56S13_AT_J171ADA3.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_58S12_AT_MECR12.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_59S03_MT_MEC-R16.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_59S13_AT_MEC-R17.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_70S00_MEC-R45.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_79S01_MEC-R40.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_80503_MT_MEC-R72R_bottom.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_80S01_MEC-R42.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_80S11_AT_MEC-R43.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_80S12_MECR48.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_MEC-R37.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20DET_MEC-R49_Autech.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR31_RB20ET_76S10.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `HR33_RB20E_26U00.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `J30_VE30DE_97E10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `J30_VE30DE_97E60_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `J30_VG30DE_17Y11.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `J30_VG30E_87E00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `J30_VG30E_98E00_MT_E255FFM2.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `J30_VG30_87E05_MT.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `J30_VG30_E255efm7.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG10DE_0U000k.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG10DE_0U400_MT_late_64KB.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG10DE_1U210_64KB.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG10DE_41B10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG10DE_72B01_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_1U203_64KB.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_44B00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_71B00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_74B01_late_64KB.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_74B61_late_64KB.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_99B00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_99B05_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_99B16_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_99B60_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `K11_CG13DE_99B65_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `KN13_CA18DE_02Y01_MT_USDM_1989_Fed.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `KN13_CA18DE_02Y03_MT_USDM_1988_Fed.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `M30_VG30_F6610_K255AFA6.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `M30_VG30_F6610_TB45MAPS.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `M30_VG30_F6615_AT_1990.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `M30_VG30_F6670_AT_1991.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `M30_VG30_F6675_AT_1991.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N12_E15ET_28M04_MT_N306P5T1.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N12_E15ET_28M04_MT_V2.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N13_CA16DE_64M00_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N13_CA16DE_65M00_CA18DE.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N13_CA16DE_82M00_MT_MEC-410_1987.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N14_GA16DE_65C05.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N14_SR18DE_58Y01_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N14_SR20DE_68C00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N14_SR20DE_68C10_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N15A_GA16DE_1N900_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N15A_GA16DE_1N910_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N15_SR20DE_0A540_autech.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N15_SR20DE_1N401_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N15_SR20DE_1N410_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N15_SR20DE_1N411_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `N15_SR20DE_1N960_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR18DE_0J312_AT.Bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_0J261_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_5J000_MT_1993.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_62J00_MT_1991.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_63J11_AT_1991.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_70J00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_70J10_AT_1993.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_70J15_AT_1993.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_71C00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_77J00_MT_1992.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_83J00_MT_1994.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_83J10.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DE_83J14.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P10_SR20DI_70J81_1992.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR18DE_79J71.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_2J200_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J400.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J403_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J404.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J461_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J501_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J503_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J504_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J800_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J801_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_3J905_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `P11_SR20DE_7J100_1999_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `PW10_SR20DE_78N05.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_60U00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_61U00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_62U00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U01_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U04_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U05_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U06_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U07_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U08_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U09_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U12_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U21.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U61_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_64U65_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_66U15_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_71U04_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Q45_VH45DE_71U12_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `R30_FJ20DET_R2201_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `RNN14_SR20DET_54C00_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `RNN14_SR20DET_54C60_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `RNN14_SR20DET_69C05_MT_EDM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `RNU12_CA18DET_MT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `RS13_CA18DET_36F05_MT_MEC-D016B_JDM.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `RS13_CA18DET_36F11_MT_MEC-D015A_JDM.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `RS13_CA18DET_36F15_MT_MEC-D017B_JDM.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S12_CA18ET_21F13_c321aem4.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S12_CA18ET_30F00_MT_MEC-450.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S12_CA18ET_30F10_AT_MEC-550.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S12_CA18ET_33F01.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DET_36F00_MEC-D003E2_JDM_MT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DET_39F00_MEC-D007D_EDM_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DET_44F02_MT_MEC-D005B.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DET_44F06_MT_MEC-D022A.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DET_44F07_MT_MEC-D009D.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DET_MEC-D010C.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DE_35F00_MEC-D001_JDM_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DE_35F11_MEC-D014.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18DE_35F11_MEC-R015_JDM_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_CA18ET_D4600_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_51F11.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_53F00_MT_1991_FED.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_53F01_MT_1993_FED.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_53F10_AT_1991.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_53F11_MT_1991_FED.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_54F00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_54F02_MT.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_54F10_AT_CAL.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_54F12_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_59F10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_59F12_AT_1994_FED.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24DE_59F16_AT_CAL.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24E_40F0X_1990_MT_FED.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24E_42F61_89_AT_CALI.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24E_42F62_89_AT_CALI.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_KA24E_42F65_89_AT_CALI.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_50F00_MT_red_top.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_50F01_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_50F05_MT_black_top.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_50F10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_50F11_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_50F15_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_60F06_MT_TypeX.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_60F07_TypeX.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DET_60F16_TypeX.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DE_52F00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DE_52F10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DE_60F00_TypeS.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S13_SR20DE_60F10_TypeS.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_70F00_MT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_70F01_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_70F02.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_70F03_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_70F05_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_70F06.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_70F08_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_70F10_AT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_72F01_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_KA24DE_72F13_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_69F00_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_69F01_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_69F10.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_74F00_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_74F01_MT.BIN` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_74F05_MT.BIN` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_74F05_s14a-wiring.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_74F10_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_74F11_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_74F15_s14a-wiring.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_75F00_MT_NATS_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_75F01_MT_NATS_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_75F10_AT_NATS_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_80F00_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_80F10_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F00_MT_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F01_MT_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F04_MT_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F05_MT_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F06_MT_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F08_MT_EDM.BIN` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F14_AT_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F15_AT_EDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_82F18_MT_EDM.BIN` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_83F00_MT_ADM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_83F05.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DET_83F10_AT_ADM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DE_65F00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DE_65F00_MT_knockadj.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S14_SR20DE_65F10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_91F00_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_91F01_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_91F05_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_91F06_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_91F07_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_91F08_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_91F10_AT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_91F15_AT_JDM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_93F00_MT_ADM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `S15_SR20DET_93F10_AT_ADM.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U11_VG30E_56U62.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_CA18DET_56E62_MEC-C006C.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_CA18DET_56E70_MEC-C006.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_KA24E_65E01.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_KA24E_65E14.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_KA24E_95E03_E480AAM6.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_KA24E_95E11.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_SR20DET_5E200_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_SR20DET_79E01_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_SR20DET_79E10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U12_SR20DET_79E11_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U13_KA24DE_1E460_1993_MT_Altima.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U13_KA24DE_1E470_1993_AT_Altima.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U13_KA24DE_3E600_1994_JDM_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U13_KA24DE_4E800_1995_FED_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U13_SR20DET_1E000_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U13_SR20DET_1E010.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `U13_SR20DET_4E610_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `UC32-VG30E.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `VL_RB30ET_B4903_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `VL_RB30ET_B4913_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `VL_RB30E_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `VL_RB30E_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `W10_SR20DET_95N11.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `W10_SR20DET_95N15.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_0V810_4WD_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_0V811_4WD_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_0V812_4WD_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_0V813_4WD_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_23710_0V800_4WD_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_23710_0V801_4WD_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_23740_0V800_2WD_AT.BIN` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_23740_0V802_2WD_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `WC34_RB25DET_23740_0V810_4WD_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y30_VG30ET_MECV16.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y31_VG20DET_71V10_AT_MECE101.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y31_VG30DET_71V70_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y32_VG30DET_0P501_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y32_VG30DET_0P602_MT_1992_Gloria.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y32_VG30DET_OP660.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y32_VH41DE_1P121-Tuned.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y33_VQ30DET_4P200_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y33_VQ30DET_4P201_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y33_VQ30DET_4P202_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y33_VQ30DET_4P203_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y33_VQ30DET_5P710_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y33_VQ30DET_5P711_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y33_VQ30DET_6P500_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y33_VQ30DET_6P501_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y60_TB42E_35J00_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y60_TB42E_35J01_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y60_TB42E_35J10_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Y62_TB45E_VB716.BIN` | `Original OEM Binary Flash Dump` | 65,152 | Berkas biner firmware resmi pabrikan (65,152 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_RB20DET_20P61_MEC_R62_MT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_RB20DET_20P70_MEC_R61_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1984_02P02_MT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1984_02P03_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1984_02P07_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1984_07P00_MT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1984_10P00_MT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1986_19P12_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1987_21P01_MT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1987_21P11_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1988_26P00_MT_SS.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1988_26P01_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30ET_1988_26P10.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1984_01P00_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1984_06P01_MT.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1984_06P11_AT.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1984_06P15_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1984_10P00_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1986_18P03_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1986_18P07_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1986_18P18_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1986_21P66_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1988_25P00_MT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1988_25P10_AT.bin` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z31_VG30E_1988_NA_CA.BIN` | `Original OEM Binary Flash Dump` | 16,384 | Berkas biner firmware resmi pabrikan (16,384 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_FOR_RB25DET_41P03_MT_v3.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_FOR_RB25DE_41P03_MT_S2_v3.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_1989_NA_AT_M257ACA8.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_30P10.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_31P02_1990_MT_FED.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_31P03_1990_MT_FED.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_31P08_1990_MT_CALI.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_31P11.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_31P12.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_37P01_1991_1993_MT_EDM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_37P06_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_37P11_AT_1992_EDM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P01_AT_1990_JDM_M4.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P02_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P03_MT_JDM.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P04_MT_1991_JDM.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P11_AT_TXC_661.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P12_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P13_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P14_JDM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P60_MT_1992.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_41P70_MT.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_47P10_MT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_48P01_MT_1991.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_48P76.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_49P71.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_51P00_MT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_51P05_MT_1995.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_51P60_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_51P65_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_51P70.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DETT_54P00_1996_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_30P00_1990_NA_MT_FED.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_30P60_1990_NA_MT_FED.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_30P75_1991_NA_AT.BIN` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_39P00_1990_NA_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_39P12_1990_NA_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_39P12_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_40P01_1991_NA_MT_JDM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_40P13_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_45P05_1993_NA_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_45P15_1993_NA_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_46P10_1992_AT_ADM.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_46P80_1992_AT.bin` | `Original OEM Binary Flash Dump` | 32,768 | Berkas biner firmware resmi pabrikan (32,768 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_50P06.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_50P76_1994_NA_AT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_52P05.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_53P00_NA_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_53P05_NA_MT.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |
| `Z32_VG30DE_AT_49P66.bin` | `Original OEM Binary Flash Dump` | 65,536 | Berkas biner firmware resmi pabrikan (65,536 bytes) hasil hardware read murni (Zero-Synthetic) |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, MAF/MAP Transfer Functions, Smoke Limiter, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance independen, High/Low Octane Timing Tables, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow, Boost & Cam Phasing**: Target Boost Pressure, Wastegate Duty Cycle (WGDC), Electronic Throttle Valve (Drive-by-Wire) Angle, dan Variable Cam Phasing (VANOS, VTC, VTEC).
- **Safety Limits & Thresholds**: Rev Limiter (Hard & Soft Cut), Top Speed Limiter (Vmax), Overboost Protection, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
