# CIVIC 1.8L 2.0L R18 K20 - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CIVIC_1_8L_2_0L_R18_K20`  
**Classification**: `Hybrid Binary & TunerPro Definition Suite`  
**Total Managed Assets**: `311 files` (1 binary/calibration dumps, 310 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `CIVIC_1_8L_2_0L_R18_K20` menyediakan pustaka kalibrasi dan pemetaan ECU profesional untuk Honda Civic 1.8L & 2.0L (R18A / R18Z / K20Z) Engine Management Platform. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID) untuk menjaga kecocokan header pada TunerPro dan alat flasher.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805--13-A020_37805--13-A020.xdf` | `.XDF` | `173,829` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-3050-CVT_37805-3050-CVT.xdf` | `.XDF` | `56,806` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AA-A120_37805-5AA-A120.xdf` | `.XDF` | `105,896` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AF-B420_37805-5AF-B420.xdf` | `.XDF` | `95,229` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5AN-CC10_37805-5AN-CC10.xdf` | `.XDF` | `100,337` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5BF-A050_37805-5BF-A050.xdf` | `.XDF` | `125,752` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5BF-A230_37805-5BF-A230.xdf` | `.XDF` | `120,426` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5BF-E030_37805-5BF-E030.xdf` | `.XDF` | `115,900` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5G0-A370_37805-5G0-A370.xdf` | `.XDF` | `72,310` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5PA-7740_37805-5PA-7740.xdf` | `.XDF` | `41,275` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5PA-CC10_37805-5PA-CC10.xdf` | `.XDF` | `42,988` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5YF-AD20_37805-5YF-AD20.xdf` | `.XDF` | `50,626` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-5YF-C420_37805-5YF-C420.xdf` | `.XDF` | `50,626` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-64A-A540_37805-64A-A540.xdf` | `.XDF` | `118,511` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-64B-A010_37805-64B-A010.xdf` | `.XDF` | `95,039` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-64L-J020_37805-64L-J020.xdf` | `.XDF` | `119,620` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-64L-J530_37805-64L-J530.xdf` | `.XDF` | `119,100` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PCX-U120_37805-PCX-U120.xdf` | `.XDF` | `1,568` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PHM -A630.rwd_37805-PHM_-A630.rwd.xdf` | `.XDF` | `1,578` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PHM-4050.rwd_37805-PHM-4050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-3170.rwd_37805-PLM-3170.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-3360_Honda_Civic_2001_DX__LX_1.7L__L4_-_Gas.xdf` | `.XDF` | `1,594` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-3390.rwd_37805-PLM-3390.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-4050.rwd_37805-PLM-4050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-4170.rwd_37805-PLM-4170.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-4260.rwd_37805-PLM-4260.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-4390.rwd_37805-PLM-4390.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-A150-M1.rwd_37805-PLM-A150-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-A760-M1.rwd_37805-PLM-A760-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-C150-M1.rwd_37805-PLM-C150-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLM-C760-M1.rwd_37805-PLM-C760-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-3150.rwd_37805-PLR-3150.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-3170.rwd_37805-PLR-3170.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-3360.rwd_37805-PLR-3360.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-3390.rwd_37805-PLR-3390.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-4050.rwd_37805-PLR-4050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-4170.rwd_37805-PLR-4170.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-4260.rwd_37805-PLR-4260.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-4390.rwd_37805-PLR-4390.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-A130-M1.rwd_37805-PLR-A130-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-A750-M1.rwd_37805-PLR-A750-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-C130-M1.rwd_37805-PLR-C130-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PLR-C750-M1.rwd_37805-PLR-C750-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMM-3170.rwd_37805-PMM-3170.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMM-3390.rwd_37805-PMM-3390.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMM-4050.rwd_37805-PMM-4050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMM-4170.rwd_37805-PMM-4170.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMM-4260.rwd_37805-PMM-4260.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMM-4390.rwd_37805-PMM-4390.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-3050.rwd_37805-PMP-3050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-3060_Honda_Civic_2001_HX_1.7L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-3070.rwd_37805-PMP-3070.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-3090.rwd_37805-PMP-3090.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-4050.rwd_37805-PMP-4050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-4060.rwd_37805-PMP-4060.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-4170_Honda_Civic_2003_HX_1.7L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-4190_Honda_Civic_2002_HX_1.7L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-A130_Honda_Civic_2002_HX_1.7L__L4_-_Gas.xdf` | `.XDF` | `1,590` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMP-A830-M1.rwd_37805-PMP-A830-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMR-3170.rwd_37805-PMR-3170.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMR-3390.rwd_37805-PMR-3390.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMR-4050.rwd_37805-PMR-4050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMR-4170.rwd_37805-PMR-4170.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMR-4260.rwd_37805-PMR-4260.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMR-4390.rwd_37805-PMR-4390.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMS-A660-M1.rwd_37805-PMS-A660-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PMS-A680_Honda_Civic_2003_GX_1.7L__L4_-_CNG.xdf` | `.XDF` | `1,590` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PND-3050_Honda_Civic_2004_2005_GX_1.7L__L4_-_CNG.xdf` | `.XDF` | `1,595` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PND-3060.rwd_37805-PND-3060.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PND-3070.rwd_37805-PND-3070.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PNF-A060-M1.rwd_37805-PNF-A060-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PPA-3050.rwd_37805-PPA-3050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PPA-3180.rwd_37805-PPA-3180.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PPA-4260.rwd_37805-PPA-4260.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PRB-3050.rwd_37805-PRB-3050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PRB-A080-M1.rwd_37805-PRB-A080-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PVJ-X560-M1.rwd_37805-PVJ-X560-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PVJ-X810-M1.rwd_37805-PVJ-X810-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PVJ-X910-M1.rwd_37805-PVJ-X910-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PVJ-Y530-M1.rwd_37805-PVJ-Y530-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PVJ-Y550-M1.rwd_37805-PVJ-Y550-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PWG-3050.rwd_37805-PWG-3050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PWG-3060.rwd_37805-PWG-3060.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZA-3050.rwd_37805-PZA-3050.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZA-3280.rwd_37805-PZA-3280.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZA-3290.rwd_37805-PZA-3290.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZA-4060.rwd_37805-PZA-4060.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZA-4280.rwd_37805-PZA-4280.rwd.xdf` | `.XDF` | `1,576` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZA-A170-M1.rwd_37805-PZA-A170-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZA-L150-M1.rwd_37805-PZA-L150-M1.rwd.xdf` | `.XDF` | `1,582` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZD-4160_37805-PZD-4160.xdf` | `.XDF` | `10,063` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZD-A130-M1.rwd_37805-PZD-A130-M1.rwd.xdf` | `.XDF` | `10,077` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-PZD-A380_37805-PZD-A380.xdf` | `.XDF` | `10,055` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-A190_37805-R40-A190.xdf` | `.XDF` | `5,007` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-K130_37805-R40-K130.xdf` | `.XDF` | `5,007` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-K530_37805-R40-K530.xdf` | `.XDF` | `5,007` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-K630_37805-R40-K630.xdf` | `.XDF` | `5,007` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R40-U530_37805-R40-U530.xdf` | `.XDF` | `5,007` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R49-U030_37805-R49-U030.xdf` | `.XDF` | `5,007` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R60-M720_37805-R60-M720.xdf` | `.XDF` | `3,887` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R60-U550_37805-R60-U550.xdf` | `.XDF` | `3,887` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-R8A-A560_37805-R8A-A560.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RBJ-A560_37805-RBJ-A560.xdf` | `.XDF` | `7,212` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RBJ-T520_37805-RBJ-T520.xdf` | `.XDF` | `7,212` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC0-M030_37805-RC0-M030.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC0-M130_37805-RC0-M130.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC0-M530_37805-RC0-M530.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC0-M630_37805-RC0-M630.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC1-M030_37805-RC1-M030.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC1-M540_37805-RC1-M540.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC1-P120_37805-RC1-P120.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC1-P520_37805-RC1-P520.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RC1-P720_37805-RC1-P720.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-3150.rwd_37805-RCA-3150.rwd.xdf` | `.XDF` | `4,452` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-3160.rwd_37805-RCA-3160.rwd.xdf` | `.XDF` | `4,452` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-A060-M5.rwd_37805-RCA-A060-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-A360-M5.rwd_37805-RCA-A360-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-A850-M5.rwd_37805-RCA-A850-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-A980-M5.rwd_37805-RCA-A980-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-K570-M5.rwd_37805-RCA-K570-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-K740-M5.rwd_37805-RCA-K740-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-K940-M5.rwd_37805-RCA-K940-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-L060-M5.rwd_37805-RCA-L060-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-L250-M5.rwd_37805-RCA-L250-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-L360-M5.rwd_37805-RCA-L360-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-L850-M5.rwd_37805-RCA-L850-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-L980-M5.rwd_37805-RCA-L980-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-M740-M5.rwd_37805-RCA-M740-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-M940-M5.rwd_37805-RCA-M940-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X050-M5.rwd_37805-RCA-X050-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X130-M5.rwd_37805-RCA-X130-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X330-M5.rwd_37805-RCA-X330-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X440-M5.rwd_37805-RCA-X440-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X570-M5.rwd_37805-RCA-X570-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X670-M5.rwd_37805-RCA-X670-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X740-M5.rwd_37805-RCA-X740-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X840-M5.rwd_37805-RCA-X840-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCA-X950-M5.rwd_37805-RCA-X950-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCB-U810-M5.rwd_37805-RCB-U810-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCB-Y740-M5.rwd_37805-RCB-Y740-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCE-U820-M5.rwd_37805-RCE-U820-M5.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCJ-3350.rwd_37805-RCJ-3350.rwd.xdf` | `.XDF` | `4,452` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCJ-3360.rwd_37805-RCJ-3360.rwd.xdf` | `.XDF` | `4,452` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RCJ-A690-M1.rwd_37805-RCJ-A690-M1.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RDA-A070-M1.rwd_37805-RDA-A070-M1.rwd.xdf` | `.XDF` | `4,458` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RDA-X630-M1.rwd_37805-RDA-X630-M1.rwd.xdf` | `.XDF` | `9,511` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RDA-X750_37805-RDA-X750.xdf` | `.XDF` | `9,497` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RDB-A630_37805-RDB-A630.xdf` | `.XDF` | `9,497` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RGL-K920_37805-RGL-K920.xdf` | `.XDF` | `8,332` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RGL-X560-M1.rwd_37805-RGL-X560-M1.rwd.xdf` | `.XDF` | `8,346` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RGL-X730-M1.rwd_37805-RGL-X730-M1.rwd.xdf` | `.XDF` | `8,346` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RGL-X830_37805-RGL-X830.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RGL-X920_37805-RGL-X920.xdf` | `.XDF` | `8,332` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RGL-Y560-M1.rwd_37805-RGL-Y560-M1.rwd.xdf` | `.XDF` | `8,346` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RGL-Y820_37805-RGL-Y820.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RGM-A650-M1.rwd_37805-RGM-A650-M1.rwd.xdf` | `.XDF` | `7,784` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RJE-3250.rwd_37805-RJE-3250.rwd.xdf` | `.XDF` | `7,778` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RJE-A650-M1.rwd_37805-RJE-A650-M1.rwd.xdf` | `.XDF` | `7,784` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RJE-K020_37805-RJE-K020.xdf` | `.XDF` | `8,332` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RJE-X640_37805-RJE-X640.xdf` | `.XDF` | `8,332` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RJE-X730_37805-RJE-X730.xdf` | `.XDF` | `7,776` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RK8-N520_37805-RK8-N520.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RK8-N740_37805-RK8-N740.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RK8-N840_37805-RK8-N840.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RKG-X550_37805-RKG-X550.xdf` | `.XDF` | `9,497` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RKG-X720_37805-RKG-X720.xdf` | `.XDF` | `7,776` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RKG-Y520_37805-RKG-Y520.xdf` | `.XDF` | `9,497` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-C410_37805-RME-C410.xdf` | `.XDF` | `3,314` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-C520_37805-RME-C520.xdf` | `.XDF` | `3,314` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-C720_37805-RME-C720.xdf` | `.XDF` | `3,314` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RME-C890_37805-RME-C890.xdf` | `.XDF` | `3,314` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RMX-3250_37805-RMX-3250.xdf` | `.XDF` | `2,725` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RMX-5070_37805-RMX-5070.xdf` | `.XDF` | `2,725` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RMX-5150_37805-RMX-5150.xdf` | `.XDF` | `2,725` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RMX-A060_Honda_Civic_1.3_16v_SH7058_1Mb.xdf` | `.XDF` | `2,741` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RMX-A130_37805-RMX-A130.xdf` | `.XDF` | `2,725` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RMX-X550_37805-RMX-X550.xdf` | `.XDF` | `2,725` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-3150_37805-RN0-3150.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-3160_37805-RN0-3160.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-A070_37805-RN0-A070.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-A570_37805-RN0-A570.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-C050_37805-RN0-C050.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-C950_37805-RN0-C950.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-K030_37805-RN0-K030.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-K130_37805-RN0-K130.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-M040_37805-RN0-M040.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-M130_37805-RN0-M130.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-M830_37805-RN0-M830.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-M940_37805-RN0-M940.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-X030_37805-RN0-X030.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-X560_37805-RN0-X560.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-X620_37805-RN0-X620.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-X760_37805-RN0-X760.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-X820_37805-RN0-X820.xdf` | `.XDF` | `7,770` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RN0-X940_37805-RN0-X940.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-3260_37805-RNA-3260.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-3290_37805-RNA-3290.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-3450_37805-RNA-3450.xdf` | `.XDF` | `4,440` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-3470_Honda_Civic_2006_DX__EX__LX_1.8L__L4_-_Gas.xdf` | `.XDF` | `4,470` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A150_Honda_Civic_1.8_16v_SH7058_1Mb.xdf` | `.XDF` | `3,899` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A240_37805-RNA-A240.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A330_Honda_Civic_2009_2010_EX-L_1.8L_L4_-_Gas.xdf` | `.XDF` | `84,467` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A340_37805-RNA-A340.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A680_37805-RNA-A680.xdf` | `.XDF` | `4,440` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A740_Honda_Civic_2007_2008_DX__EX__LX_1.8L__L4_-_Gas___ECU_Honda_.xdf` | `.XDF` | `4,599` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A830_37805-RNA-A830.xdf` | `.XDF` | `79,204` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A830_Honda_Civic_2009_2010_2011_EX-L_1.8L_L4_-_Gas.xdf` | `.XDF` | `79,235` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-A840_Honda_Civic_2009_2010_2011_DX__EX__LX__LX-S_1.8L__L4_-_Gas.xdf` | `.XDF` | `4,488` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-C130_Honda_Civic_2009_2010_2011_EX-L_1.8L__L4_-_Gas.xdf` | `.XDF` | `3,917` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-C240_37805-RNA-C240.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-C340_37805-RNA-C340.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-C440_37805-RNA-C440.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-C640_37805-RNA-C640.xdf` | `.XDF` | `4,440` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-C740_37805-RNA-C740.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-C840_37805-RNA-C840.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-C910_37805-RNA-C910.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-K080_37805-RNA-K080.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-K590_37805-RNA-K590.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-U720_37805-RNA-U720.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-U840_37805-RNA-U840.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-U950_37805-RNA-U950.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-Y030_37805-RNA-Y030.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-Y330_37805-RNA-Y330.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-Y530_37805-RNA-Y530.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-Y720_37805-RNA-Y720.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNA-Y830_37805-RNA-Y830.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNB-X040_37805-RNB-X040.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNB-X120_37805-RNB-X120.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNB-X560_37805-RNB-X560.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNB-X620_37805-RNB-X620.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RND-M030_37805-RND-M030.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RND-M530_37805-RND-M530.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RND-M620_37805-RND-M620.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RND-M720_37805-RND-M720.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RND-P030_37805-RND-P030.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RND-P540_37805-RND-P540.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RND-P740_37805-RND-P740.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNE-A550_37805-RNE-A550.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNF-U050_Honda_Civic_2006_2007_2008_2009_2010_2011_GX_1.8L__L4_-_CNG.xdf` | `.XDF` | `4,493` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNF-U540_37805-RNF-U540.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNF-U730_37805-RNF-U730.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNT-U030_37805-RNT-U030.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNT-U520_37805-RNT-U520.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-B030_37805-RNV-B030.xdf` | `.XDF` | `5,006` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-B530_37805-RNV-B530.xdf` | `.XDF` | `4,445` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-B630_37805-RNV-B630.xdf` | `.XDF` | `4,445` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-B730_37805-RNV-B730.xdf` | `.XDF` | `4,445` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-M070_37805-RNV-M070.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-M560_37805-RNV-M560.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-M660_37805-RNV-M660.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-R020_37805-RNV-R020.xdf` | `.XDF` | `5,006` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-R520_37805-RNV-R520.xdf` | `.XDF` | `5,002` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-R620_37805-RNV-R620.xdf` | `.XDF` | `5,002` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-R720_37805-RNV-R720.xdf` | `.XDF` | `5,002` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-Z020_37805-RNV-Z020.xdf` | `.XDF` | `5,006` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-Z520_37805-RNV-Z520.xdf` | `.XDF` | `5,002` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-Z620_37805-RNV-Z620.xdf` | `.XDF` | `5,002` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNV-Z720_37805-RNV-Z720.xdf` | `.XDF` | `5,002` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNX-M020_37805-RNX-M020.xdf` | `.XDF` | `4,446` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNX-M520_37805-RNX-M520.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RNX-M620_37805-RNX-M620.xdf` | `.XDF` | `4,442` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RP3-3050_37805-RP3-3050.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RP3-3070_37805-RP3-3070.xdf` | `.XDF` | `4,444` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RP6-X640_37805-RP6-X640.xdf` | `.XDF` | `7,776` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RPY-G040_37805-RPY-G040.xdf` | `.XDF` | `99,004` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRA-C040_37805-RRA-C040.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRA-C540_37805-RRA-C540.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRB-3150_37805-RRB-3150.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRB-A090_37805-RRB-A090.xdf` | `.XDF` | `8,891` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRB-K020_Honda_Civic_2007_2008_2009_2010_2011_Si_2.0L__L4_-_Gas.xdf` | `.XDF` | `8,933` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRB-X120_37805-RRB-X120.xdf` | `.XDF` | `8,891` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRD-M120_37805-RRD-M120.xdf` | `.XDF` | `8,891` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRD-M220_Honda_Civic_2.0_16v_SH7058_1Mb.xdf` | `.XDF` | `8,907` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRD-P120_37805-RRD-P120.xdf` | `.XDF` | `8,891` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRH-U020_37805-RRH-U020.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRH-U520_37805-RRH-U520.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RRH-U620_Honda_Civic_2.0_16v_SH7058_1Mb.xdf` | `.XDF` | `3,858` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RSP-E020_37805-RSP-E020.xdf` | `.XDF` | `164,224` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RTW-3050_37805-RTW-3050.xdf` | `.XDF` | `3,884` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RV0-3290_37805-RV0-3290.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RV0-A580_37805-RV0-A580.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RV0-X640_37805-RV0-X640.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RV0-X780_37805-RV0-X780.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RV0-Y640_37805-RV0-Y640.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RV0-Y780_37805-RV0-Y780.xdf` | `.XDF` | `7,214` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RWC-X560_37805-RWC-X560.xdf` | `.XDF` | `5,004` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RWC-X620_37805-RWC-X620.xdf` | `.XDF` | `10,055` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RX0-A030_Honda_Civic_2012_Si_2.4L_L4_-_Gas.xdf` | `.XDF` | `117,880` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RX0-A140_Honda_Civic_2012_Si_2.4L__L4_-_Gas.xdf` | `.XDF` | `109,265` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RX0-A220_Honda_Civic_2013_Si_2.4L__L4_-_Gas.xdf` | `.XDF` | `109,788` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RYE-A040_37805-RYE-A040.xdf` | `.XDF` | `7,776` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RYE-A140_37805-RYE-A140.xdf` | `.XDF` | `7,776` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RYE-X620_37805-RYE-X620.xdf` | `.XDF` | `8,332` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RYE-X750_37805-RYE-X750.xdf` | `.XDF` | `7,776` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RYE-X830_37805-RYE-X830.xdf` | `.XDF` | `7,776` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RYP-A570-M1.rwd_37805-RYP-A570-M1.rwd.xdf` | `.XDF` | `7,790` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RYP-A620-M1.rwd_37805-RYP-A620-M1.rwd.xdf` | `.XDF` | `7,790` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-K130_37805-RZA-K130.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-K230_37805-RZA-K230.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-K320_37805-RZA-K320.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-K520_37805-RZA-K520.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-K620_37805-RZA-K620.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-K720_37805-RZA-K720.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-K930_37805-RZA-K930.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-X630_37805-RZA-X630.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZA-X830_37805-RZA-X830.xdf` | `.XDF` | `3,842` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZP-M020_37805-RZP-M020.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZP-M520_37805-RZP-M520.xdf` | `.XDF` | `3,883` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZP-M720_37805-RZP-M720.xdf` | `.XDF` | `4,440` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `37805-RZP-M820_37805-RZP-M820.xdf` | `.XDF` | `4,440` bytes | TunerPro Binary Definition Map / Parameter Layout |
| `HONDA_CIVIC_FB_2012-2015_1.8L_R18Z1_KEIHIN_37805-R1J-A660-M1.rwd` | `.RWD` | `2,031,794` bytes | OEM Firmware Calibration Flash Dump / Binary Package |

### Subdirektori Tambahan

- **`OFFICIAL_CALIBRATION_PACKAGES/`**: Mengelola 482 aset kalibrasi lanjutan.

---

## 3. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup sebelum melakukan flashing kalibrasi.
3. **Tegangan Catu Daya**: Pastikan kestabilan tegangan catu daya 13.5V – 14.2V selama proses penulisan firmware.
