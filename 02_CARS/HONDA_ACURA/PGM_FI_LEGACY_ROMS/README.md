# PGM FI LEGACY ROMS - ECU Calibration Suite

**Repository Path**: `02_CARS/HONDA_ACURA/PGM_FI_LEGACY_ROMS`  
**Classification**: `Binary Firmware & Calibration Repository`  
**Total Managed Assets**: `232 files` (232 binary dumps, 0 definition maps)  

---

## 1. Technical Platform Overview

Paket direktori `PGM_FI_LEGACY_ROMS` menyediakan pustaka kalibrasi dan pemetaan ECU profesional yang ditujukan bagi teknisi otomotif, tuner, dan reverse engineer. Berkas di direktori ini mencakup kalibrasi firmware pabrikan (OEM), pembacaan perangkat keras (OBD2/BDM/Bench), serta tabel definisi TunerPro XDF untuk eksplorasi parameter mesin.

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
| `203stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `243stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `245stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `248stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `249stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `251stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `269stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `273stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `274stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `304stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `305stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `318stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `332stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `368-d14a2-p1j-stock.bin` | `.BIN` | `32,860` bytes | Binary Firmware / Calibration Dump |
| `MSM66507_365.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `P29-T01-321MCU.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `P54-J00-204MCUwithE2Ext.bin` | `.BIN` | `32,000` bytes | Binary Firmware / Calibration Dump |
| `P61-USDM-215.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `P70-900_259_ZC_VTEC_AT.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `P91-900-253MCU.bin` | `.BIN` | `32,000` bytes | Binary Firmware / Calibration Dump |
| `PK2-6660-53.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `PK2-rom-51.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `PM7-E020-121.bin` | `.BIN` | `16,385` bytes | Binary Firmware / Calibration Dump |
| `PR5-003-59.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `PW0-X00.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `Pm7-0330-50.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `STOCK_PW0-E00_76.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `arduino_ArduiLog_52_mm.ino.eightanaloginputs1.hex` | `.HEX` | `75,696` bytes | Subaru Denso / Hitachi Flash Dump (Intel HEX) |
| `arduino_ArduiLog_52_mm.ino.with_bootloader.eightanaloginputs1.hex` | `.HEX` | `79,408` bytes | Subaru Denso / Hitachi Flash Dump (Intel HEX) |
| `crome gold.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_203stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_243stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_245stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_248stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_249stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_251stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_269stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_273stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_274stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_303stock-P07-D15Z1.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_304stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_305stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_317P28-G02-317.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_318stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_327stock-P28auto.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_332stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_368-d14a2-p1j-stock.bin` | `.BIN` | `32,860` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_37820-P11-G00.bin` | `.BIN` | `32,768` bytes | Honda OBD1/OBD2 ECU Hardware Code `37820-P11` |
| `ecu-roms_37820-P13-Q00.bin` | `.BIN` | `32,768` bytes | Honda OBD1/OBD2 ECU Hardware Code `37820-P13` |
| `ecu-roms_37820-P28-L50.bin` | `.BIN` | `32,768` bytes | Honda OBD1/OBD2 ECU Hardware Code `37820-P28` |
| `ecu-roms_Civ328ex.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Civ409ex.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Civ471hx.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Int338gr.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Int340ls.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Int359tr.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Int422gr.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Int474gr.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Int475ls.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Int497tr.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Int712gr.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_JDMP30_932_311code.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_MSM66507_365.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P07-225--.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P07-900-262MCU.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P08-001-237.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P08-900AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P13-G00-C3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P13-N01-E6.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P13OEMJ50AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P14-A11_stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P28-230.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P29-T01-321MCU.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P30_G00_209_EDM.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P54-J00-204MCUwithE2Ext.bin` | `.BIN` | `32,000` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P61-USDM-215.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P70-900_259_ZC_VTEC_AT.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P73_M66507-715.bin` | `.BIN` | `49,152` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P74-USDM-214.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_P91-900-253MCU.bin` | `.BIN` | `32,000` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PH3-0732-88-89-Accord.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PK2-6660-53.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PK2-rom-51.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PM6-A09-65.bin` | `.BIN` | `17,408` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PM7-E020-121.bin` | `.BIN` | `16,385` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PR3-900-93.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PR3GSR.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PR5-003-59.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_PW0-X00.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Pm7-0330-50.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_STOCK-PM6.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_STOCK-PR3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_STOCK_PW0-E00_76.bin` | `.BIN` | `16,384` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_Stock_P30-901_AT.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_crome gold.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_int233stock.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_ng6001.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_ng60_04.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_obd1-p29-224_normal.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_orgasm_p28.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p05-USDM-231.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p06-301.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p06-import-only.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p06-q00-314.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p07-g01-218.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p07-g01-252.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p08-911-243.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p08-n01-283.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p0a-q50-d5.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p0c-q00-d8.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p0c-q10-L3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p12-a00.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p14-q00-c0.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p14-q52-e4.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p14.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p28-q50-315.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p29-q01-244.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p29-q50-202.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p2p_p75-rom.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p30-010-244MCU-extensionG8.bin` | `.BIN` | `32,000` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p30-900JDM-AT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p30-j00-240.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p39-n50-89.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_p75-q01-270.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pk2-0133-10.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pk2-6214-12.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pk2-6220-27.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pk2-6640-19.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pm6ng_stable.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pr3-901-58.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pr3-j01-205.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pr3-j51-219.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pr4-USDM-232.bin` | `.BIN` | `32,769` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pr4-a02.bin.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pr4-q51-33.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pr4-q60-92.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pr4-q61-235.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pt3-q50-83.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ecu-roms_pt6-j50-d2.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `hts_bins_D14A4@122HP SP98.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `hts_bins_D15B-3stage.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `hts_bins_D15B2@126HP E85.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `hts_bins_D15Z6 E85 147hp.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `hts_bins_D16Z6 Street tuning SP98.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `hts_bins_D16Z6Baserom.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `hts_bins_Y7-Z6Cam9PSI.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `hts_bins_lyonnel 2.0 launch ok.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ng6001.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `ng60_04.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `obd1-p29-224_normal.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p0a-q50-d5.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p0c-q00-d8.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p0c-q10-L3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p29-q01-244.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p29-q50-202.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `p39-n50-89.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `pk2-0133-10.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `pk2-6214-12.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `pk2-6220-27.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `pk2-6640-19.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_bre_JDM_pw0_boost_450cc_60trimT3T4.bin` | `.BIN` | `32,703` bytes | Binary Firmware / Calibration Dump |
| `xenocron_bre_troy.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_bre_turboB16_8.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_1.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_7.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_B201000SC61.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_Crome-Stock-TypeR-P73-240cc.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_Crome4.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_GSRSC611000.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_JCbaseNO2step.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_JoeyBuiltB16.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_Jon-Ls-DA-4.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_JoshTurbolsvtec1.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_New turbo civic map.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_RedHatchDynoTune.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_RuebenDynoTune.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_Wesbase880cc3bar8partial.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b__15Sept05-CromeTuned.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_cheoh.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_chris550-ls-101-3bar.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_final-tune.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_final.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_frankieLSVTAK.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_ryantegafter.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_stock-ls-jason.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_test.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_todabin.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_treyb20.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_v2-stock-ls-jason.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_b_wierd half 110 final 17 psi.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_11psi-FooK.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_2.5tune9final.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_Minimet25450.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_RSmotors tune ZC.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_Stevefinal.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_Tuned-D16y7.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_bang-bin3-450cc-z6.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_d16z657trim450.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_dietz_2.5bar_750cc_race.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_edsohc450cc.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_final-notes.bin` | `.BIN` | `32,923` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_haroon3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_jaredbase.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_jeffsBoostbin.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_jeffsciv23.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_d_steve stock MAP final3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_h_Crome-Stock-H22-P13-240cc.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_crome_h_JDMH22AFINAL.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_hondata_s200_S200-H22A Turbo.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_hondata_s300_LastDyno.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_4gvtectune.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_550supr.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_CRXStockMotorTd0410psiNon-Vtec.bin` | `.BIN` | `32,720` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_D15boost.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_NG55-PM7CurrentTune.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_NG60_Splitime.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_brett1.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_chris-ZC-450-8.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_church7.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng48 DTT.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng48-PR4tune-19.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng48_rory.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng48_rory_2.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng55_25barbasetuned.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng55costum.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng55costum2.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng60_splitime_560cc.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng60_vtec3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_ng60brenttestricher.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_perfect pm7 2.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |
| `xenocron_turboedit_polk1.3.bin` | `.BIN` | `32,768` bytes | Binary Firmware / Calibration Dump |

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
