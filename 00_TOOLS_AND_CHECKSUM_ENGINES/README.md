# 🛠️ Direktori Utilitas, Engine Checksum & Spesifikasi Memori ECU

Direktori ini memuat perangkat lunak bantu (scripts, checksum engines, pinout wiring, dan spesifikasi batasan memori) yang esensial untuk proses flashing dan tuning.

---

## 📁 Daftar Tool & Direktori

1. **`MOTO_ECU_CHECKSUM/`**:
   - Engine Python untuk verifikasi dan kalkulasi perbaikan checksum firmware motor:
     * Bosch MSE6.0 & MSE8.0 (CFMoto, Benelli, KTM)
     * Bosch MG1 (KTM 790/890)
     * Honda Keihin (X-ADV 750, ADV 350)
     * Yamaha (MT-07, MT-09, R1, R6)
     * Italjet Dragster / Suzuki
     * Dell'Orto EFI

2. **`TOYOTA_DENSO_XDF_TOOL/`**:
   - Generator otomatis TunerPro XDF untuk ECU Toyota Denso microcode D76F019xxx (Innova, Fortuner, Hilux 2KD/1GD/2GD).

3. **`PINOUTS_AND_DTC_DATABASES/`**:
   - Skema pinout konektor ECM 33-PIN dan 39-PIN untuk seluruh varian matic dan sport Honda.
   - Database koneksi Yamaha K-Line vs CANBUS untuk 101 model.
   - Tabel referensi DTC fault code motor Honda & Yamaha.

4. **`YAMAHA_HONDA_FLASH_SPECS/`**:
   - `YAMAHA_ECU_MEMORY_WRITE_BOUNDARIES.txt`: Penjelasan area baca/tulis terlindungi (*protected vs writable map area*) untuk ECU Renesas 64KB dan 128KB.
   - `YamahaFlasher_support_list.xls`: Matriks dukungan hardware dan software flasher Yamaha.
