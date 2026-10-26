# OFFICIAL CALIBRATION PACKAGES - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/CIVIC_1_8L_2_0L_R18_K20/OFFICIAL_CALIBRATION_PACKAGES`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `298 files` (298 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `OFFICIAL_CALIBRATION_PACKAGES` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`): Nomor resmi Toyota Techstream / Denso MCU firmware flash.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **GM OS IDs** (misal `12587603`, `12212156`): Operating system ID kontroler GM Delphi P01/P59.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `37805-5AF-B420-M1.rwd` | `.RWD` | `2,555,962` bytes | Honda Keihin Factory Calibration Package `37805-5AF-B420` |
| `37805-5AN-CC10-M1.rwd` | `.RWD` | `2,555,962` bytes | Honda Keihin Factory Calibration Package `37805-5AN-CC10` |
| `37805-5YF-AD20-M1.rwd` | `.RWD` | `2,555,962` bytes | Honda Keihin Factory Calibration Package `37805-5YF-AD20` |
| `37805-64A-A540-M1.rwd` | `.RWD` | `2,555,962` bytes | Honda Keihin Factory Calibration Package `37805-64A-A540` |
| `37805-64B-A010-M1.rwd` | `.RWD` | `2,555,962` bytes | Honda Keihin Factory Calibration Package `37805-64B-A010` |
| `37805-64L-J020-M1.rwd` | `.RWD` | `2,555,962` bytes | Honda Keihin Factory Calibration Package `37805-64L-J020` |
| `37805-64L-J530-M1.rwd` | `.RWD` | `2,555,962` bytes | Honda Keihin Factory Calibration Package `37805-64L-J530` |
| `37805-PCX-U120-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-PCX-U120` |
| `37805-PHM-4050.rwd` | `.RWD` | `109,541` bytes | Honda Keihin Factory Calibration Package `37805-PHM-4050` |
| `37805-PLM-3170.rwd` | `.RWD` | `85,627` bytes | Honda Keihin Factory Calibration Package `37805-PLM-3170` |
| `37805-PLM-3360.rwd` | `.RWD` | `121,337` bytes | Honda Keihin Factory Calibration Package `37805-PLM-3360` |
| `37805-PLM-3390.rwd` | `.RWD` | `121,315` bytes | Honda Keihin Factory Calibration Package `37805-PLM-3390` |
| `37805-PLM-4050.rwd` | `.RWD` | `85,869` bytes | Honda Keihin Factory Calibration Package `37805-PLM-4050` |
| `37805-PLM-4170.rwd` | `.RWD` | `85,891` bytes | Honda Keihin Factory Calibration Package `37805-PLM-4170` |
| `37805-PLM-4260.rwd` | `.RWD` | `121,579` bytes | Honda Keihin Factory Calibration Package `37805-PLM-4260` |
| `37805-PLM-4390.rwd` | `.RWD` | `121,579` bytes | Honda Keihin Factory Calibration Package `37805-PLM-4390` |
| `37805-PLM-A150-M1.rwd` | `.RWD` | `117,857` bytes | Honda Keihin Factory Calibration Package `37805-PLM-A150` |
| `37805-PLM-A760-M1.rwd` | `.RWD` | `155,701` bytes | Honda Keihin Factory Calibration Package `37805-PLM-A760` |
| `37805-PLM-C150-M1.rwd` | `.RWD` | `117,857` bytes | Honda Keihin Factory Calibration Package `37805-PLM-C150` |
| `37805-PLM-C760-M1.rwd` | `.RWD` | `155,701` bytes | Honda Keihin Factory Calibration Package `37805-PLM-C760` |
| `37805-PLR-3150.rwd` | `.RWD` | `88,091` bytes | Honda Keihin Factory Calibration Package `37805-PLR-3150` |
| `37805-PLR-3170.rwd` | `.RWD` | `88,069` bytes | Honda Keihin Factory Calibration Package `37805-PLR-3170` |
| `37805-PLR-3360.rwd` | `.RWD` | `123,779` bytes | Honda Keihin Factory Calibration Package `37805-PLR-3360` |
| `37805-PLR-3390.rwd` | `.RWD` | `123,757` bytes | Honda Keihin Factory Calibration Package `37805-PLR-3390` |
| `37805-PLR-4050.rwd` | `.RWD` | `88,311` bytes | Honda Keihin Factory Calibration Package `37805-PLR-4050` |
| `37805-PLR-4170.rwd` | `.RWD` | `88,355` bytes | Honda Keihin Factory Calibration Package `37805-PLR-4170` |
| `37805-PLR-4260.rwd` | `.RWD` | `124,021` bytes | Honda Keihin Factory Calibration Package `37805-PLR-4260` |
| `37805-PLR-4390.rwd` | `.RWD` | `124,043` bytes | Honda Keihin Factory Calibration Package `37805-PLR-4390` |
| `37805-PLR-A130-M1.rwd` | `.RWD` | `119,133` bytes | Honda Keihin Factory Calibration Package `37805-PLR-A130` |
| `37805-PLR-A750-M1.rwd` | `.RWD` | `156,999` bytes | Honda Keihin Factory Calibration Package `37805-PLR-A750` |
| `37805-PLR-C130-M1.rwd` | `.RWD` | `119,133` bytes | Honda Keihin Factory Calibration Package `37805-PLR-C130` |
| `37805-PLR-C750-M1.rwd` | `.RWD` | `156,999` bytes | Honda Keihin Factory Calibration Package `37805-PLR-C750` |
| `37805-PMM-3170.rwd` | `.RWD` | `85,649` bytes | Honda Keihin Factory Calibration Package `37805-PMM-3170` |
| `37805-PMM-3390.rwd` | `.RWD` | `121,337` bytes | Honda Keihin Factory Calibration Package `37805-PMM-3390` |
| `37805-PMM-4050.rwd` | `.RWD` | `85,869` bytes | Honda Keihin Factory Calibration Package `37805-PMM-4050` |
| `37805-PMM-4170.rwd` | `.RWD` | `85,913` bytes | Honda Keihin Factory Calibration Package `37805-PMM-4170` |
| `37805-PMM-4260.rwd` | `.RWD` | `121,579` bytes | Honda Keihin Factory Calibration Package `37805-PMM-4260` |
| `37805-PMM-4390.rwd` | `.RWD` | `121,601` bytes | Honda Keihin Factory Calibration Package `37805-PMM-4390` |
| `37805-PMP-3050.rwd` | `.RWD` | `97,947` bytes | Honda Keihin Factory Calibration Package `37805-PMP-3050` |
| `37805-PMP-3060.rwd` | `.RWD` | `131,017` bytes | Honda Keihin Factory Calibration Package `37805-PMP-3060` |
| `37805-PMP-3070.rwd` | `.RWD` | `97,947` bytes | Honda Keihin Factory Calibration Package `37805-PMP-3070` |
| `37805-PMP-3090.rwd` | `.RWD` | `131,017` bytes | Honda Keihin Factory Calibration Package `37805-PMP-3090` |
| `37805-PMP-4050.rwd` | `.RWD` | `99,201` bytes | Honda Keihin Factory Calibration Package `37805-PMP-4050` |
| `37805-PMP-4060.rwd` | `.RWD` | `141,445` bytes | Honda Keihin Factory Calibration Package `37805-PMP-4060` |
| `37805-PMP-4170.rwd` | `.RWD` | `99,245` bytes | Honda Keihin Factory Calibration Package `37805-PMP-4170` |
| `37805-PMP-4190.rwd` | `.RWD` | `141,489` bytes | Honda Keihin Factory Calibration Package `37805-PMP-4190` |
| `37805-PMP-A130-M1.rwd` | `.RWD` | `119,133` bytes | Honda Keihin Factory Calibration Package `37805-PMP-A130` |
| `37805-PMP-A830-M1.rwd` | `.RWD` | `176,953` bytes | Honda Keihin Factory Calibration Package `37805-PMP-A830` |
| `37805-PMR-3170.rwd` | `.RWD` | `88,091` bytes | Honda Keihin Factory Calibration Package `37805-PMR-3170` |
| `37805-PMR-3390.rwd` | `.RWD` | `123,779` bytes | Honda Keihin Factory Calibration Package `37805-PMR-3390` |
| `37805-PMR-4050.rwd` | `.RWD` | `88,311` bytes | Honda Keihin Factory Calibration Package `37805-PMR-4050` |
| `37805-PMR-4170.rwd` | `.RWD` | `88,355` bytes | Honda Keihin Factory Calibration Package `37805-PMR-4170` |
| `37805-PMR-4260.rwd` | `.RWD` | `124,021` bytes | Honda Keihin Factory Calibration Package `37805-PMR-4260` |
| `37805-PMR-4390.rwd` | `.RWD` | `124,043` bytes | Honda Keihin Factory Calibration Package `37805-PMR-4390` |
| `37805-PMS-A660-M1.rwd` | `.RWD` | `120,243` bytes | Honda Keihin Factory Calibration Package `37805-PMS-A660` |
| `37805-PMS-A680-M1.rwd` | `.RWD` | `127,299` bytes | Honda Keihin Factory Calibration Package `37805-PMS-A680` |
| `37805-PND-3050.rwd` | `.RWD` | `123,335` bytes | Honda Keihin Factory Calibration Package `37805-PND-3050` |
| `37805-PND-3060.rwd` | `.RWD` | `194,091` bytes | Honda Keihin Factory Calibration Package `37805-PND-3060` |
| `37805-PND-3070.rwd` | `.RWD` | `540,209` bytes | Honda Keihin Factory Calibration Package `37805-PND-3070` |
| `37805-PNF-A060-M1.rwd` | `.RWD` | `118,787` bytes | Honda Keihin Factory Calibration Package `37805-PNF-A060` |
| `37805-PPA-3050.rwd` | `.RWD` | `123,313` bytes | Honda Keihin Factory Calibration Package `37805-PPA-3050` |
| `37805-PPA-3180.rwd` | `.RWD` | `590,419` bytes | Honda Keihin Factory Calibration Package `37805-PPA-3180` |
| `37805-PPA-4260.rwd` | `.RWD` | `588,729` bytes | Honda Keihin Factory Calibration Package `37805-PPA-4260` |
| `37805-PRB-3050.rwd` | `.RWD` | `123,313` bytes | Honda Keihin Factory Calibration Package `37805-PRB-3050` |
| `37805-PRB-A080-M1.rwd` | `.RWD` | `123,203` bytes | Honda Keihin Factory Calibration Package `37805-PRB-A080` |
| `37805-PVJ-X560-M1.rwd` | `.RWD` | `655,619` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-X560` |
| `37805-PVJ-X810-M1.rwd` | `.RWD` | `637,189` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-X810` |
| `37805-PVJ-X910-M1.rwd` | `.RWD` | `655,259` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-X910` |
| `37805-PVJ-Y530-M1.rwd` | `.RWD` | `637,159` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-Y530` |
| `37805-PVJ-Y550-M1.rwd` | `.RWD` | `655,199` bytes | Honda Keihin Factory Calibration Package `37805-PVJ-Y550` |
| `37805-PWG-3050.rwd` | `.RWD` | `156,744` bytes | Honda Keihin Factory Calibration Package `37805-PWG-3050` |
| `37805-PWG-3060.rwd` | `.RWD` | `156,744` bytes | Honda Keihin Factory Calibration Package `37805-PWG-3060` |
| `37805-PZA-3050.rwd` | `.RWD` | `356,519` bytes | Honda Keihin Factory Calibration Package `37805-PZA-3050` |
| `37805-PZA-3280.rwd` | `.RWD` | `319,749` bytes | Honda Keihin Factory Calibration Package `37805-PZA-3280` |
| `37805-PZA-3290.rwd` | `.RWD` | `319,749` bytes | Honda Keihin Factory Calibration Package `37805-PZA-3290` |
| `37805-PZA-4060.rwd` | `.RWD` | `366,599` bytes | Honda Keihin Factory Calibration Package `37805-PZA-4060` |
| `37805-PZA-4280.rwd` | `.RWD` | `367,049` bytes | Honda Keihin Factory Calibration Package `37805-PZA-4280` |
| `37805-PZA-A170-M1.rwd` | `.RWD` | `380,629` bytes | Honda Keihin Factory Calibration Package `37805-PZA-A170` |
| `37805-PZA-L150-M1.rwd` | `.RWD` | `377,969` bytes | Honda Keihin Factory Calibration Package `37805-PZA-L150` |
| `37805-PZD-4160.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-PZD-4160` |
| `37805-PZD-A130-M1.rwd` | `.RWD` | `533,709` bytes | Honda Keihin Factory Calibration Package `37805-PZD-A130` |
| `37805-PZD-A380-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-PZD-A380` |
| `37805-R40-A190-M1.RWD` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-R40-A190` |
| `37805-R40-K130-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-R40-K130` |
| `37805-R40-K530-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-R40-K530` |
| `37805-R40-K630-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-R40-K630` |
| `37805-R40-U530-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-R40-U530` |
| `37805-R49-U030-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-R49-U030` |
| `37805-R60-M720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-R60-M720` |
| `37805-R60-U550-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-R60-U550` |
| `37805-R8A-A560-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-R8A-A560` |
| `37805-RBJ-A560-M1.RWD` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RBJ-A560` |
| `37805-RBJ-T520-M1.RWD` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RBJ-T520` |
| `37805-RC0-M030-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RC0-M030` |
| `37805-RC0-M130-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RC0-M130` |
| `37805-RC0-M530-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RC0-M530` |
| `37805-RC0-M630-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RC0-M630` |
| `37805-RC1-M030-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RC1-M030` |
| `37805-RC1-M540-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RC1-M540` |
| `37805-RC1-P120-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RC1-P120` |
| `37805-RC1-P520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RC1-P520` |
| `37805-RC1-P720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RC1-P720` |
| `37805-RCA-3150.rwd` | `.RWD` | `529,049` bytes | Honda Keihin Factory Calibration Package `37805-RCA-3150` |
| `37805-RCA-3160.rwd` | `.RWD` | `529,049` bytes | Honda Keihin Factory Calibration Package `37805-RCA-3160` |
| `37805-RCA-A060-M5.rwd` | `.RWD` | `531,009` bytes | Honda Keihin Factory Calibration Package `37805-RCA-A060` |
| `37805-RCA-A360-M5.rwd` | `.RWD` | `618,009` bytes | Honda Keihin Factory Calibration Package `37805-RCA-A360` |
| `37805-RCA-A850-M5.rwd` | `.RWD` | `617,979` bytes | Honda Keihin Factory Calibration Package `37805-RCA-A850` |
| `37805-RCA-A980-M5.rwd` | `.RWD` | `600,979` bytes | Honda Keihin Factory Calibration Package `37805-RCA-A980` |
| `37805-RCA-K570-M5.rwd` | `.RWD` | `528,952` bytes | Honda Keihin Factory Calibration Package `37805-RCA-K570` |
| `37805-RCA-K740-M5.rwd` | `.RWD` | `528,472` bytes | Honda Keihin Factory Calibration Package `37805-RCA-K740` |
| `37805-RCA-K940-M5.rwd` | `.RWD` | `599,482` bytes | Honda Keihin Factory Calibration Package `37805-RCA-K940` |
| `37805-RCA-L060-M5.rwd` | `.RWD` | `531,009` bytes | Honda Keihin Factory Calibration Package `37805-RCA-L060` |
| `37805-RCA-L250-M5.rwd` | `.RWD` | `530,589` bytes | Honda Keihin Factory Calibration Package `37805-RCA-L250` |
| `37805-RCA-L360-M5.rwd` | `.RWD` | `618,009` bytes | Honda Keihin Factory Calibration Package `37805-RCA-L360` |
| `37805-RCA-L850-M5.rwd` | `.RWD` | `617,979` bytes | Honda Keihin Factory Calibration Package `37805-RCA-L850` |
| `37805-RCA-L980-M5.rwd` | `.RWD` | `600,979` bytes | Honda Keihin Factory Calibration Package `37805-RCA-L980` |
| `37805-RCA-M740-M5.rwd` | `.RWD` | `528,472` bytes | Honda Keihin Factory Calibration Package `37805-RCA-M740` |
| `37805-RCA-M940-M5.rwd` | `.RWD` | `599,482` bytes | Honda Keihin Factory Calibration Package `37805-RCA-M940` |
| `37805-RCA-X050-M5.rwd` | `.RWD` | `600,949` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X050` |
| `37805-RCA-X130-M5.rwd` | `.RWD` | `617,399` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X130` |
| `37805-RCA-X330-M5.rwd` | `.RWD` | `617,529` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X330` |
| `37805-RCA-X440-M5.rwd` | `.RWD` | `600,919` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X440` |
| `37805-RCA-X570-M5.rwd` | `.RWD` | `528,952` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X570` |
| `37805-RCA-X670-M5.rwd` | `.RWD` | `528,952` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X670` |
| `37805-RCA-X740-M5.rwd` | `.RWD` | `528,479` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X740` |
| `37805-RCA-X840-M5.rwd` | `.RWD` | `528,479` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X840` |
| `37805-RCA-X950-M5.rwd` | `.RWD` | `600,949` bytes | Honda Keihin Factory Calibration Package `37805-RCA-X950` |
| `37805-RCB-U810-M5.rwd` | `.RWD` | `524,939` bytes | Honda Keihin Factory Calibration Package `37805-RCB-U810` |
| `37805-RCB-Y740-M5.rwd` | `.RWD` | `599,452` bytes | Honda Keihin Factory Calibration Package `37805-RCB-Y740` |
| `37805-RCE-U820-M5.rwd` | `.RWD` | `617,369` bytes | Honda Keihin Factory Calibration Package `37805-RCE-U820` |
| `37805-RCJ-3350.rwd` | `.RWD` | `537,009` bytes | Honda Keihin Factory Calibration Package `37805-RCJ-3350` |
| `37805-RCJ-3360.rwd` | `.RWD` | `537,009` bytes | Honda Keihin Factory Calibration Package `37805-RCJ-3360` |
| `37805-RCJ-A690-M1.rwd` | `.RWD` | `560,249` bytes | Honda Keihin Factory Calibration Package `37805-RCJ-A690` |
| `37805-RDA-A070-M1.rwd` | `.RWD` | `364,409` bytes | Honda Keihin Factory Calibration Package `37805-RDA-A070` |
| `37805-RDA-X630-M1.rwd` | `.RWD` | `568,129` bytes | Honda Keihin Factory Calibration Package `37805-RDA-X630` |
| `37805-RDA-X750-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RDA-X750` |
| `37805-RDB-A630-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RDB-A630` |
| `37805-RGL-K920-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RGL-K920` |
| `37805-RGL-X560-M1.rwd` | `.RWD` | `637,379` bytes | Honda Keihin Factory Calibration Package `37805-RGL-X560` |
| `37805-RGL-X730-M1.rwd` | `.RWD` | `646,519` bytes | Honda Keihin Factory Calibration Package `37805-RGL-X730` |
| `37805-RGL-X830-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RGL-X830` |
| `37805-RGL-X920-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RGL-X920` |
| `37805-RGL-Y560-M1.rwd` | `.RWD` | `637,249` bytes | Honda Keihin Factory Calibration Package `37805-RGL-Y560` |
| `37805-RGL-Y820-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RGL-Y820` |
| `37805-RGM-A650-M1.rwd` | `.RWD` | `663,849` bytes | Honda Keihin Factory Calibration Package `37805-RGM-A650` |
| `37805-RJE-3250.rwd` | `.RWD` | `640,659` bytes | Honda Keihin Factory Calibration Package `37805-RJE-3250` |
| `37805-RJE-A650-M1.rwd` | `.RWD` | `648,659` bytes | Honda Keihin Factory Calibration Package `37805-RJE-A650` |
| `37805-RJE-K020-M1.0x8000_1.bin` | `.BIN` | `1,015,808` bytes | Honda Keihin Factory Calibration Package `37805-RJE-K020` |
| `37805-RJE-X640-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RJE-X640` |
| `37805-RJE-X730-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RJE-X730` |
| `37805-RK8-N520-M1.RWD` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RK8-N520` |
| `37805-RK8-N740-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RK8-N740` |
| `37805-RK8-N840-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RK8-N840` |
| `37805-RKG-X550-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RKG-X550` |
| `37805-RKG-X720-M1.RWD` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RKG-X720` |
| `37805-RKG-Y520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RKG-Y520` |
| `37805-RME-C410-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RME-C410` |
| `37805-RME-C520-M1.rwd` | `.RWD` | `1,016,058` bytes | Honda Keihin Factory Calibration Package `37805-RME-C520` |
| `37805-RME-C720-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RME-C720` |
| `37805-RME-C890-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RME-C890` |
| `37805-RMX-3250.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RMX-3250` |
| `37805-RMX-5070.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RMX-5070` |
| `37805-RMX-5150.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RMX-5150` |
| `37805-RMX-A060-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RMX-A060` |
| `37805-RMX-A130-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RMX-A130` |
| `37805-RMX-X550-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RMX-X550` |
| `37805-RN0-3150-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RN0-3150` |
| `37805-RN0-3160-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RN0-3160` |
| `37805-RN0-A070-M1.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RN0-A070` |
| `37805-RN0-A570-M1.RWD` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RN0-A570` |
| `37805-RN0-C050-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RN0-C050` |
| `37805-RN0-C950-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RN0-C950` |
| `37805-RN0-K030-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RN0-K030` |
| `37805-RN0-K130-M1.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RN0-K130` |
| `37805-RN0-M040-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RN0-M040` |
| `37805-RN0-M130-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RN0-M130` |
| `37805-RN0-M830-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RN0-M830` |
| `37805-RN0-M940-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RN0-M940` |
| `37805-RN0-X030-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RN0-X030` |
| `37805-RN0-X560-M1.RWD` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RN0-X560` |
| `37805-RN0-X620-M1.RWD` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RN0-X620` |
| `37805-RN0-X760-M1.RWD` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RN0-X760` |
| `37805-RN0-X820-M1.RWD` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RN0-X820` |
| `37805-RN0-X940-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RN0-X940` |
| `37805-RNA-3260.rwd` | `.RWD` | `1,016,058` bytes | Honda Keihin Factory Calibration Package `37805-RNA-3260` |
| `37805-RNA-3290.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RNA-3290` |
| `37805-RNA-3450.rwd` | `.RWD` | `1,016,130` bytes | Honda Keihin Factory Calibration Package `37805-RNA-3450` |
| `37805-RNA-3470.rwd` | `.RWD` | `1,016,106` bytes | Honda Keihin Factory Calibration Package `37805-RNA-3470` |
| `37805-RNA-A150-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RNA-A150` |
| `37805-RNA-A240-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-A240` |
| `37805-RNA-A330-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNA-A330` |
| `37805-RNA-A340-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-A340` |
| `37805-RNA-A680-M1.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RNA-A680` |
| `37805-RNA-A740-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-A740` |
| `37805-RNA-A830-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNA-A830` |
| `37805-RNA-A840-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-A840` |
| `37805-RNA-C130-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNA-C130` |
| `37805-RNA-C240-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-C240` |
| `37805-RNA-C340-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-C340` |
| `37805-RNA-C440-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-C440` |
| `37805-RNA-C640-M1.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RNA-C640` |
| `37805-RNA-C740-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-C740` |
| `37805-RNA-C840-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-C840` |
| `37805-RNA-C910-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RNA-C910` |
| `37805-RNA-K080-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RNA-K080` |
| `37805-RNA-K590-M1.rwd` | `.RWD` | `1,016,058` bytes | Honda Keihin Factory Calibration Package `37805-RNA-K590` |
| `37805-RNA-U720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNA-U720` |
| `37805-RNA-U840-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNA-U840` |
| `37805-RNA-U950-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RNA-U950` |
| `37805-RNA-Y030-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNA-Y030` |
| `37805-RNA-Y330-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNA-Y330` |
| `37805-RNA-Y530-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNA-Y530` |
| `37805-RNA-Y720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNA-Y720` |
| `37805-RNA-Y830-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNA-Y830` |
| `37805-RNB-X040-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNB-X040` |
| `37805-RNB-X120-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNB-X120` |
| `37805-RNB-X560-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RNB-X560` |
| `37805-RNB-X620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNB-X620` |
| `37805-RND-M030-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RND-M030` |
| `37805-RND-M530-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RND-M530` |
| `37805-RND-M620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RND-M620` |
| `37805-RND-M720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RND-M720` |
| `37805-RND-P030-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RND-P030` |
| `37805-RND-P540-M1.0x8000.bin` | `.BIN` | `1,015,808` bytes | Honda Keihin Factory Calibration Package `37805-RND-P540` |
| `37805-RND-P740-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RND-P740` |
| `37805-RNE-A550-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RNE-A550` |
| `37805-RNF-U050-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RNF-U050` |
| `37805-RNF-U540-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RNF-U540` |
| `37805-RNF-U730-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNF-U730` |
| `37805-RNT-U030-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNT-U030` |
| `37805-RNT-U520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNT-U520` |
| `37805-RNV-B030-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNV-B030` |
| `37805-RNV-B530-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNV-B530` |
| `37805-RNV-B630-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNV-B630` |
| `37805-RNV-B730-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RNV-B730` |
| `37805-RNV-M070-M1.rwd` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RNV-M070` |
| `37805-RNV-M560-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RNV-M560` |
| `37805-RNV-M660-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RNV-M660` |
| `37805-RNV-R020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNV-R020` |
| `37805-RNV-R520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNV-R520` |
| `37805-RNV-R620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNV-R620` |
| `37805-RNV-R720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNV-R720` |
| `37805-RNV-Z020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNV-Z020` |
| `37805-RNV-Z520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNV-Z520` |
| `37805-RNV-Z620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNV-Z620` |
| `37805-RNV-Z720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNV-Z720` |
| `37805-RNX-M020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNX-M020` |
| `37805-RNX-M520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNX-M520` |
| `37805-RNX-M620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RNX-M620` |
| `37805-RP3-3050.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RP3-3050` |
| `37805-RP3-3070.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RP3-3070` |
| `37805-RP6-X640-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RP6-X640` |
| `37805-RPY-G040-M6.rwd` | `.RWD` | `2,752,645` bytes | Honda Keihin Factory Calibration Package `37805-RPY-G040` |
| `37805-RRA-C040-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RRA-C040` |
| `37805-RRA-C540-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RRA-C540` |
| `37805-RRB-3150.rwd` | `.RWD` | `1,016,010` bytes | Honda Keihin Factory Calibration Package `37805-RRB-3150` |
| `37805-RRB-A090-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RRB-A090` |
| `37805-RRB-K020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RRB-K020` |
| `37805-RRB-X120-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RRB-X120` |
| `37805-RRD-M120-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RRD-M120` |
| `37805-RRD-M220-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RRD-M220` |
| `37805-RRD-P120-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RRD-P120` |
| `37805-RRH-U020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RRH-U020` |
| `37805-RRH-U520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RRH-U520` |
| `37805-RRH-U620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RRH-U620` |
| `37805-RSP-E020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RSP-E020` |
| `37805-RTW-3050-M1.RWD` | `.RWD` | `1,015,986` bytes | Honda Keihin Factory Calibration Package `37805-RTW-3050` |
| `37805-RV0-3290-M1.rwd` | `.RWD` | `1,016,106` bytes | Honda Keihin Factory Calibration Package `37805-RV0-3290` |
| `37805-RV0-A580-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RV0-A580` |
| `37805-RV0-X640-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RV0-X640` |
| `37805-RV0-X780-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RV0-X780` |
| `37805-RV0-Y640-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RV0-Y640` |
| `37805-RV0-Y780-M1.rwd` | `.RWD` | `1,016,034` bytes | Honda Keihin Factory Calibration Package `37805-RV0-Y780` |
| `37805-RWC-X560-M1.rwd` | `.RWD` | `1,015,962` bytes | Honda Keihin Factory Calibration Package `37805-RWC-X560` |
| `37805-RWC-X620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RWC-X620` |
| `37805-RX0-A030-M1.RWD` | `.RWD` | `2,031,722` bytes | Honda Keihin Factory Calibration Package `37805-RX0-A030` |
| `37805-RX0-A140-M1.RWD` | `.RWD` | `2,031,746` bytes | Honda Keihin Factory Calibration Package `37805-RX0-A140` |
| `37805-RX0-A220-M1.rwd` | `.RWD` | `2,031,698` bytes | Honda Keihin Factory Calibration Package `37805-RX0-A220` |
| `37805-RYE-A040-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A040` |
| `37805-RYE-A140-M1.rwd` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RYE-A140` |
| `37805-RYE-X620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RYE-X620` |
| `37805-RYE-X750-M1.RWD` | `.RWD` | `1,015,938` bytes | Honda Keihin Factory Calibration Package `37805-RYE-X750` |
| `37805-RYE-X830-M1.RWD` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RYE-X830` |
| `37805-RYP-A570-M1.rwd` | `.RWD` | `682,129` bytes | Honda Keihin Factory Calibration Package `37805-RYP-A570` |
| `37805-RYP-A620-M1.rwd` | `.RWD` | `682,369` bytes | Honda Keihin Factory Calibration Package `37805-RYP-A620` |
| `37805-RZA-K130-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZA-K130` |
| `37805-RZA-K230-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZA-K230` |
| `37805-RZA-K320-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZA-K320` |
| `37805-RZA-K520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZA-K520` |
| `37805-RZA-K620-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZA-K620` |
| `37805-RZA-K720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZA-K720` |
| `37805-RZA-K930-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZA-K930` |
| `37805-RZA-X630-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RZA-X630` |
| `37805-RZA-X830-M1.rwd` | `.RWD` | `1,015,914` bytes | Honda Keihin Factory Calibration Package `37805-RZA-X830` |
| `37805-RZP-M020-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZP-M020` |
| `37805-RZP-M520-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZP-M520` |
| `37805-RZP-M720-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZP-M720` |
| `37805-RZP-M820-M1.rwd` | `.RWD` | `1,015,890` bytes | Honda Keihin Factory Calibration Package `37805-RZP-M820` |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance, Low/High Octane Timing, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow & Boost Management**: Peta Target Boost Pressure, Wastegate Duty Cycle (WGDC), MAF/MAP Scaling, dan Throttle Response Curves.
- **Safety Limits & Thresholds**: Rev Limiter (Hard/Soft Cut), Top Speed Limiter (Vmax), Overboost Fuel Cut, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
