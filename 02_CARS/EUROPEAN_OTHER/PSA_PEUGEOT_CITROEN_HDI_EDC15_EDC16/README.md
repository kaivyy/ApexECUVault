# PSA PEUGEOT & CITROEN - HDi Bosch EDC15C2, EDC16C34 & Siemens SID Suite

**Repository Path**: `02_CARS/EUROPEAN_OTHER/PSA_PEUGEOT_CITROEN_HDI_EDC15_EDC16`  
**Classification**: `Universal ECU Firmware & Calibration Suite`  
**Total Managed Assets**: `190 files` (190 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Koleksi 190 berkas biner original dumps (.ori/.bin) untuk jajaran kendaraan PSA Group (Peugeot 206, 207, 306, 307, 308, 406, 407, 607, Boxer; Citroen C2, C3, C4, C5, Xsara, Berlingo) dengan mesin diesel common rail HDi 1.4 HDi, 1.6 HDi, 2.0 HDi, 2.2 HDi, dan 2.7 HDi V6. Mesin 1.6 HDi (DV6) dan 2.0 HDi (DW10) serta ECU Bosch EDC16C34 adalah unit lintas platform yang juga digunakan pada Ford Fiesta/Focus (1.6 TDCi), Volvo S40/V50 (1.6D/2.0D), Mazda 3 (1.6 MZ-CD), dan MINI Cooper D.

### Detail Arsitektur Kontroler & Komunikasi:
- **Keluarga ECU / Controller Family**: `Bosch EDC15C2, EDC16C34, Siemens SID801, SID803, Magneti Marelli IAW`
- **Arsitektur MCU & Memori**: `Infineon C167CR / Motorola MPC561 / MPC562 512KB-2MB Flash`
- **Protokol Diagnostik & Flashing**: `K-Line (ISO 9141 / PSA KWP2000) / CAN-Bus / BDM100`

### Mengapa Sebagian Berkas Memiliki Nama Berupa Angka / Kode?
Nama berkas yang tersimpan merefleksikan identitas perangkat keras (Hardware ID), versi perangkat lunak (Software ID), atau nomor kalibrasi pabrikan asli (OEM Calibration ID):
- **Bosch Part Numbers** (misal `0261xxxxxx`, `1037xxxxxx`): Standar identifikasi universal Bosch untuk ECU Motronic, MED17, EDC16, dan EDC17.
- **BMW Software IDs** (misal `00005C64xxxxxx`, `10SW002828`, `0110C6`, `MS430069`): Alamat dan assembly identification number pada modul DME Siemens/Continental/Bosch.
- **Denso / Toyota Calibration IDs** (misal `89663-xxxxx`, `32920-xxxxx`): Nomor resmi Denso MCU firmware flash untuk mobil dan motor.
- **Keihin Part Numbers** (misal `37805-xxx-xxxx`, `38770-xxx-xxxx`): Kode perakitan ECU Honda untuk verifikasi kecocokan checksum dan proteksi immobilizer.
- **VAG Hardware / Software IDs** (misal `038906012xx`, `03G906021xx`, `8D0907558xx`): Nomor bagian resmi Volkswagen Audi Group untuk identifikasi kalibrasi mesin EDC15, EDC16, dan ME7.

> [!NOTE]
> Mempertahankan kode dan nomor asli pabrikan pada penamaan berkas sangat krusial agar perangkat lunak kalibrasi (seperti **TunerPro**, **WinOLS**, atau **RomRaider**) dapat mengenali dan mencocokkan peta definisi (*definition maps*) secara otomatis tanpa merusak asosiasi header ECU.

---

## 2. Manifest Aset Berkas Fisik (100% Verified)

Berikut adalah daftar lengkap berkas fisik yang tersimpan secara lokal di direktori ini:

| Nama Berkas | Tipe / Format | Ukuran (Bytes) | Deskripsi Teknis & Identifikasi |
| :--- | :--- | :--- | :--- |
| `0281001782_1037359041_9634662880.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `0281011634_eep.bin` | `.BIN` | `8,192` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `0281011634_flash.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `213_492.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `306 HDI 0281010163 1037359088 B075WFS.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `306.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `5WS40110C-T HW9653447480 SW9648624280.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `5WS40136C-T 380 380.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `C5_2_9HZ_0281013872.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `CITROEN-ZX-2.0 16V-0261200218-1267357390.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `CITROEN-ZX-2.0 16V-0261200218-1267358295.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `CITROEN-ZX-2.0 16V-0261200218-2227355803.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `CITROEN_5W40378C-T_HW_9655534080_SW_9663862780_SiD803A.ori` | `.ORI` | `515,938` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen AX GTI 1.4 MP31  0261200217-1267357551.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Berlingo 1.6HDI 90HP 1037393468.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Berlingo 2.0HDI 90HP 5WS40108E-T 9651942080 9647423380.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C2 1.6 VTS 0261208376 369477.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C3 1.4HDI 68HP 0281012529 1037386117.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C3 1.4HDI 68HP 5WS40285C-T 9660300280 9653451880.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C3 1.6HDI 90HP 372289 DPF.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C4 1.6HDI 110HP 0281011629 376755.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C4 1.6HDI 8v 90HP 376754.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C4 2.0HDI 9655534080 5WS40277G-T 9660497480.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.0HDI 0281011524 369508.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.0HDI 110HP  0281010774 353726.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.0HDI 110HP 0281011340 368212.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.0HDI 136HP 5WS40199D-T 9655041480 9656171480.ori` | `.ORI` | `462,848` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.2 HDI 133BHP 0281010764 353785.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Citroen C5 2.2HDI 128HP 0281011033 364376.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.2HDI 133HP 0281010371 353456.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.2HDI 133HP 0281010641 1037353491.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.2HDI 133HP 0281010764 1037353572.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C5 2.2HDI 133HP 0281010886 353785.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C8 2.2HDI 133HP 0281011779 1037375143.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen C8 2.2HDI 133HP 0281012141 378622.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Jumper 2.8HDI 127HP 0281010932 363533.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Nemo 1.4HDI 1037391713.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Picasso 1.6HDI 90HP 374952.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Picasso 2.0HDI 90HP 0281010595 353363.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Xantia 2.0 IAW8P20 162.21.134.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Xhantia 2.0HDI 109HP 0281010029 359131.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Xsara 2.0HDI 110HP 0281010550 353310.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen Xsara 2.0HDI 90HP 0281010499 353305.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen ZX 1.9 118HP 0261200160 356744.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen berlingo 1.6HDI 90HP 96539589 96618137 377715.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen berlingo 2.0HDI 90HP 5WS40146A-T.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen berlingo 2.0HDI 90HP 5WS40146F-T.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen berlingo 2.0HDI 90HP HW9647423388 5WS40049C-T SW9659517880.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen evasion 2.0HDI 110HP 0281010368 1037353574.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen jumper 2.2HDI 101HP 0281010484 1037363244.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen picasso 1.6HDI 110HP 377720.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen picasso 1.6HDI 90HP 0281011802 371537.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen picasso 2.0HDI 90HP 0281010358 1037353044.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen picasso 2.0HDI 90HP 0281011084 364198.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen saxo 1.6 16V 118HP 16225574.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen saxo 1.6 16v 1AP41 464.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen saxo 1.6i VTS 120HP 0261206214 350812.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xanthia 2.0HDI 0281010251 359146.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xantia 2.0HDI 0281010164 359089.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xantia 2.0HDI 110HP 0281001782 1037359027.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xsara 2.0HDI 110HP 0281010499 353305.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xsara 2.0HDI 110HP 0281010962 1037353913.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xsara 2.0HDI 5WS40023D-T.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xsara 2.0HDI 90HP 0281010595 353363.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xsara 2.0HDI 90HP 0281010996 353949.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xsara 2.0HDi 90HP 0281010362 353148.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xsara picasso 2.0HDI 90HP 0281010137 1037359162.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Citroen xsara picasso 2.0HDI 90HP 0281010750 1037353528.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Flash_bdm.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `JoachimS.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `MPC55x_bdm.ori` | `.ORI` | `459,008` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `P3008_1.6hdi_1037386171 ori.bin` | `.BIN` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `PEUGEOT 5WS40262B-T HW 9655534080 SW 9660780880 SID803A.ORI` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `PEUGEOT 5WS40612B-T HW 9661642180 SW 9664626680 SID803A.ORI` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `PEUGEOT_207_B1600_R4V4T_110kw_xxx_xxx_392034_crc655D7935.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Pegeot 407 1.6HDI 0281011588 374181.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 106 1.4 0261200203 356717.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 106 1.4XSI 0261200203 357243.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 2.0 HDI 0281010842 353821.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 205 1.9 GTI 130HP 0261200162 356149.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.4HDI 68HP 0281010707 363558.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.4HDI 68HP 0281011707 366512.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.4HDI 69HP 0080B680 374477.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.4HDI 69HP 0281010707 363160.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.4HDI 90HP 0281011784 371040.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.4i 1AP-81.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.6HDI 110HP 375528.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.6i 0261208101 366631.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 1.6i 98HP 0261206942 364124.ori` | `.ORI` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281001866 359055.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281010250 359136.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281010250 359222.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281010500 353319.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281010592 353483.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281010594 353648.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281010594 364196.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281010767 353735.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281011188 364378.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281011525 368453.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 206 2.0HDI 90HP 0281011525 374499.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 207 1.4HDI 68HP SW381875.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 207 1.4HDI 90HP 381875.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 207 1.6HDI 110HP 1037379394.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 207 1.6HDI 110HP 1037386112.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 207 RC 1.6 THP 175HP 602 386427.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 207 THP 1.6 150HP 1037394738.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 306 0261204495 356916.ori` | `.ORI` | `262,144` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 306 1.6 16v 0261204062 355982.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 306 2.0HDI 90HP 0281010162 359087.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 306 2.0HDI 90HP 0281010592 353483.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 1.4HDI 90HP 0281011390 1037363557.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 1.6HDI 110HP 0281012465 375963.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 1.6HDI 110HP 1037381884.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 1.6HDI 110HP 386115.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 1.6HDI 90HP 1037375526.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 1.6HDI 90HP 380727.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0 HDI 110HP 028101124810 369509.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 110HP 0281010779 353725.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 110HP 0281010935 364448.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 110HP 0281011081 364193.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 110HP 0281014019 386313.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 0281010163 359088.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 0281010249 359145.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 0281010252 359183.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 0281010935 364309.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 0281011341 371045.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 0281012140 374400.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 5WS40020G-T.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 5WS40020GT.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP 9653205380 5WS40145A-T.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI 90HP Siemens 5WS40045B-T.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 307 2.0HDI-5WS40025D-T.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 308  1.6HDI 1037393476 .ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 405 1.9 110HP 0261200162 355643.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 405 Mi16 19 16V  160bhp 0261200139.bin` | `.BIN` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Peugeot 405 Mi16 19 16V 148bhp 0261200161.bin` | `.BIN` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `Peugeot 406 2.0HDI 0281010033 359065.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 110HP 0281001977 359082.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 110HP 0281010775 1037353610.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 110HP 0281011338 1037364408.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 90HP 0281001978 359083.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 90HP 0281010165 359120.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 90HP 0281010248 353494.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 90HP 0281010248 359169.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 90HP 0281010361 353047.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HDI 90HP 5WS40037D-T.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.0HdI 110HP 0281010363 353049.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.2HDI 133HP 0281010370 353454.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.2HDI 133HP 0281010772 353609.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.2HDI 133HP 0281010772 353776.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.2HDI 133HP 0281011446 368979.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.2HDI 136HP 0281010597 1037353968.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.2HDI 136HP 0281010773 353575.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406 2.2HDI 136HP 02810187710 353776.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 406HDI 110HP 0281011520 369507.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 407 1.6 HDI 0281011558 371807.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 407 1.6HDI 110HP 1037377754.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 407 1.6HDI 381872.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 407 2.0HDI  5WS40167H-T SID 803 Mpc555.ori` | `.ORI` | `462,848` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 407 2.0HDI 136HP 5WS40196E-T 9656413080 965504148.ori` | `.ORI` | `462,848` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 407 2.0HDI 136HP 5WS40204ET 9655041480 9658345280.ori` | `.ORI` | `458,752` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 407 2.0HDI 5WS40167G-T SID 803 Mpc555.ori` | `.ORI` | `462,848` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 407 2.2HDI 170HP 386058.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 607 2.2HDI 133HP 0281010567 353453.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 607 2.2HDI 136HP 0281010765 1037353571.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 607 2.2HDI 136HP 0281010765 353778.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 806 2.0HDI 110HP 028101013 359165.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot 807 2.2HDI 128HP 0281011363 368404.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot Partner 1.6 HDI 90HP 1037393487.ori` | `.ORI` | `2,097,152` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot boxer 2.2HDI 101HP 0281010484 1037369278.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot expert 2.0HDI 110HP 0281010359 353497.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot partner 1037383736.ori` | `.ORI` | `647,168` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot partner 2.0HDI 90HP 0281010360 353444.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot partner 2.0HDI 90HP 5WS40036D-T 9649063480 9644302380.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot partner 2.0HDI 90HP 5ws40155c-t 9653577680 9647423380.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot_405_B1900_R4V4_108kW_0261200161_96027111_1267356020_crc506232A8.ori` | `.ORI` | `32,768` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot_406_B3000_V6V4_140kW_0261204234_9622552780_1037356462_crcDE2363F5.ori` | `.ORI` | `131,073` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Peugeot_807_D2200_R4V4T_98kW_0281011363_B075WF2S010287_NZGG38H2_1037368404_crcC4F58194.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `Pug 206 14HDi 1037368866 Stock.bin` | `.BIN` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `eeprom_bdm.ori` | `.ORI` | `4,096` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `my hdi read.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `original.bin` | `.BIN` | `65,536` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `peugeot 206 1.4HDI 68HP 0281011089 368200.ori` | `.ORI` | `1,048,576` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `peugeot-306-2.0hdi90-0281010249-359145.ori` | `.ORI` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (ORI) |
| `peugeot_306_2.0_hdi_90.0_0281001976_359058.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `peugeot_306_2.0_hdi_90.0_0281010162_359087.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `peugeot_306_2.0_hdi_90.0_0281010249_359145.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `peugeot_306_2.0_hdi_90.0_0281010362_353148.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `peugeot_306_2.0_hdi_90.0_0281010500_353319.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |
| `peugeot_306_2.0_hdi_90.0_0281010592_353483.bin` | `.BIN` | `524,288` bytes | Raw OEM Factory Binary / Hardware Read (BIN) |

---

## 3. Matriks Kalibrasi & Parameter Pemetaan

Bagi berkas biner dan definisi TunerPro / RomRaider yang tersedia, struktur kalibrasi mencakup parameter esensial:
- **Volumetric Efficiency & Fuel Delivery**: Kurva Base Fuel, Open/Closed Loop Transition, Injection Timing, Smoke Limiter, Torque-to-Fuel Limiter, dan Cranking Enrichment.
- **Ignition Timing & Knock Control**: Peta Main Ignition Advance, Low/High Octane Timing, Knock Retard Thresholds, dan Dwell Timing.
- **Airflow & Boost Management**: Peta Target Boost Pressure, Wastegate Duty Cycle (WGDC / N75 Map), MAF/MAP Scaling, dan Throttle Response Curves (Driver Wish).
- **Safety Limits & Thresholds**: Rev Limiter (Hard/Soft Cut), Top Speed Limiter (Vmax), Overboost Fuel Cut, EGT (Exhaust Gas Temperature) Protection, dan Engine Protection Strategies.

---

## 4. Protokol Flashing & Panduan Keamanan

1. **Pemeriksaan Checksum**: Selalu verifikasi dan kalkulasi ulang checksum sebelum menulis firmware kembali ke ECU guna mencegah kondisi *ECU bricking* atau *no-start*.
2. **Pencadangan Full Read (Backup)**: Lakukan full backup (Flash + EEPROM / Microcontroller ROM) sebelum melakukan flashing kalibrasi yang dimodifikasi.
3. **Tegangan Sumber Stabil**: Gunakan unit catu daya terstabilisasi (*bench battery maintainer*) dengan tegangan minimum 13.5V – 14.2V selama sesi flashing OBD2 atau Bootmode.
4. **Kecocokan Hardware & Software**: Jangan pernah melakukan *cross-flashing* berkas kalibrasi ke ECU dengan nomor part hardware yang berbeda tanpa verifikasi arsitektur pinout dan transreceiver bus.
