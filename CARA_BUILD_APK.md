# Cara Dapat APK "Buku Kas" — Semua dari HP, Tanpa Laptop

Project ini akan di-build jadi APK oleh **server GitHub** (gratis), bukan oleh HP kamu.
HP hanya dipakai untuk upload file dan download hasilnya. Ikuti urut dari atas.

## Langkah 1 — Buat akun GitHub
1. Buka github.com lewat Chrome di HP
2. Daftar akun baru (gratis)

## Langkah 2 — Buat repository baru
1. Tap ikon "+" di pojok kanan atas → **New repository**
2. Nama repo: `bukukas` (bebas)
3. Pilih **Public**
4. Tap **Create repository**

## Langkah 3 — Upload semua file project
1. Di halaman repo, tap **Add file** → **Upload files**
2. Extract file zip yang saya berikan pakai aplikasi file manager di HP (biasanya sudah ada fitur "Extract"/"Unzip")
3. Upload SEMUA folder & file hasil extract — pastikan struktur foldernya tetap sama persis (folder `app`, folder `.github`, file `build.gradle`, dst)
   - Kalau browser HP kamu tidak bisa upload folder sekaligus, upload lewat GitHub Desktop di komputer teman, atau pakai aplikasi seperti **Working Copy**/**GitHub Mobile app** yang mendukung upload folder
4. Tap **Commit changes**

## Langkah 4 — Biarkan GitHub build otomatis
1. Setelah file ke-upload, buka tab **Actions** di repo kamu
2. Akan muncul proses "Build APK" yang berjalan otomatis (lambang kuning berputar)
3. Tunggu 3–5 menit sampai tandanya jadi centang hijau ✅

## Langkah 5 — Download APK
1. Masih di tab **Actions**, tap running/selesai job paling atas
2. Scroll ke bawah, ada bagian **Artifacts** → tap `bukukas-debug-apk`
3. File akan terdownload dalam bentuk `.zip`, extract untuk dapat file `app-debug.apk`

## Langkah 6 — Install di HP
1. Buka file `app-debug.apk` dari file manager
2. Kalau muncul peringatan "sumber tidak dikenal", izinkan instalasi (Settings → izinkan install dari sumber ini)
3. Install seperti biasa, aplikasi "Buku Kas" akan muncul di HP

---

**Catatan:** APK hasil build ini adalah versi "debug" — bisa langsung diinstall dan dipakai normal, cuma belum ditandatangani untuk dirilis ke Play Store. Untuk pemakaian pribadi ini sudah cukup.

**Data aman:** Data transaksi tersimpan langsung di HP (local storage aplikasi), tidak terhubung internet, tidak terkirim ke mana pun.
