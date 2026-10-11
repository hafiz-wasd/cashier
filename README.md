# Kasir Restoran

Aplikasi kasir web (HTML + CSS + JavaScript murni, tanpa instalasi).

## Cara menjalankan
Buka `index.html` di browser. Selesai.

## Struktur
- `index.html` : kerangka halaman
- `style.css`  : tampilan tema Jawa modern (motif awan dan foto wayang kulit `img/wayang.jpg` di folder `img/`) dan cetak struk
- `jspdf.umd.min.js` : library pembuat PDF struk (lokal, tanpa internet)
- `app.js`     : logika meja, pesanan, pembayaran, struk, kelola menu

## Mengubah isi
- Menu awal: array `defMenu` di `app.js`
- Jumlah meja: `nTables` di `app.js` (default 12)
- Nama restoran di struk: cari teks `RESTORAN` di `app.js`
- Warna: variabel CSS di bagian atas `style.css`

Data tersimpan di localStorage browser (per perangkat).

## Diskon
Menu **Kelola Diskon** (pojok atas) untuk membuat kode: jenis persen/nominal, nilai, minimal belanja, maksimal potongan, dan tanggal berlaku. Contoh awal: `HEMAT10`, `PROMO5K`. Kasir memakai kode di halaman pembayaran.

## Dashboard
Tombol **Dashboard**: ubah nama restoran dan alamat/telepon (tampil di struk), lihat pendapatan, jumlah transaksi, total diskon, menu terlaris hari ini, dan transaksi terakhir.

## Foto profil restoran
Di **Dashboard → Pengaturan restoran**, unggah foto/logo (JPG/PNG, maks. 8 MB). Foto tampil sebagai logo di pojok kiri atas halaman, dan di pojok kiri atas struk dalam warna hitam putih (layar, cetak, dan PDF). Tombol **Hapus foto** mengembalikan ke huruf awal nama restoran.
