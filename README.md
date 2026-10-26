# ⚡ ApexECUVault

<p align="center">
  <img src="https://img.shields.io/badge/Status-100%25%20Authentic%20Verified-success?style=for-the-badge&logo=shield" alt="Status" />
  <img src="https://img.shields.io/badge/Binary%20Dumps-2%2C496%20Files-blue?style=for-the-badge&logo=microchip" alt="BIN Dumps" />
  <img src="https://img.shields.io/badge/TunerPro%20XDF-2%2C457%20Maps-orange?style=for-the-badge&logo=gauge" alt="TunerPro XDFs" />
  <img src="https://img.shields.io/badge/EcuFlash%20XML-1%2C083%20Defs-green?style=for-the-badge&logo=xml" alt="EcuFlash XML" />
  <img src="https://img.shields.io/badge/Total%20Assets-6%2C280%2B%20Files-purple?style=for-the-badge&logo=database" alt="Total Assets" />
</p>

<p align="center">
  <b>The Premier Open-Source Automotive & Motorcycle ECU Calibration Vault</b><br>
  <i>Factory Original Binary Dumps • TunerPro XDF Definition Maps • EcuFlash XML Metadata • Checksum Engines</i>
</p>

---

## 🏎️ Overview & Mission

**ApexECUVault** is a curated, high-integrity master repository of factory original binary dumps (`.bin`, `.rom`, `.ori`, `.hex`, `.mpc`, `.fls`, `.epr`) paired 1:1 with **TunerPro XDF definition maps** and **EcuFlash / RomRaider XML definitions**.

Whether you are performing standalone dynamometer remapping, reverse engineering OEM engine management protocols, or analyzing factory calibration strategies, **ApexECUVault** provides a verified, structured baseline for platforms ranging from iconic supercars and superbikes to mass-market daily vehicles.

### 🛡️ The Zero-Synthetic Standard
* **100.00% Genuine Hardware Reads**: Every single binary file in this vault originates from an authentic physical memory dump (EPROM, Flash, TriCore, AURIX, or Microcontroller).
* **Zero Dummy / Mock Files**: No synthetic buffers, no filler scripts, and no dummy padding (`b'\xFF' * size`).
* **Cryptographic Integrity**: Audited against SHA-256 cross-reference hashes from verified international community archives and bench read backups.

---

## 📊 Vault Statistics at a Glance

| Asset Category | File Count | Description & Standards |
| :--- | :---: | :--- |
| **📦 Factory Binary Dumps** | **2,496** | Raw factory ROMs, Flash, MPC, and EEPROM dumps (`.bin`, `.hex`, `.ori`, `.rom`, `.fls`, `.mpc`, `.epr`) |
| **🗺️ TunerPro Definition Maps** | **2,457** | 2D/3D calibration tables for fuel, ignition, boost target, WGDC, and limiters (`.xdf`, `.ecu`, `.adx`) |
| **📑 EcuFlash & RomRaider XMLs** | **1,083** | Standard OpenECU XML definitions with memory offsets and scaling formulas (`.xml`) |
| **🛠️ Checksum Engines & Project Maps** | **730+** | WinOLS `.ols` projects, map packs (`.kp`), checksum plugins (`.dll`), and technical dossiers |
| **Total Curated Assets** | **6,280+** | **3.71 GB** of verified calibration data |

---

## 🏁 Featured Platform Collections

### 1. Supercars, Exotics & High-Performance Division
* **Ferrari**:
  * **360 Modena & 360 Challenge** (`02_CARS/FERRARI/FERRARI_360_MODENA_CHALLENGE_ME73/`): Factory race car binary dumps (`0261204841`), dual-bank master/slave Bosch ME7.3H4 ECU.
  * **458 Italia / Speciale** (4.5L Flat-Plane V8) & **488 GTB / F8 Tributo** (3.9L Twin-Turbo V8).
* **Porsche**:
  * **911 (993) Turbo 3.6L Twin-Turbo** (`02_CARS/PORSCHE/PORSCHE_993_3_6L_TWIN_TURBO/`): Air-cooled 408 PS factory flash dumps (`0261204377`) paired with TunerPro MAF definitions.
  * **Porsche Classic Line** (`02_CARS/PORSCHE/911_964_928_951_BINS/`): 911 Carrera 3.2, 964 C2, 928 GT V8, and 944 Turbo (951) EPROM dumps and XDFs.
  * **911 GT3 (991/992)** 4.0L High-Rev Flat-6 & **911 Turbo S** 3.8L VTG definitions.
* **BMW M-Power & Alpina**:
  * **M4 (G82/G83) & M3 (G80/G81)** (`02_CARS/BMW/M_POWER_S58_G80_M3_M4/`): S58 3.0L Twin-Turbo 8MB Bosch MG1CS024 factory dumps + 12 matching TunerPro XDF maps.
  * **M4 (F82/F83) & M3 (F80)** (`02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/`): S55 3.0L Twin-Turbo 4MB Bosch MEVD17.2.G dumps + 13 matching TunerPro XDF maps.
  * **E46 M3 & M3 CSL** (`02_CARS/BMW/BMW_E46_M3_S54B32_MSS54_CSL_SUITE/`): 105 factory dumps (6MT, SMG, CSL, EU, US) + 37 TunerPro XDF maps & ASAP2 A2L.
  * **M5 & M6 V8 Biturbo** (`02_CARS/BMW/S63_TWIN_TURBO_V8_M5_M6_X5M/`): S63 4.4L V8 Twin-Turbo factory dumps & maps.
  * **Alpina B3 3.0 (E36)**: Rare hand-crafted 250 PS Bosch DME 413 red label binary dump.
* **Audi & VAG High-Performance**:
  * **RS4 Avant (B5)** (`02_CARS/VAG_AUDI_VOLKSWAGEN/AUDI_RS4_B5_2_7TT_COSWORTH/`): 2.7T Biturbo Cosworth 381 PS binary dump (`8D0907551F`) + 3.2MB TunerPro XDF.
  * **TT RS & RS3 2.5 TFSI** (`02_CARS/VAG_AUDI_VOLKSWAGEN/AUDI_TTRS_RS3_MED17_1_62/`): 5-cylinder DAZA / CEPA Bosch MED17.1.62 factory binaries + matching XDFs.
  * **Golf GTI Mk5 & Mk4**: 2.0 TFSI Bosch MED9.1 and 1.8T Motronic M3.8.3 binaries + XDFs.
* **Chevrolet & American Muscle**:
  * **Corvette C5** (`02_CARS/CHEVROLET/CHEVROLET_CORVETTE_C5_LS1_V8/`): 5.7L LS1 V8 Manual 6-speed factory dump (OS `12587603`) + TunerPro XDFs.
  * **Cadillac CTS-V LS6**, Corvette C5 Z06, Silverado SS, Hummer H2 6.0L LQ4, 8.1L Big Block L18.

### 2. JDM & Domestic Legends
* **Nissan & Infiniti**:
  * **Skyline GT-R** (BNR32, BCNR33, BNR34 RB26DETT twin-turbo original factory EPROM dumps).
  * **Skyline GTS-t / GT-T** (HCR32, ECR33, ER34 NEO RB25DET 70+ dumps).
  * **Silvia & 180SX** (S13, S14, S15 SR20DET Redtop, Blacktop, Type-X 84+ dumps).
  * **Fairlady Z (300ZX Z32)** VG30DETT twin-turbo and GT-R R35 VR38DETT definitions.
* **Toyota & Daihatsu**:
  * **Supra 2JZ-GTE / 1JZ-GTE** (JZA80) & Supra MK5 (A90 B58) calibration maps.
  * **GR Yaris & GR Corolla** (G16E-GTS 1.6L 3-cylinder Turbo).
  * **Classic Icons**: 4A-GE 16V/20V Silvertop/Blacktop and 1UZ-FE 4.0L V8 dumps.
* **Subaru**:
  * Over 500 authentic binary dumps covering Impreza WRX, WRX STI (EJ20, EJ257, EJ255), Legacy GT, and Forester XT paired with 675 RomRaider definitions.

### 3. ASEAN & Emerging Market Platforms
* **Mitsubishi**:
  * **Destinator / DST Concept (2025–2026)** (`02_CARS/MITSUBISHI/DESTINATOR_DST_CONCEPT_2025_2026/`): Engineering dossier for the Melco Gen3 CAN architecture (SH72543 / MH8115F), UDS Seed/Key protocols, and bench flashing procedures.
  * **Xforce 1.5L CVT** (1860E035) & **Xpander 1.5L MIVEC** (1860Bxxx).
  * **Pajero Sport**: 4N15 2.4L MIVEC Commonrail Diesel & 4D56 2.5L DI-D.
  * **Magna, Diamante & Ralliart 3.5L V6**: 15 genuine factory hex dumps + 31 EcuFlash XML definitions.
  * **Lancer Evolution**: Complete TephraMOD XML definition suite for Evo 5, 6, 7, 8, 9, and 10.
* **Toyota / Daihatsu ASEAN**:
  * Innova Reborn & Fortuner VRZ (2GD-FTV 2.4L & 1GD-FTV 2.8L VN Turbo).
  * Innova & Fortuner 2KD-FTV 2.5L Commonrail Diesel.
  * Avanza, Xenia, Rush, Terios, Veloz, Yaris Cross (Dual VVT-i 1NR-VE, 2NR-VE, 3SZ-VE).
* **Honda ASEAN**:
  * Civic Turbo 1.5L (L15B7 Earth Dreams), Brio 1.2L (L12B), Jazz GK5 / City / Mobilio (L15Z), WR-V & All New HR-V (L15ZF).

### 4. Motorcycle Superbike & Sport Division
* **Suzuki**: GSX-R1000 K5/K6 Denso (`32920-41G00`) full bin & XDF pair, Hayabusa GSX-1300R, GSX-R600/750, GSX-R150, Satria F150 FI.
* **Honda**: CBR1000RR Fireblade, CBR600RR, CBR250RR MC51 Twin, CB150R, CRF150L/250L, Beat, Vario 125/160, PCX 160, ADV 160, Stylo 160.
* **Yamaha**: YZF-R1, R6, R15 V3/V4 VVA, R25, MT-15, NMAX 155, Aerox 155 Connected, WR155R, Fazzio & Grand Filano Blue Core Hybrid.
* **Kawasaki**: Ninja ZX-25R 4-cylinder, ZX-6R 636, ZX-10R, Ninja 250 FI, KLX150, KLX230.
* **European & American Motorcycles**: Ducati 900 SS AM28F010, Panigale V4, Buell BUEIA V5, Moto Guzzi IAW15M, and Harley-Davidson Delphi Centurion dumps.

---

## 📁 Repository Directory Structure

```
ApexECUVault/
├── 00_TOOLS_AND_CHECKSUM_ENGINES/    # Checksum engines, algorithms, and flash pinout specs
│   ├── MOTO_ECU_CHECKSUM/            # Keihin, Shindengen, Denso, Bosch checksum modules
│   └── YAMAHA_HONDA_FLASH_SPECS/     # Hardware bench flashing wiring and boot pinouts
│
├── 01_MOTORCYCLES/                   # Two-wheeler calibration files (.bin & .xdf)
│   ├── BUELL/                        # Buell BUEIA ECU definitions & ADX logging
│   ├── DUCATI/                       # Ducati 900 SS, Monster, Panigale V4 Marelli
│   ├── HARLEY_DAVIDSON_INDIAN/       # Delphi Centurion dyno calibration dumps
│   ├── HONDA/                        # CBR1000RR, CBR250RR, CRF, Vario, Beat, PCX, Stylo
│   ├── KAWASAKI/                     # Ninja ZX-25R 4-cyl, ZX-6R, ZX-10R, Ninja 250
│   ├── MOTO_GUZZI/                   # Moto Guzzi IAW15M P7 GuzziDiag definitions
│   ├── SUZUKI/                       # GSX-R1000 Denso, GSX-R150, Satria FU FI DOHC
│   └── YAMAHA/                       # YZF-R1, R15 VVA, R25, NMAX 155, Aerox, WR155R
│
├── 02_CARS/                          # Passenger, sport, and supercar calibrations
│   ├── ALFA_ROMEO/                   # Bosch Motronic M1.x/M3.x definitions (GTV, 155, SZ)
│   ├── BMW/                          # S58 (M4 G82), S55 (M4 F82), S54 (M3 CSL), S63, N54, Alpina
│   ├── CHEVROLET/                    # Corvette C5 5.7L LS1 V8 Manual, Captiva 2.2 AWD
│   ├── FERRARI/                      # 360 Challenge & 360 Spider Bosch ME7.3H4
│   ├── FORD/                         # Fox Body Mustang 5.0L A9L, Falcon Barra Turbo, Ranger SID209
│   ├── GENERAL_MOTORS/               # GM LS V8 Gen III / Gen IV P01 & P59 calibrations
│   ├── GM_CHEVROLET/                 # Duramax 6.6L LBZ/LMM, Silverado SS, Tahoe, Hummer H2
│   ├── HONDA_ACURA/                  # Acura NSX, Civic Turbo L15B, Brio L12B, Jazz, K20, B16/B18
│   ├── HYUNDAI_KIA/                  # Genesis G70/Stinger SIM2K-250, Santa Fe 2.2 CRDi, Creta
│   ├── MAZDA/                        # MX-5 Miata NC 2.0L MZR, Mazda 2 SkyActiv-D, RX-8
│   ├── MITSUBISHI/                   # Destinator Melco Gen3, Xforce, Xpander, Pajero Sport, Magna, Evo
│   ├── MULTI_BRAND_COMMUNITY_TUNES/  # Global tuner community verified calibrations
│   ├── NISSAN_INFINITI/              # Skyline GT-R RB26DETT, Silvia SR20DET, 300ZX VG30DETT
│   ├── PORSCHE/                      # 911 993 Turbo 3.6T Air-Cooled, 964 C2, 928 GT, 944 Turbo
│   ├── SUBARU/                       # Impreza WRX STI EJ20/EJ25 (500+ authentic dumps)
│   ├── TOYOTA_DAIHATSU/              # Innova/Fortuner 1GD/2GD/2KD, GR Yaris, Supra 2JZ, Avanza
│   ├── VAG_AUDI_VOLKSWAGEN/          # Audi RS4 B5 Cosworth, TT RS/RS3 MED17, Golf GTI MED9/M3.8
│   └── VOLVO_SAAB/                   # Volvo S60R/V70R ME7, Redblock LH-Jetronic, Saab Trionic
│
├── CROSS_REFERENCE_ASEAN_GLOBAL.md    # Global ECU hardware to regional vehicle cross-reference
└── PANDUAN_PRAKTIS_REMAP_TUNERPRO.md # Step-by-step practical TunerPro remap guide
```

---

## 🛠️ Recommended Software & Tools

| Software Tool | Primary Function | Compatible Formats |
| :--- | :--- | :--- |
| **[TunerPro / TunerPro RT](http://www.tunerpro.net/)** | 2D/3D table visualizer and calibration editor | `.bin`, `.hex`, `.ori`, `.xdf`, `.adx` |
| **[EcuFlash (OpenECU)](http://www.tactrix.com/)** | Tactrix OpenPort reflasher and map viewer | `.bin`, `.hex`, `.xml` |
| **[RomRaider](https://www.romraider.com/)** | Open-source tuning editor and live logger | `.bin`, `.hex`, `.xml` |
| **[WinOLS (EVC)](https://www.evc.de/)** | Professional hex binary editor & map discovery | `.ols`, `.kp`, `.bin` |
| **[PCMFlash](https://pcmflash.ru/) / [BitBox](https://bitbox.ru/)** | Bench, Boot, and OBD flashing hardware interfaces | Raw micro/flash memory dumps |

---

## ⚖️ Disclaimer & License

* **Educational & Research Purpose**: The data contained within this repository is compiled strictly for automotive reverse engineering, calibration study, software development, and non-commercial educational research.
* **Safety & Regulatory Compliance**: Modifying engine control parameters (such as emissions devices, boost pressure, rev limits, or fuel tables) may violate motor vehicle emissions regulations and warranty policies in your jurisdiction. The maintainers assume no liability for mechanical damages, ECU bricking, or regulatory non-compliance resulting from the use of these files.
* **Integrity Guarantee**: All trademarks, brand names, and part numbers belong to their respective manufacturers and are cited strictly for identification and vehicle compatibility indexing.

---

<p align="center">
  <b>ApexECUVault</b> • Maintained with technical rigor by enthusiasts, for enthusiasts.<br>
  <i>Crafted by <a href="https://github.com/kaivyy">kaivyy</a></i>
</p>
