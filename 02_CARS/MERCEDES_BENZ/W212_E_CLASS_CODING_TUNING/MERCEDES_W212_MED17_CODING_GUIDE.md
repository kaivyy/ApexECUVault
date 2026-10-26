# 🔥Mercedes-Benz W212 Variant Coding & ECU Tuning Database (CODING ECU PANGGANG EDITION)🔥

**Maintained by: Dwi Suryo Nugroho**

Dokumentasi teknis parameter *Variant Coding*, aktivasi *Hidden Features*, dan penyesuaian koding modul untuk Mercedes-Benz E-Class W212 (Pre-Facelift & Facelift).

---

## 🛠️ Hardware & Software Tools

- **Diagnostic & Engineering Software:**
  * **Vediamo (v05.01.01 / v04.02.02)**
  * **DTS Monaco (v8.16 / v9.02)**
  * **Xentry / DAS**
- **Hardware Pasangan OBD:**
  * **Openport 2.0 Tactrix (J2534 PassThru)**
  * **MB SD Connect C4 / C5 / C6 / Xentry VCI**

---

## 📌 1. W212 Pre-Facelift (2009–2012) — Era Twin Headlights ("Lampu Kacang")

### A. Central Gateway (`CGW212.cbf`) & Instrument Cluster (`IC212.cbf`)

| Fitur | Modul | Domain / Parameter | Nilai Baru | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| **AMG Menu Display** | `IC212` | `VCD_Parameter_Atelier` -> `AMG_Menu` | `ja` / `active` | Menampilkan suhu oli, suhu pendingin, & Lap Timer di layar MID. |
| **Remaining Fuel in Liters** | `IC212` | `VCD_Parameter_Atelier` -> `Tankanzeige_Liter` | `ja` | Mengubah indikator bensin dari persen ke angka pasti (Liter). |
| **Belt Warning Chime Off** | `IC212` | `VCD_Parameter_Gurt` -> `Gurtwarnung_akustisch` | `nein` | Mematikan alarm pengingat sabuk pengaman. |
| **Agility / Manual Mode** | `CGW212` | `VCD_Parameter_Getriebe` -> `Fahrprogramm` | `A_S_E_M` | Membuka mode transmisi Agility (A) dan Manual (M) pada 7G-Tronic. |
| **Peringatan Kecepatan (Speed Warning)** | `IC212` | `VCD_Parameter_Warnung` -> `Speed_Warning_120kmh` | `deaktiviert` | Mematikan bunyi alarm saat mobil menyentuh kecepatan 120 km/jam. |

---

### B. Special Setup: Mesin M271 CGI (ECU Bosch MED17.7.2 / "ECU Panggang" 🔥)

> **Maintainer Note:** 
> Penanganan khusus untuk W212 Pre-Facelift (E200/E250 CGI) agar ECU MED17.7.2 tidak matang/retak akibat suhu mesin berlebih (>105°C).

#### Software Fan Control Tuning (`MED177.cbf`)
- **Parameter Target:** `VCD_Lueftersteuerung` / `Cooling Fan Duty Cycle Target Temperature`
- **OEM Default:** Kipas ekstra menyala kecepatan tinggi pada suhu **103°C–108°C**
- **Modified Tuning:** Atur *Threshold Start* kipas radiator menyala pada **92°C–95°C**

#### Physical Heat Shield Upgrade
- Pemasangan *thermal insulation pad* di bawah *bracket* dudukan ECU.
- Spacing / Alumunium Heat Shield di antara manifold dan ECU.

---

## 📌 2. W212 Facelift (2013–2016) — Era Single-Lens LED & FlexRay

### A. Modul SAM & Engine Control Unit (`MED40` / `MED1773`)

| Fitur | Modul | Domain / Parameter | Nilai Baru | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| **ECO Start/Stop Last Mode Memory** | `MED40` / `SAMF212` | `VCD_Parameter_ECO` -> `ECO_Start_Stop_Default` | `Last_User_Mode` | Mengingat posisi terakhir tombol ECO (tidak otomatis ON tiap kontak). |
| **IHC Highbeam Assist Auto** | `SAMF212` | `VCD_Parameter_Licht` -> `IHC_Aktivierung` | `aktiv` | Mengaktifkan bantuan lampu jauh otomatis sesuai kecepatan. |
| **DRL Kecerahan Malam Hari** | `SAMF212` | `VCD_Parameter_TFL` -> `TFL_Dimmung_Nacht` | `20%`–`30%` | Mengatur tingkat kecerahan LED DRL saat lampu utama menyala. |
| **Throttle Response Curve** | `MED1773` / `MED40` | `VCD_Pedal charakteristik` | `Sport / Dynamic` | Mengurangi lag pada pedal gas M274/M276. |

---

## 📌 3. Koding Seluruh Modul Aksesori & Kenyamanan (All W212 Models)

### A. Electronic Seat Adjustment (`ESA_FL` / `ESA_FR`)

| Fitur | Modul | Domain / Parameter | Nilai Baru | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| **Easy Entry / Easy Exit** | `ESA_FL` / `ESA_FR` | `VCD_Parameter_Easy_Entry` -> `Easy_Exit_Seat_Move` | `aktiv` / `30mm` | Kursi otomatis mundur saat mesin dimatikan & pintu dibuka. |
| **Pemanas/Ventilasi Kursi** | `ESA_FL` / `ESA_FR` | `VCD_Parameter_Heating` -> `Temp_Stage_3` | `42°C` | Penyesuaian batas suhu maksimal pemanas/ventilasi kursi. |
| **Seat Memory Lock** | `ESA_FL` / `ESA_FR` | `VCD_Parameter_Memory` -> `Save_Key_Dependent` | `aktiv` | Menyimpan posisi kursi spesifik sesuai remote kunci yang digunakan. |

---

### B. Lighting Control (`SAMF212` & `SAMR212`)

| Fitur | Modul | Domain / Parameter | Nilai Baru | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| **Blinker Touch (Soft Turn)** | `SAMF212` | `VCD_Parameter_Blinker` -> `Tippblinken_Anzahl` | `5 Claps` | Mengubah kedipan lampu sein sekali sentuh dari 3x menjadi 5x. |
| **Adaptive Brake Light** | `SAMR212` | `VCD_Parameter_Licht` -> `Adaptive_Brakelight` | `Blinking_LED` | Lampu rem belakang berkedip cepat saat pengereman mendadak. |
| **US Sidemarkers** | `SAMF212` | `VCD_Parameter_US_Licht` -> `US_Marker_Light` | `aktiv` | Menyala redupkan sein depan bersamaan dengan lampu kota. |
| **Welcome Light Duration** | `SAMF212` | `VCD_Parameter_Licht` -> `Auffindbeleuchtung_Zeit` | `45s` | Menyesuaikan durasi menyala lampu DRL/foglamp saat di-unlock. |

---

### C. Climate Control (`KLA212` / `TAC`)

| Fitur | Modul | Domain / Parameter | Nilai Baru | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| **Air Recirculation Memory** | `KLA212` | `VCD_Parameter_Air` -> `Umluft_Memory` | `aktiv_permanent` | Mencegah sirkulasi luar menyala otomatis setelah 30 menit. |
| **Blower Speed in Auto** | `KLA212` | `VCD_Parameter_Display` -> `Geblaese_Auto_Display` | `aktiv` | Menampilkan indikator kecepatan kipas AC saat mode AUTO. |
| **Max Cooling Tropen Mode** | `KLA212` | `VCD_Parameter_Klima` -> `Klimatisierung_Zone` | `Heissland / Tropen` | Mengoptimalkan kompresor AC & kipas untuk iklim panas. |

---

### D. Head Unit & Audio (`HU45` / `HU5`)

| Fitur | Modul | Domain / Parameter | Nilai Baru | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| **Video In Motion (VIM)** | `HU45` / `HU5` | `VCD_Parameter_Video` -> `Geschwindigkeit_DVD` | `255` | Pemutaran video/DVD di layar utama saat mobil berjalan. |
| **AMG Boot Logo** | `HU45` / `HU5` | `VCD_Parameter_Atelier` -> `Start_Logo` | `AMG_Hallmark` | Mengubah gambar bootscreen COMAND menjadi Logo AMG. |
| **Bluetooth Audio Streaming** | `HU45` | `VCD_Parameter_Bluetooth` -> `BT_Audio_Streaming` | `aktiv` | Membuka fitur Bluetooth Audio pada NTG4.5 awal. |
| **AUX Input Activation** | `HU45` | `VCD_Parameter_Audio` -> `Audio_AUX_Port` | `aktiv` | Membuka channel AUX internal untuk modul Android Box/CarPlay. |

---

### E. Parktronic (`PTS212`) & Power Tailgate (`PTCM`)

| Fitur | Modul | Domain / Parameter | Nilai Baru | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| **Parktronic Early Warning** | `PTS212` | `VCD_Parameter_Ton` -> `Warnung_Auditiv_Start` | `frueh` | Beeper sensor parkir berbunyi dari jarak lebih jauh (zona kuning). |
| **Parktronic Beeper Volume** | `PTS212` | `VCD_Parameter_Ton` -> `Lautstaerke_Hinten/Vorn` | `100%` | Menaikkan volume suara beep sensor parkir. |
| **Remote Power Tailgate Close** | `PTCM` | `VCD_Parameter_Kofferraum` -> `Fernschliessen_Fahrerschalter` | `aktiv_ohne_Hold` | Menutup bagasi belakang cukup sekali tekan dari pintu/remote. |

---

### F. Suspension Control (`AIRMATIC_212`)

| Fitur | Modul | Domain / Parameter | Nilai Baru | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| **Airmatic Lowering** | `AIRMATIC` | `VCD_Parameter_Niveau` -> `Sollhoehe_Fahrwerk` | `-10mm` s/d `-15mm` | Menurunkan ketinggian standar suspensi udara. |

---

## ⚠️ Safety Rules

1. **Voltage Stabilizer:** Pasokan aki wajib di **12.5V – 13.8V** saat *Variant Coding*.
2. **Hard Reset:** Lakukan `FN_ECU_Reset` atau `Hard_Reset` pada modul setelah koding agar parameter aktif.
3. **Backup First:** Selalu backup data variant coding asli (*.txt / *.html*) sebelum melakukan perubahan.

---
