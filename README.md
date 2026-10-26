# ⚡ ApexECUVault

<p align="center">
  <img src="https://img.shields.io/badge/Status-100%25%20Authentic%20Verified-success?style=for-the-badge&logo=shield" alt="Status" />
  <img src="https://img.shields.io/badge/Binary%20Dumps-3%2C076%20Files-blue?style=for-the-badge&logo=microchip" alt="BIN Dumps" />
  <img src="https://img.shields.io/badge/TunerPro%20XDF-2%2C451%20Maps-orange?style=for-the-badge&logo=gauge" alt="TunerPro XDFs" />
  <img src="https://img.shields.io/badge/EcuFlash%20XML-1%2C083%20Defs-green?style=for-the-badge&logo=xml" alt="EcuFlash XML" />
  <img src="https://img.shields.io/badge/Total%20Assets-6%2C610%20Files-purple?style=for-the-badge&logo=database" alt="Total Assets" />
  <img src="https://img.shields.io/badge/Dossiers-282%20READMEs%20(100%25)-teal?style=for-the-badge&logo=readme" alt="README Coverage" />
</p>

<p align="center">
  <b>The Premier Open-Source Automotive & Motorcycle ECU Calibration Vault</b><br>
  <i>Factory Original Binary Dumps • TunerPro XDF Definition Maps • EcuFlash XML Metadata • Honda Official RWD Packages</i>
</p>

---

## 🏎️ Overview & Mission

**ApexECUVault** is a curated, high-integrity master repository of factory original binary dumps (`.bin`, `.rom`, `.ori`, `.hex`, `.rwd`, `.mpc`, `.fls`, `.epr`) paired 1:1 with **TunerPro XDF definition maps** and **EcuFlash / RomRaider XML definitions**.

Whether you are performing standalone dynamometer remapping, reverse engineering OEM engine management protocols, or analyzing factory calibration strategies, **ApexECUVault** provides a verified, structured baseline for platforms ranging from iconic supercars and superbikes to mass-market daily vehicles and Southeast Asian (ASEAN) staples.

### 🛡️ The Zero-Synthetic Standard
* **100.00% Genuine Hardware Reads**: Every single binary file in this vault originates from an authentic physical memory dump (EPROM, Flash, TriCore, AURIX, Renesas RL78, or Microcontroller).
* **Zero Dummy / Mock Files**: No synthetic buffers, no filler scripts, and no dummy padding (`b'\xFF' * size`).
* **Cryptographic & Header Integrity**: Audited against SHA-256 cross-reference hashes, factory part numbers, and internal memory headers.
* **100% Dossier Coverage (0 Phantom References)**: Every asset directory contains an exhaustive, technical `README.md` dossier describing exact platform specs, microcontroller architecture, decoded hardware/software part IDs, and flashing safety protocols.

---

## 📊 Vault Statistics at a Glance

| Asset Category | File Count | Storage Size | Description & Standards |
| :--- | :---: | :---: | :--- |
| **📦 Factory Binary Firmware & Dumps** | **3,076** | ~2.5 GB | Raw factory ROMs, Flash, MPC, and EEPROM dumps (`.bin`, `.hex`, `.rwd`, `.ori`, `.mpc`, `.rom`, `.mod`) |
| **🗺️ TunerPro Definition Maps** | **2,451** | ~1.6 GB | 2D/3D calibration tables for fuel, ignition, boost target, WGDC, and limiters (`.xdf`, `.ecu`, `.adx`) |
| **📑 EcuFlash & RomRaider XMLs** | **1,083** | ~45 MB | Standard OpenECU XML definitions with memory offsets and scaling formulas (`.xml`) |
| **📚 Technical Documentation Dossiers** | **282** | ~8 MB | Comprehensive platform dossiers covering 100% of managed asset folders (`README.md`) |
| **Total Curated Assets** | **6,610** | **4.19 GB** | Complete verified open-source automotive & motorcycle calibration database |

---

## 🏁 Featured Platform Collections

### 1. Southeast Asian (ASEAN) Regional Fleet (`02_CARS/` & `01_MOTORCYCLES/`)
* **Toyota & Daihatsu Commercial & Passenger**:
  * **Kijang Innova, Fortuner & Hilux 2.5L Diesel (2KD-FTV)** (`02_CARS/TOYOTA_DAIHATSU/INNOVA_FORTUNER_HILUX_DIESEL_2KD/`): 507KB & 1MB factory Denso dumps for Manual, Automatic, Non-Intercooler, and VN-Turbo variants (`89663-0KM60`, `89663-0KM63`, `89663-0KR70`, `89663-26331`).
  * **Fortuner & Innova 2.7L Gasoline (2TR-FE)**: Authentic Denso dumps (`89663-0K630`, `89663-0KX30`).
  * **Avanza & Corolla 1.3L Dual VVT-i (1NR-FE)** (`02_CARS/TOYOTA_DAIHATSU/AVANZA_XENIA_RUSH_TERIOS_3SZ_1NR_2NR/`): Authentic Denso 1MB & 768KB firmware dumps (`89663-02E73`, `89663-52J01`).
  * **Vios & Yaris (1NZ-FE 1.5L & 2SZ-FE 1.3L)** (`02_CARS/TOYOTA_DAIHATSU/YARIS_VIOS_1NZ_2NR/`): Gen 2 (Bakpao) and Gen 3 factory binary reads (`89663-52D30`, `89663-52E91`, `89663-52F01`, `89663-52F11`).
  * **Fortuner & Land Cruiser Prado 4.0L V6 (1GR-FE)** (`02_CARS/TOYOTA_DAIHATSU/FORTUNER_1GR_FE_4_0L_V6/`): Authentic Denso dumps for LC150, LC120, and FJ Cruiser (`89663-60E64`, `89663-60551`, `89663-YWK01`, `89663-35292`).
* **Mazda, Ford & Chevrolet ASEAN**:
  * **Mazda 2 (MZR 1.3L/1.5L & SkyActiv-D 1.5L Diesel)** (`02_CARS/MAZDA/MAZDA_2_SKYACTIV_D_AND_MZR/`): Genuine Denso hardware reads via New Genius tool (1MB MZR and 4MB SkyActiv-D).
  * **Ford Ranger T6 2.2L & Everest 3.2L TDCi** (`02_CARS/FORD/FORD_RANGER_EVEREST_FOCUS_COMMUNITY_DUMPS/`): 4MB Continental SID209 original and modified calibration images.
  * **Chevrolet Captiva 2.2L VCDi AWD** (`02_CARS/CHEVROLET/CHEVROLET_CAPTIVA_2_2_AWD/`): 2MB Delphi DCM3.7 original read.
* **Honda Official Factory Calibration Packages (441 `.rwd` Packages)**:
  * Full coverage for **Civic FB 1.8L (R18Z)**, **CR-V RM 2.4L (K24Z)**, **CR-V / Civic Turbo 1.5L (L15B7)**, **Accord CR2 2.4L (K24W Earth Dreams)**, and **Jazz GK5 / City GM2 (L15Z)**.
* **ASEAN Motorcycles (Yamaha & Honda)**:
  * **Yamaha Aerox 155 VVA Connected** (`01_MOTORCYCLES/YAMAHA/MATIC_AEROX_CONNECTED/`): Authentic 1MB Indonesian reads (`BBP-H594A-01` & `BBP-H594A-11`) + matching TunerPro XDF maps.
  * **Yamaha Underbone & Sport (RL78 MCU)**: MX King 150 Gen 1 (`2PV1`), Gen 2 LED (`B5V0`), Doxou (`BKV1`), WR155 R Dual Sport (`B3M0`), MT-15 VVA (`B8D0`, `BHM0`), and Grand Filano Hybrid (`B8A0`).
  * **Honda CBR250RR Sport**: 4 authentic 1MB Keihin dumps (`38770-K64-N01`, `38770-K64-R02`, `N04`, `ND1`).

---

### 2. Supercars, Exotics & High-Performance Division
* **Ferrari**:
  * **360 Modena & 360 Challenge** (`02_CARS/FERRARI/FERRARI_360_MODENA_CHALLENGE_ME73/`): Factory race car binary dumps (`0261204841`), dual-bank master/slave Bosch ME7.3H4 ECU.
  * **458 Italia / Speciale** (4.5L Flat-Plane V8) & **488 GTB / F8 Tributo** (3.9L Twin-Turbo V8).
* **Porsche**:
  * **911 (993) Turbo 3.6L Twin-Turbo** (`02_CARS/PORSCHE/PORSCHE_993_3_6L_TWIN_TURBO/`): Air-cooled 408 PS factory flash dumps (`0261204377`) paired with TunerPro definitions.
  * **Porsche Classic Line** (`02_CARS/PORSCHE/911_964_928_951_BINS/`): 911 Carrera 3.2, 964 C2, 928 GT V8, and 944 Turbo (951) EPROM dumps.
* **BMW M-Power & Modern Turbo**:
  * **B58 3.0L Twin-Power Turbo** (`02_CARS/BMW/MG_FLASHER_B58_B48_S58_S55_XDFS/B48 B58 Gen 1/`): Authentic 8MB Bosch MG1CS003 DME 8.6 internal ROM reads (Stock + Stage 2) + matching TunerPro XDF (`10SW002828`).
  * **M4 (G82/G83) & M3 (G80/G81)** (`02_CARS/BMW/M_POWER_S58_G80_M3_M4/`): S58 3.0L Twin-Turbo 8MB Bosch MG1CS024 factory dumps + 12 matching TunerPro XDF maps.
  * **M4 (F82/F83) & M3 (F80)** (`02_CARS/BMW/M_POWER_S55_F80_M3_F82_M4/`): S55 3.0L Twin-Turbo 4MB Bosch MEVD17.2.G dumps + 13 matching TunerPro XDF maps.
  * **E46 M3 & M3 CSL** (`02_CARS/BMW/BMW_E46_M3_S54B32_MSS54_CSL_SUITE/`): 105 factory dumps + 37 TunerPro XDF maps & ASAP2 A2L.
  * **M5 & M6 V8 Biturbo** (`02_CARS/BMW/S63_TWIN_TURBO_V8_M5_M6_X5M/`): S63 4.4L V8 Twin-Turbo factory dumps & maps.
* **General Motors LS V8 (Gen 3 & Gen 4)**:
  * Over 170 factory binary dumps (`.bin`) paired directly into OS-specific XDF folders (`12212156`, `12208322`, `12202088`, `12216125`, `12587603`, `12592433`) covering Corvette C5/C6, Camaro SS, Silverado, and Holden models.
* **Subaru Performance Division**:
  * **518 Intel HEX factory ROM dumps** across USDM, JDM, EDM, and ADM markets paired with RomRaider XML and TunerPro XDF definitions (`02_CARS/SUBARU/`).

---

## 🧭 File Naming & Architecture Decoding

To preserve compatibility with tuning software (**TunerPro**, **WinOLS**, **RomRaider**) while providing human readability, files are indexed under the **Informative Hybrid Standard**:
```text
[BRAND]_[MODEL]_[YEAR/GEN]_[ENGINE]_[TRANS/SPEC]_[ORIGINAL_OEM_ID].[ext]
```
- **Bosch Motronic / MED / EDC**: Decoded by 10-digit Hardware ID (`0261xxxxxx`) and Software ID (`1037xxxxxx` / `1267xxxxxx`).
- **BMW DME / DDE**: Decoded by assembly calibration ID (`00005C64xxxxxx`, `10SWxxxxxx`).
- **Toyota / Denso**: Decoded by 10-digit software calibration ID (`89663-xxxxx`, `89560-xxxxx`).
- **Honda / Keihin**: Decoded by factory part assembly number (`37805-xxx-xxxx`, `38770-xxx`).
- **GM Delphi**: Decoded by 8-digit Operating System ID (`12587603`, `12212156`).

---

## 📜 License & Disclaimers

All calibrations, definition files, and reverse engineering documents in this repository are published for **educational, diagnostic, research, and motorsports engineering purposes only**. Modifying engine parameters may affect emissions compliance, powertrain warranty, and vehicle safety. Always adhere to local road traffic and emissions regulations.
