# Myprofitland — Kalkulator Harga Jual

Aplikasi kalkulator biaya produksi & harga jual (dengan pajak pasar, mata uang lokal, dan margin/harga manual) untuk kebutuhan game economy. Berjalan 100% di browser, tanpa server — semua resep tersimpan di penyimpanan browser HP/komputermu sendiri (`localStorage`).

## Isi folder ini

- `index.html` — aplikasinya. Ini satu-satunya file yang wajib ada.

## 1. Upload ke GitHub Pages (hosting gratis, wajib HTTPS)

1. Buat akun di [github.com](https://github.com) kalau belum punya.
2. Klik **New repository** → beri nama bebas, misalnya `myprofitland` → pastikan **Public** → **Create repository**.
3. Di halaman repo, klik **Add file → Upload files**, lalu upload `index.html` dari folder ini.
4. Klik **Commit changes**.
5. Masuk ke **Settings → Pages** (menu di sidebar kiri).
6. Di bagian **Build and deployment → Source**, pilih **Deploy from a branch**, branch **main**, folder **/ (root)** → **Save**.
7. Tunggu 1–2 menit, lalu buka `https://<username-kamu>.github.io/myprofitland/` — aplikasinya harus tampil di sana.

Simpan URL ini, dipakai di langkah berikutnya.

## 2. Bungkus jadi APK Android lewat PWABuilder

1. Buka [pwabuilder.com](https://www.pwabuilder.com) di komputer.
2. Tempel URL GitHub Pages dari langkah 1, klik **Start**.
3. Tunggu proses pemindaian selesai (mengecek manifest & ikon — file ini sudah dilengkapi keduanya).
4. Klik **Package for Store** → pilih **Android**.
5. Biarkan pengaturan default, lalu klik **Generate** / **Download**.
6. Kamu akan dapat file `.zip` berisi:
   - `app-release-signed.apk` → bisa langsung diinstal ke HP untuk dicoba sendiri
   - `app-release-bundle.aab` → dipakai kalau nanti mau upload ke Google Play Store

## 3. Instal APK di HP Android

1. Pindahkan file `.apk` ke HP (kabel USB, Google Drive, WhatsApp ke diri sendiri, dll).
2. Buka file tersebut lewat File Manager di HP.
3. Kalau muncul peringatan, ketuk **Setelan** → aktifkan **Izinkan dari sumber ini** untuk aplikasi yang kamu pakai membuka file.
4. Kembali dan ketuk **Instal**.
5. Aplikasi **Myprofitland** akan muncul di layar utama seperti aplikasi biasa.

## Catatan penting

- Data resep tersimpan **lokal di HP/browser tempat kamu membuka aplikasinya** — tidak otomatis sinkron antar HP atau antar browser berbeda.
- Kalau kamu update `index.html` (misalnya lewat Claude lagi), cukup upload ulang file yang baru ke repo GitHub yang sama (**Add file → Upload files**, timpa yang lama) — tidak perlu ulang proses PWABuilder dari nol kecuali kamu ingin APK baru juga.
- Publikasi resmi ke Google Play Store butuh akun Google Play Console (biaya sekali $25) dan proses review dari Google sebelum bisa diunduh publik.
