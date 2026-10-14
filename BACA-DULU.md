# Rolling Tenis (versi aplikasi HP)

Isi folder ini:

- `index.html` : aplikasinya
- `manifest.webmanifest` dan `sw.js` : bagian yang membuatnya bisa dipasang dan dibuka tanpa internet
- `icons/` : logo bola tenis (ikon tab browser, ikon layar utama)

## Penting: harus ditaruh di web dulu

Aplikasi seperti ini hanya bisa dipasang kalau dibuka lewat alamat `https://`. Kalau file `index.html` dibuka langsung dari folder HP atau laptop, aplikasinya tetap jalan, tapi tombol "Pasang" dan mode offline tidak aktif.

Cara paling gampang (gratis), pilih salah satu:

1. **Netlify Drop**: buka app.netlify.com/drop, lalu seret folder ini (sudah di-unzip) ke halamannya. Kamu langsung dapat alamat https.
2. **GitHub Pages**: taruh semua file di satu repository, lalu aktifkan Pages di pengaturan repository.
3. **Cloudflare Pages**: buat project baru, pilih upload langsung, lalu unggah folder ini.

Semua file harus ada di satu folder yang sama, dengan susunan seperti sekarang (folder `icons` tetap di sebelah `index.html`).

## Memasang di HP

- **Android (Chrome)**: buka alamatnya, lalu tekan tombol "Pasang di HP" di pojok atas aplikasi. Kalau tombolnya belum muncul, buka menu titik tiga di Chrome dan pilih "Instal aplikasi" atau "Tambahkan ke layar utama".
- **iPhone (Safari)**: buka alamatnya di Safari, tekan tombol Bagikan, lalu pilih "Tambah ke Layar Utama". Di iPhone tombol "Pasang di HP" tidak muncul, jadi pakai cara ini.

## Hal yang perlu diketahui

- Daftar pemain dan riwayat match disimpan di HP yang dipakai. HP lain tidak ikut melihatnya.
- Kalau nanti `index.html` diubah, naikkan angka versi di baris pertama `sw.js` (misalnya `rolling-tenis-v1` jadi `rolling-tenis-v2`), supaya HP mengambil versi baru.
- Font Barlow diambil dari Google Fonts saat pertama dibuka dengan internet, lalu disimpan untuk dipakai offline. Tanpa itu, tampilan tetap jalan dengan font bawaan HP.
