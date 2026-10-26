# BMW E-Series Coding & ECU Parameter Database (E46 & E60)
**Maintained by:** Dwi Suryo Nugroho

---

## 🛠️ Hardware & Software

- **Akses Modul & Diagnostik:** NCS Expert, INPA, EDIABAS, Tool32
- **Antarmuka OBD:** Kabel K+DCAN (Chip FT232RL) dengan switch fisik Pin 7/8
- **Flashing DME & Transmisi:** TunerPro, MS43 / MS45 Flash Tool, WinKFP

---

## 📌 1. BMW E46 Coding Database

### A. Body & Kenyamanan (GM5 & ALSZ)

| Fitur | Modul | Parameter NCS Expert | Value | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| Auto-Fold Spion via Remote | `GM5` | `BEIKLAPPEN_B_KOMFORTSCHL` | `aktiv` | Tahan tombol lock remote |
| Buka Kaca & Sunroof via Remote | `GM5` | `KOMFORTOEFFNEN_FB` | `aktiv` | Tahan tombol unlock remote |
| One-Touch Triple Blink | `ALSZ` | `BLINKIMPULSE_CRASHBLK` | `3_impulse` | Khusus LSZ CI 31+ (Facelift) |
| US Sidemarkers | `ALSZ` | `GEDIMMT_BLK_BEI_LICHT` | `aktiv` | Lampu sein depan menyala redup (*amber*) |
| Konfirmasi Suara Locking | `GM5` | `QUIT_OPT_SICHERN` | `aktiv` | Memerlukan modul DWA/sirene alarm |
| Konfirmasi Lampu Hazard Locking | `GM5` | `QUIT_OPT_VERSCHL` | `aktiv` | Hazard kedip saat lock |

### B. Instrument Cluster (AKMB)

| Fitur / Parameter | Modul | Value | Tipe Mesin / Varian | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| Speedometer Digital | `AKMB` | `BC_DIGITAL_GESCHW` | **Semua E46** | Angka kecepatan di layar OBC |
| Indicator Warning RPM | `AKMB` | `WARNANZEIGE_GONG` | **Semua E46** | Warning chime aktif |
| `ZYLINDER_ZAHL` | `AKMB` | `4_zyl` | **318i Only** (M43 / N42 / N46) | Sinyal RPM mesin 4-silinder |
| `ZYLINDER_ZAHL` | `AKMB` | `6_zyl` | **320i, 323i, 325i, 330i** (M52TU / M54) | Sinyal RPM mesin 6-silinder |

### C. Engine Management & Burble Tuning (DME)

- **318i (M43B19 / N42B20 / N46B20):**
  * Bosch M5.2 / ME7.2 (M43): Overrun burble via tabel *ignition map* di TunerPro.
  * Bosch ME9.2 (N42/N46): Valvetronic. Overrun fuel cut-off retard tidak disarankan untuk mencegah malfungsi Valvetronic.
- **323i & 328i (M52TUB25 / M52TUB28 - Siemens MS42):**
  * Map Target: `Overrun Fuel Cutoff Delay` & `Ignition Retard`
  * Duration: `1.0s - 1.5s` | Ignition Retard: `-8°` s.d. `-12°` (2500–4000 RPM)
- **325i & 330i (M54B25 / M54B30 - Siemens MS43):**
  * Parameter: `K_N_OB_N` (Overrun delay)
  * Map Target: `Ignition Retard on Overrun` set `-10°` s.d. `-15°` (2200–4200 RPM) | Min Water Temp: `80°C`

---

## 📌 2. BMW E60 Coding Database

### A. Body & Access (CAS / KGM)

| Fitur | Modul | Parameter NCS Expert | Value | Keterangan |
| :--- | :--- | :--- | :--- | :--- |
| Auto-Fold Spion via Remote | `CAS` / `KGM` | `KOMFORT_EINKLAPP` | `aktiv` | Tahan tombol lock pada remote |
| Buka Sunroof & Kaca via Remote | `CAS` | `KOMFORTOEFFNEN_FB` | `aktiv` | Tahan tombol unlock pada remote |
| Wiper Park Position on Ignition OFF | `KGM` / `RLS` | `WAESCHE_FOLD_INIT` | `aktiv` | Wiper kembali ke posisi bawah saat mesin mati |
| Auto Door Lock at >16 km/h | `CAS` | `VERRIEGELUNG_AUT_AB_X_KMH` | `aktiv` | Mengunci pintu otomatis saat berjalan |

### B. Lighting Module (LMA1 Pre-LCI vs LMA2 LCI)

| Fitur | Modul | Parameter NCS Expert | Value | Kompatibilitas E60 |
| :--- | :--- | :--- | :--- | :--- |
| US Sidemarkers (Amber Lights) | `LMA` | `SIDEMARKER_US` | `aktiv` | E60 Pre-LCI & LCI |
| Welcome Lights Fade-In | `LMA2` | `WELCOME_LIGHT_CUSTOM` | `aktiv` | **E60 LCI Only** (2007–2010) |
| Angel Eyes as DRL | `LMA2` | `VERHALTEN_DRL_TFL` | `drl_s` | **E60 LCI Only** |
| Cornering Fog Lights | `LMA2` | `ABBIEGELICHT_MIT_NSW` | `aktiv` | E60 LCI dengan Xenon Dynamic |

### C. iDrive System (CCC / CIC / MASK)

| Fitur | Modul | Parameter NCS Expert | Value | Tipe iDrive |
| :--- | :--- | :--- | :--- | :--- |
| Volume Bar Display | `CAPPL` / `CIC` | `VOLUME_POPUP` | `aktiv` | CCC / CIC iDrive |
| MP3 Playback Activation | `CAPPL` | `MP3_CCC` | `full` | CCC iDrive (Pre-LCI) |
| Acoustic Lock Menu | `CAPPL` / `CIC` | `ACOUSTIC` | `aktiv` | Tampilan menu ON/OFF alarm di iDrive |

### D. Instrument Cluster, Transmission & DME (KOMBI / EGS / DME)

| Fitur / Modul | Parameter / Tool | Value | Keterangan |
| :--- | :--- | :--- | :--- |
| Speedometer Digital (`KOMBI`) | `DIGITAL_SPEED_DIGITAL` | `aktiv` | Angka kecepatan di cluster MID |
| Gauge Needle Sweep (`KOMBI`) | `INITIAL_SWEEP` | `aktiv` | Sweep jarum indikator saat kontak ON |
| Disable Seatbelt Chime (`KOMBI`) | `GURTWARNUNG_KOMBI` | `nicht_aktiv` | Mematikan alarm sabuk pengaman |
| Sport Transmission 2TB (`EGS`) | WinKFP Flash | `2TB Firmware` | **E60 LCI (ZF6HP21):** Shifting lebih cepat |
| Burble Map Pre-LCI M54 (`DME MS45.1`) | TunerPro | Retard `-10°` s.d. `-15°` | Overrun delay 1.2s - 1.8s |
| Burble Map LCI N52 (`DME MSV70/80`) | TunerPro XDF / BDM | Overrun & Exhaust Flap | Penyesuaian tabel Overrun Fuel Cutoff |

---

## 💻 Sample Code Snippet (`FSW_PSW.MAN`)

```text
# ==========================================
# E46 CODING EXAMPLES
# Author: Dwi Suryo Nugroho
# ==========================================

# Mirror Fold via Remote (Module: GM5)
BEIKLAPPEN_B_KOMFORTSCHL
	aktiv

# Cluster RPM Signal Calibration - 318i 4-Cyl Only (Module: AKMB)
ZYLINDER_ZAHL
	4_zyl

# ==========================================
# E60 CODING EXAMPLES
# Author: Dwi Suryo Nugroho
# ==========================================

# Digital Speedometer on Cluster (Module: KOMBI)
DIGITAL_SPEED_DIGITAL
	aktiv

# Mirror Fold via Remote Fob (Module: CAS)
KOMFORT_EINKLAPP
	aktiv

# Disable Seatbelt Warning Chime (Module: KOMBI)
GURTWARNUNG_KOMBI
	nicht_aktiv

# Enable MP3 CD Support (Module: CAPPL / CCC iDrive)
MP3_CCC
	full
