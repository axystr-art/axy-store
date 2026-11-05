# AXY STORE — Premium Blue & Gold

Website katalog toko dengan panel admin dan penyimpanan online Netlify Blobs.

## Penting sebelum deploy
Website ini membutuhkan Netlify Functions + Netlify Blobs. Jangan deploy hanya file `index.html` jika ingin produk tersinkron ke semua pengunjung.

## Cara menyiapkan
1. Buat repository GitHub dan upload seluruh isi folder ZIP ini.
2. Di Netlify pilih **Add new site → Import an existing project**, lalu hubungkan repository.
3. Setelah deploy, buka **Site configuration → Environment variables** dan tambahkan:
   - `ADMIN_PASSWORD` = password admin pilihanmu
   - `ADMIN_TOKEN` = token rahasia panjang yang kamu buat (jangan bagikan ke siapa pun)
4. Trigger deploy ulang setelah menambahkan environment variables.
5. Buka alamat website. Tekan **ADMIN PANEL**, masukkan `ADMIN_PASSWORD`.
6. Produk yang disimpan akan disimpan di Netlify Blobs dan tampil untuk semua pengunjung.

## Pengaturan WhatsApp
Di `index.html`, cari `6281234567890` lalu ganti dengan nomor WhatsApp toko dalam format internasional tanpa tanda `+`.

## Catatan
- Maksimal foto 900 KB per produk pada starter ini.
- Starter ini mendukung tambah, edit, dan hapus produk.
- Jangan membagikan `ADMIN_PASSWORD` atau `ADMIN_TOKEN`.
- Netlify Blobs adalah penyimpanan online yang disediakan Netlify; tidak perlu membuat project Firebase.
