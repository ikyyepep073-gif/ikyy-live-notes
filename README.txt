IKYY LIVE NOTES — paket siap dipasang

ISI
- index.html: editor dan overlay dalam satu halaman.
- database.rules.json: rules database contoh untuk tes.

CARA MEMAKAI
1. Buat project di https://console.firebase.google.com/
2. Buat Realtime Database.
3. Tambahkan aplikasi Web di Project settings > General > Your apps.
4. Salin Firebase web config ke kolom di situs setelah di-host.
5. Terapkan rules dari database.rules.json pada Realtime Database > Rules.
   PERINGATAN: rules contoh ini membuat catatan publik bisa dibaca/ditulis.
   Gunakan hanya untuk demo/stream pribadi dengan kode room yang sulit ditebak;
   jangan simpan data pribadi. Untuk keamanan produksi, perlu autentikasi dan rules
   yang membatasi akses.
6. Host index.html di HTTPS (misalnya GitHub Pages).
7. Buka URL halaman di HP, isi config, lalu Simpan config.
8. Salin URL Overlay ke OBS > Sources > + > Browser. URL-nya berbentuk:
   https://alamat-host/index.html?overlay=1&room=kode-ruang
9. URL Editor berbentuk:
   https://alamat-host/index.html?room=kode-ruang

CATATAN PENTING
- Belum ada URL publik yang diterbitkan oleh paket ini. Hosting dan konfigurasi
  Firebase harus dibuat dari akun milik pengguna.
- Config web Firebase bukan private key, tetapi jangan pernah menaruh service-account
  key atau rahasia server di HTML.
- Untuk akses editor di perangkat lain, simpan Firebase config pada browser editor itu
  juga, lalu gunakan room yang sama. URL overlay dan editor tidak perlu diubah saat
  teks diperbarui.
