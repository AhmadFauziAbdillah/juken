# 🏍️ Juken 5+ Vario ECU Mapper

Auto Mapping ECU dengan Bluetooth Live Data untuk Honda Vario menggunakan ECU Juken 5+.

---

## 🚀 CARA DAPAT APK — 5 LANGKAH MUDAH

### Tidak perlu install Android Studio atau tools apapun!

---

### LANGKAH 1 — Buat akun GitHub (gratis)
Buka https://github.com dan daftar akun baru.

---

### LANGKAH 2 — Buat repository baru
1. Klik tombol **"New"** / **"+"** di pojok kanan atas
2. Isi nama repo: `juken5plus-mapper`
3. Pilih **Public**
4. Klik **"Create repository"**

---

### LANGKAH 3 — Upload semua file ini ke GitHub

Klik **"uploading an existing file"** lalu upload semua file berikut dengan **struktur folder yang sama**:

```
📁 .github/
   📁 workflows/
      📄 build-apk.yml        ← WAJIB, jangan sampai salah path!
📁 www/
   📄 index.html
📄 package.json
📄 capacitor.config.json
📄 README.md
```

> ⚠️ PENTING: Folder `.github/workflows/` harus dibuat manual di GitHub.
> Caranya: Saat upload, di kolom nama file ketik `.github/workflows/build-apk.yml`
> GitHub akan otomatis buat foldernya.

Klik **"Commit changes"** setelah upload.

---

### LANGKAH 4 — Cek proses build
1. Buka tab **"Actions"** di repository kamu
2. Kamu akan lihat workflow **"Build Juken 5+ APK"** sedang berjalan
3. Tunggu sekitar **5-10 menit**
4. Status hijau ✅ = BUILD SUKSES

---

### LANGKAH 5 — Download APK
**Cara 1 — Via Releases (paling mudah):**
- Klik tab **"Releases"** di sidebar kanan
- Download file `juken5plus-vario-mapper-v1.0.apk`

**Cara 2 — Via Actions Artifacts:**
- Klik tab **"Actions"**
- Klik build yang sudah selesai
- Scroll ke bawah, klik **"Juken5Plus-APK"** untuk download

---

## 📱 INSTALL APK DI HP ANDROID

1. Transfer APK ke HP (WhatsApp, email, atau kabel USB)
2. Buka **Settings → Security**
3. Aktifkan **"Install from unknown sources"** (atau "Install unknown apps")
4. Buka file APK → Install
5. Buka app **"Juken 5+ Mapper"**

---

## 🔵 KONEKSI BLUETOOTH

### Modul BT yang didukung:
| Modul | Tipe | Keterangan |
|-------|------|-----------|
| HC-05 | Classic BT | Paling umum, harga murah |
| HM-10 | BLE 4.0 | Lebih stabil, hemat baterai |
| JDY-08 | BLE 4.0 | Alternatif HM-10 |

### Cara koneksi:
1. Pasang modul BT ke ECU Juken 5+
2. Nyalakan motor → LED modul BT berkedip cepat = siap pairing
3. Buka app → tap **CONNECT BT**
4. Pilih nama modul (misal: `HC-05`, `JUKEN5+`, `HM-10`)
5. Masukkan PIN jika diminta: **1234** atau **0000**
6. Selesai! Live data mulai mengalir 🎉

---

## ✨ Fitur App

- 🗺️ **Auto Mapping 84 cell** (12 RPM × 7 TPS)
- 📊 **Live data** RPM, TPS, MAP, O2, ECT, IAT, Injector Duty, Ignition Advance
- ⚡ **Flash ECU** via Bluetooth
- 💾 **Save/Load map** file `.jkn`
- 🎯 **4 map:** Fuel, Ignition Timing, IAT Correction, Target AFR
- 📈 **Live chart** RPM / AFR / Load real-time

---

## ❓ TROUBLESHOOTING

| Masalah | Solusi |
|---------|--------|
| Actions tidak jalan | Pastikan file ada di `.github/workflows/build-apk.yml` |
| Build gagal | Lihat log di tab Actions, klik step yang merah |
| BT tidak ketemu | Pastikan modul dalam mode pairing (LED kedip cepat) |
| App crash | Pastikan izin Bluetooth diberikan di Settings HP |
