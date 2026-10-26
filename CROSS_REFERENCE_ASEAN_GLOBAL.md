# 🌏 Panduan Komparasi Nama Kendaraan: Indonesia vs Luar Negeri (Thailand, Vietnam, Malaysia, Global)

> **Fakta Teknis Penting**: Pabrikan otomotif (Honda, Yamaha, Suzuki, Kawasaki, Toyota, Mitsubishi, Land Rover, Hyundai) sering menggunakan **nama dagang berbeda di tiap negara**, tetapi **arsitektur mesin, pinout kabel, dan kode dasar ECU (*part code*) sama persis**.
> Contohnya: **Honda Vario 150** di Indonesia menggunakan ECU kode **K59**, sama persis dengan **Honda Click 150i** di Thailand & Vietnam. File biner `.bin` dan definisi `.xdf` pada kode tersebut sepenuhnya kompatibel.

---

## 🏍️ 1. Matriks Komparasi Sepeda Motor (Motorcycles)

| Kode ECU | Tahun Produksi | Nama Indonesia | Nama Thailand | Nama Vietnam | Nama Malaysia / Filipina / Global | Vendor ECU & Kapasitas |
| :---: | :---: | :--- | :--- | :--- | :--- | :--- |
| **KVG** | `2014-2019` | **Honda Vario 110 FI** | Honda Click 110i | Honda Click 110i | - | `Keihin 64KB` |
| **K46** | `2015-2020` | **Honda Vario 110 eSP LED** | Honda Click 110i LED | Honda Click 110i | - | `Keihin 64KB` |
| **K60** | `2015-2022` | **Honda Vario 125 eSP (Old & All New)** | Honda Click 125i (LED) | Honda Click 125i (CBU Thai) | Honda Click 125i | `Shindengen / Keihin 256KB` |
| **K2V** | `2023-2026` | **Honda New Vario 125 Facelift** | Honda Click 125i (2023+) | Honda Click 125i (2023+) | Honda Click 125i | `Shindengen 256KB` |
| **K59** | `2015-2022` | **Honda Vario 150 eSP (Old & All New)** | Honda Click 150i | Honda Click 150i | Honda Vario 150 | `Shindengen 256KB` |
| **K2S** | `2022-2026` | **Honda Vario 160 eSP+ (CBS & ABS)** | Honda Click 160 | Honda Air Blade 160 / Vario 160 | Honda Vario 160 | `Shindengen 256KB` |
| **K3V** | `2024-2026` | **Honda Stylo 160 eSP+ (CBS / ABS)** | Honda Giorno+ 125 / Stylo 160 | Honda Giorno+ 125 | Honda Stylo 160 | `Keihin / Shindengen 256KB` |
| **K97** | `2018-2021` | **Honda PCX 150 Lokal & Hybrid** | Honda PCX 150 | Honda PCX 150 | Honda PCX 150 | `Shindengen 256KB` |
| **K1Z** | `2021-2026` | **Honda PCX 160 eSP+ (CBS & ABS)** | Honda PCX 160 e:HEV / STD | Honda PCX 160 | Honda PCX 160 | `Shindengen 256KB` |
| **K0W** | `2019-2022` | **Honda ADV 150** | Honda ADV 150 | Honda ADV 150 | Honda ADV 150 | `Shindengen 256KB` |
| **K0WL** | `2022-2026` | **Honda ADV 160 eSP+** | Honda ADV 160 | Honda ADV 160 | Honda ADV 160 | `Shindengen 256KB` |
| **K25** | `2012-2015` | **Honda BeAT FI & Spacy FI** | Honda Scoopy-i / Spacy-i | Honda Vision 110 (Gen 1) | Honda BeAT 110 | `Keihin 64KB` |
| **K81** | `2016-2019` | **Honda BeAT eSP & Street (Gen 2)** | Honda Moove 110 / Scoopy-i | Honda Vision 110 eSP | Honda BeAT eSP | `Keihin 64KB` |
| **K1A** | `2020-2026` | **Honda All New BeAT & Deluxe (Gen 3)** | Honda Scoopy Prestige | Honda Vision 110 Smart Key | Honda BeAT eSP Facelift | `Keihin / Shindengen 64KB/256KB` |
| **K56** | `2015-2026` | **Honda Sonic 150R & Supra GTR 150** | Honda RS150R | Honda Winner 150 & Winner X | Honda RS150R & RS-X 150 | `Keihin 64KB` |
| **K45A** | `2014-2016` | **Honda CBR150R Dual Keen Eyes (Lokal)** | Honda CBR150R (CBU Thai) | Honda CBR150R | - | `Keihin 64KB` |
| **K45G_N_R** | `2016-2026` | **Honda CBR150R Facelift LED & All New Inverted Fork** | Honda CBR150R LED | Honda CBR150R LED | Honda CBR150R | `Keihin 64KB` |
| **K64** | `2016-2026` | **Honda CBR250RR MC51 (STD, SP, Quickshifter)** | Honda CBR250RR (CBU Indo) | - | Honda CBR250RR | `Keihin SH7058 1MB Flash` |
| **SC82_MKR** | `2020-2026` | **Honda CBR1000RR-R Fireblade SP (SC82)** | Honda CBR1000RR-R Fireblade SP | - | Honda CBR1000RR-R Fireblade SP 217.5PS | `Keihin CANBUS 2MB Flash` |
| **2DP** | `2015-2019` | **Yamaha NMAX 155 V1 (Non-ABS & ABS)** | Yamaha NMAX 155 V1 | Yamaha NM-X 155 | Yamaha NMAX 155 | `Yamaha / Denso RL78` |
| **B6H** | `2020-2024` | **Yamaha All New NMAX 155 Connected (V2)** | Yamaha NMAX 155 Connected | Yamaha NVX 155 Connected | Yamaha NMAX 155 V2 | `Yamaha Connected 1MB Flash` |
| **BLS** | `2024-2026` | **Yamaha NMAX “TURBO” 155 (YECVT)** | Yamaha NMAX Tech MAX 155 | Yamaha NMAX Turbo | Yamaha NMAX Turbo | `Yamaha Dual MCU YECVT CAN` |
| **B65** | `2016-2020` | **Yamaha Aerox 155 VVA Old** | Yamaha Aerox 155 | Yamaha NVX 155 V1 | Yamaha NVX 155 | `Yamaha / Denso RL78` |
| **BBP** | `2021-2026` | **Yamaha All New Aerox 155 Connected** | Yamaha All New Aerox 155 | Yamaha All New NVX 155 Connected | Yamaha NVX 155 V2 Connected | `Yamaha Connected 1MB Flash` |
| **2PV** | `2015-2024` | **Yamaha MX King 150 (V1 & V2)** | Yamaha Exciter 150 | Yamaha Exciter 150 RC / GP | Yamaha Y15ZR (V1 & V2) | `Yamaha / Denso RL78` |
| **B5V** | `2021-2026` | **Yamaha MX King 155 VVA (Generasi Baru)** | Yamaha Exciter 155 VVA | Yamaha Exciter 155 VVA | Yamaha Y16ZR VVA | `Yamaha Denso Gen3` |
| **BK6** | `2017-2021` | **Yamaha YZF-R15 V3 VVA** | Yamaha YZF-R15 V3 | Yamaha YZF-R15 V3 | Yamaha YZF-R15 V3 | `Yamaha / Denso RL78` |
| **BDJ** | `2022-2026` | **Yamaha All New R15 Connected & R15M Quickshifter (V4)** | Yamaha R15 Connected / R15M | Yamaha R15 V4 / R15M | Yamaha R15M Connected-ABS | `Yamaha Denso Gen3 CAN` |
| **CP4_2CR** | `2015-2026` | **Yamaha YZF-R1 & R1M Crossplane (CP4)** | Yamaha YZF-R1 CP4 | - | Yamaha YZF-R1 / R1M Crossplane 200PS | `Mitsubishi / Denso CAN 2MB` |
| **BN6_R6** | `2017-2022` | **Yamaha YZF-R6 BN6 Facelift (M1 Design)** | Yamaha YZF-R6 BN6 | - | Yamaha YZF-R6 BN6 Supersport 118.4PS | `Denso 32-bit CAN 1.5MB` |
| **23K** | `2016-2026` | **Suzuki Satria F150 FI & GSX-R150 / GSX-S150** | Suzuki Raider R150 FI / GSX-R150 | Suzuki Raider R150 FI / GSX-R150 | Suzuki Raider R150 FI / GSX-R150 | `Denso 32-bit` |
| **ZX25R** | `2020-2026` | **Kawasaki Ninja ZX-25R & ZX-25RR (Gen 1 & Gen 2 TFT)** | Kawasaki Ninja ZX-25R | - | Modenas Kawasaki Ninja ZX-25R | `Denso 32-bit CANBUS` |
| **ZX10R** | `2011-2026` | **Kawasaki Ninja ZX-10R Gen 4, Gen 5, Gen 6 Facelift** | Kawasaki Ninja ZX-10R ABS | - | Kawasaki Ninja ZX-10R / ZX-10RR 203PS | `Mitsubishi Electric CAN 2MB` |
| **PANIGALE_V4** | `2018-2026` | **Ducati Panigale V4 & V4S Desmosedici Stradale** | Ducati Panigale V4 | - | Ducati Panigale V4 / V4S / V4R 214PS | `Bosch / Continental TriCore 4MB` |
| **DUKE_790_890** | `2018-2024` | **KTM 790 Duke & 890 Duke R “The Scalpel”** | KTM 790 / 890 Duke | - | KTM 790 / 890 Duke R LC8c Parallel Twin 121PS | `Bosch MG1CA094 TriCore 4MB` |

---

## 🚗 2. Matriks Komparasi Mobil (Cars)

| Kode ECU / Mesin | Tahun Produksi | Nama Indonesia | Nama Thailand | Nama Luar Negeri / Global | Tipe Mesin | Vendor ECU |
| :---: | :---: | :--- | :--- | :--- | :--- | :--- |
| **XFORCE_4A91** | `2023-2026` | **Mitsubishi Xforce Exceed & Ultimate 1.5L CVT** | Mitsubishi Xforce 1.5 MIVEC CVT | Mitsubishi Xforce Compact SUV (4 Drive Modes: Wet/Normal/Gravel/Mud) | 1.5L 4A91 DOHC 16-Valve MIVEC (105 PS / 141 Nm) | `Mitsubishi Melco / Denso Gen3 CAN 2MB` |
| **WRV_L15ZF** | `2022-2026` | **Honda WR-V E & RS 1.5L DOHC i-VTEC (DG4)** | Honda WR-V RS 1.5L | Honda WR-V Gen 2 Small SUV 121PS | 1.5L DOHC i-VTEC L15ZF (121 PS / 145 Nm) | `Keihin SH72543 CAN 2MB Flash` |
| **HRV_L15BG** | `2022-2026` | **All New Honda HR-V RS 1.5 VTEC Turbo (RV5)** | Honda HR-V RS e:HEV / Turbo | Honda HR-V / Vezel Turbo 177PS | 1.5L VTEC Turbo L15BG / L15C (177 PS / 240 Nm) | `Keihin SH72543 CAN 2MB Flash` |
| **DEFENDER_P300** | `2020-2026` | **Land Rover Defender 90/110 P300 2.0T** | Land Rover Defender 90/110 P300 | Land Rover Defender L663 P300 2.0T Ingenium 300PS | 2.0L Turbocharged Inline-4 AJ200 Petrol (300 PS / 400 Nm) | `Bosch MG1CS028 / MED17.8.32 4MB` |
| **DEFENDER_P400** | `2020-2026` | **Land Rover Defender 110/130 P400 3.0 MHEV** | Land Rover Defender 110 P400 MHEV | Land Rover Defender L663 P400 3.0 Inline-6 MHEV + 48V ePou 400PS | 3.0L Inline-6 Turbo MHEV AJ300 (400 PS / 550 Nm) | `Bosch MG1CS028 TriCore 4MB` |
| **DEFENDER_D300** | `2020-2026` | **Land Rover Defender 110 D300 3.0D Twin-Turbo** | Land Rover Defender 110 D300 Diesel | Land Rover Defender L663 D300 3.0L Inline-6 Diesel 300PS 650Nm | 3.0L Twin-Turbo Diesel Inline-6 AJ200D (300 PS / 650 Nm) | `Bosch MD1CS003 TriCore 4MB` |
| **STARGAZER_CRETA_G15** | `2022-2026` | **Hyundai Stargazer, Stargazer X & Creta 1.5 Smartstream** | Hyundai Creta & Stargazer 1.5 | Hyundai Creta / Venue / Stargazer Smartstream G1.5 115PS | 1.5L Smartstream G1.5 MPI Dual Port (115 PS / 144 Nm) | `Kefico / Continental Sim2K-250 2MB` |
| **VELOZ_YARIS_CROSS_2NR** | `2022-2026` | **Toyota All New Veloz, Avanza & Yaris Cross (2NR-VE / Hybrid)** | Toyota Yaris Cross & Veloz 1.5 | Toyota Urban Cruiser Taisor / Yaris Cross AC200 | 1.5L 2NR-VE Dual VVT-i (106 PS) & 2NR-VEX Hybrid (138 PS) | `Denso Gen3 CAN 2MB` |
| **CHERY_OMODA5_TIGGO** | `2023-2026` | **Chery Omoda 5 & Tiggo 7/8 Pro (1.5T / 1.6TGDI)** | Chery Omoda 5 Turbo | Chery Omoda C5 / Tiggo 8 Pro TGDI Acteco | 1.5L Turbo SQRE4T15C (156 PS) / 1.6L TGDI SQRF4J16 (197 PS) | `Bosch MED17.8.10 / MG1US008 4MB` |
| **GR_YARIS_COROLLA** | `2020-2026` | **Toyota GR Yaris & Toyota GR Corolla (G16E-GTS GR-FOUR)** | Toyota GR Yaris & GR Corolla WRC | Toyota GR Yaris / GR Corolla Morizo Edition 304PS | 1.6L 3-Cylinder Turbo G16E-GTS (261 PS / 304 PS) | `Denso Gen3 CANBUS 2MB Flash` |
| **FERRARI_458_488** | `2009-2023` | **Ferrari 458 Italia / Speciale & 488 GTB / F8 Tributo** | Ferrari 458 / 488 GTB | Ferrari 458 Italia 570PS & 488 GTB 670PS V8 | 4.5L Flat-Plane V8 (9000 RPM) & 3.9L Twin-Turbo V8 | `Bosch MED9.6.1 / MED17.3.5 Dual ECU` |
| **FERRARI_360** | `1999-2005` | **Ferrari 360 Modena, Spider & Challenge Stradale** | Ferrari 360 Modena | Ferrari 360 Modena / Challenge Stradale 400PS / 425PS | 3.6L 90° V8 40-Valve DOHC | `Bosch Motronic ME7.3 Dual ECU` |
| **LAMBO_HURACAN_URUS** | `2014-2026` | **Lamborghini Huracan LP610-4 / STO & Urus V8 Turbo** | Lamborghini Huracan & Urus Super SUV | Lamborghini Huracan 5.2L V10 610PS & Urus 4.0T V8 650PS | 5.2L Odd-Firing V10 (8500 RPM) & 4.0L Twin-Turbo EA825 V8 | `Bosch MED17.1.1 / MG1CS008 4MB` |
| **PORSCHE_911_GT3_TURBO** | `2013-2026` | **Porsche 911 GT3 (9000 RPM) & 911 Turbo S VTG** | Porsche 911 GT3 & Turbo S (991/992) | Porsche 911 GT3 4.0L 500PS & Turbo S 3.8L VTG 580PS | 4.0L NA Flat-6 (9000 RPM) & 3.8L Twin VTG Flat-6 | `Bosch MED17.1.11 / Continental SDI21 4MB` |
| **MCLAREN_720S** | `2017-2024` | **McLaren 720S & 765LT Supercar** | McLaren 720S Coupe / Spider | McLaren 720S / 765LT 4.0L Twin-Turbo M840T 720PS | 4.0L Flat-Plane Twin-Turbo V8 M840T | `Bosch MED17.8.33 Dual ECU 4MB` |
| **JIMNY_5DOOR_K15B** | `2018-2026` | **Suzuki Jimny 5-Door & 3-Door (JB74) 4WD ALLGRIP PRO** | Suzuki Jimny 4WD | Suzuki Jimny 5-Door / 3-Door Sierra 1.5L K15B 102PS | 1.5L K15B 16-Valve VVT (102 PS / 130 Nm) | `Bosch ME17.9.61 / Denso CAN 2MB` |
| **2KD** | `2004-2015` | **Toyota Kijang Innova & Fortuner 2.5 D-4D** | Toyota Hilux Vigo & Fortuner 2.5 D-4D | Toyota HiAce & Hilux 2KD-FTV | 2.5L 2KD-FTV D-4D Turbo Diesel Common Rail | `Denso 32-bit` |
| **2GD_1GD** | `2015-2026` | **Toyota Innova Reborn & Fortuner VRZ (2.4 / 2.8 GD)** | Toyota Hilux Revo & Fortuner (2.4 / 2.8 GD) | - | 2.4L 2GD-FTV / 2.8L 1GD-FTV Clean Diesel VN Turbo | `Denso Gen3 (89663-F0xxx)` |
| **1GR** | `2005-2015` | **Toyota Fortuner 4.0L V6 4x4** | - | Toyota Land Cruiser Prado 120/150 4.0L V6 | 4.0L V6 1GR-FE 24-Valve Dual VVT-i | `Denso D76F019xxx` |
| **3SZ_2NR** | `2006-2026` | **Toyota Avanza / Rush & Daihatsu Xenia / Terios** | - | Perodua Myvi / Alza / Aruz | 1.3L K3-VE, 1.5L 3SZ-VE, 1.3L 1NR-VE, 1.5L 2NR-VE | `Denso EFI` |
| **L12B** | `2012-2026` | **Honda Brio Satya & Brio RS 1.2L i-VTEC** | Honda Brio & Brio Amaze 1.2L | - | 1.2L L12B SOHC 4-Cylinder i-VTEC | `Keihin PGM-FI` |
| **L15Z** | `2014-2021` | **Honda Jazz GK5, Mobilio, City, BR-V, HR-V 1.5L** | Honda Jazz GK5 & City 1.5L | Honda Fit / Jazz 1.5L SOHC | 1.5L L15Z i-VTEC SOHC | `Keihin PGM-FI` |
| **4D56** | `2008-2016` | **Mitsubishi Pajero Sport & Triton 2.5 DI-D** | Mitsubishi Pajero Sport & Triton 2.5 Common Rail | Mitsubishi Challenger / Nativa / L200 4D56 | 2.5L 4D56 DI-D Hyper Common Rail Turbo | `Denso Common Rail` |
| **4N15** | `2016-2026` | **Mitsubishi Pajero Sport Dakar & All New Triton 2.4** | Mitsubishi Pajero Sport & Triton MIVEC Diesel | Mitsubishi Montero Sport / L200 MIVEC Clean Diesel | 2.4L 4N15 MIVEC Variable Geometry Turbo Diesel | `Denso Gen3` |
| **MED17_DAZA** | `2017-2021` | **Audi RS3 (8V) & TT RS (8S) 2.5 TFSI** | Audi RS3 Sportback 2.5 TFSI | Audi RS3 / TT RS 2.5 TFSI DAZA 400PS | 2.5L 5-Cylinder Turbo DAZA 400HP | `Bosch MED17.1.62 TriCore TC1793 4MB` |
| **MED9_EA113** | `2004-2009` | **Volkswagen Golf GTI MK5 & Audi A3/S3 2.0 TFSI** | VW Golf GTI MK5 2.0 TSI | VW Golf GTI MK5 / Audi S3 EA113 200PS | 2.0L 4-Cylinder Turbo EA113 200HP | `Bosch MED9.1 MPC562 2MB Flash` |
| **ME7_27T** | `2000-2005` | **Audi S4 B5 & A6 C5 2.7 Biturbo (Collector/Impor)** | Audi S4 2.7 Biturbo | Audi S4 B5 / A6 Allroad 2.7T V6 265PS | 2.7L V6 30-Valve Twin Turbo 265HP | `Bosch ME7.1 / ME7.1.1 1MB Flash` |
| **MSS54_S54** | `2001-2006` | **BMW M3 E46 3.2L & M3 CSL (S54B32)** | BMW M3 E46 Coupe S54 | BMW M3 E46 / M3 CSL 343PS / 360PS | 3.2L Inline-6 S54B32 343HP / 360HP | `Siemens MSS54 / MSS54HP Dual MCU` |
| **5AA_L15B** | `2016-2026` | **Honda Civic Turbo Sedan/Hatchback & Civic RS (FC1/FK7/FE)** | Honda Civic Turbo RS / Hatchback | Honda Civic 1.5L Turbo L15B7 / L15CA | 1.5L DOHC VTEC Turbo L15B7 173PS / 182PS | `Keihin SH7058 / SH72543 1MB / 2MB` |
| **4A91** | `2017-2026` | **Mitsubishi Xpander & Xpander Cross 1.5L MIVEC** | Mitsubishi Xpander 1.5L | - | 1.5L 4A91 DOHC 16-Valve MIVEC | `Mitsubishi / Melco` |

---

## 💡 Tips Praktis untuk Tuner / Remapper:
1. **Periksa 3 Huruf/Angka Tengah Part Number**:
   - Contoh pada Honda: `38770-K59-A11` -> Kodenya adalah **K59** (Vario 150 Indo = Click 150i Thai).
   - Contoh pada Yamaha: `2PV-H591A-00` -> Kodenya adalah **2PV** (MX King Indo = Exciter 150 Vietnam = Sniper 150 Filipina = Y15ZR Malaysia).
   - Contoh pada Mitsubishi: `1860E035` -> ECU Mitsubishi Xforce 1.5 MIVEC CVT.
   - Contoh pada Honda WR-V / HR-V: `37820-63R-N01` (WR-V L15ZF) & `37820-64A-A01` (HR-V RS Turbo L15BG).
2. **Periksa Ukuran File Flash Binary**:
   - Honda Keihin Matic Kecil (Beat/Vario 110): `64 KB` (65,536 bytes).
   - Honda Shindengen Smart Key (Vario 125/150/160, PCX 160, Scoopy K2F): `256 KB` (262,144 bytes).
   - Yamaha Renesas RL78 (MX King, NMAX, Vixion, WR155): `27 KB` (blok kalibrasi) atau `64 KB` / `128 KB`.
   - Yamaha Connected (Aerox BBP, NMAX B6H): Full Flash `1 MB` (1,048,576 bytes).
   - Honda CBR250RR MC51: Full Flash `1 MB` (Renesas SH7058).
   - Toyota Denso Diesel (2KD / 1GD / 2GD): `1.5 MB`, `2 MB`, atau `4 MB`.
   - Honda Mobil Turbo / NA (Civic RS, WR-V, HR-V): `2 MB` (Keihin SH72543).
   - Mitsubishi Xforce (4A91 CVT): `2 MB` (Melco Gen3 CAN).
   - Land Rover Defender L663 (P300/P400/D300): `4 MB` (Bosch MG1CS028 / MD1CS003 TriCore).
3. **Cross-Flashing Warning**:
   - Meskipun peta kurva bahan bakar dan pengapian dapat ditiru antar negara menggunakan file `.xdf`, **jangan menimpa (*cross-flash*) file biner mentah secara langsung** jika terdapat perbedaan fitur immobilizer/Smart Key, sensor O2 heater, atau standar emisi Euro3 vs Euro4.