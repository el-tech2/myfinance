# MyFinance

Aplikasi pencatatan keuangan pribadi berbasis HTML, CSS, dan JavaScript.

## Menjalankan di VS Code
1. Ekstrak `MyFinance.zip`.
2. Buka folder `MyFinance` melalui Visual Studio Code.
3. Jalankan `index.html` menggunakan ekstensi Live Server (klik kanan > Open with Live Server), atau buka langsung di browser.
4. Saat pertama kali dibuka, buat password pribadi.

## Fitur
- Login satu pengguna (password dibuat saat pertama kali).
- Dashboard pemasukan, pengeluaran, sisa dana, dan saldo rekening.
- Rekening: BRI, SeaBank, GoPay, DANA, Cash.
- Tambah pemasukan, pengeluaran, dan transfer antar rekening.
- Kategori pengeluaran sesuai kebutuhan.
- Periode bergulir 30 hari, dimulai dari tanggal pemasukan pertama.
- Riwayat transaksi, laporan kategori dan sumber dana.
- Backup dan restore data JSON.
- Tampilan responsif untuk desktop dan ponsel.

## Catatan penting
Data disimpan di `localStorage` browser pada perangkat yang digunakan. Login ini adalah pengunci sederhana di sisi browser, bukan autentikasi server yang aman. Jangan gunakan untuk menyimpan kredensial bank atau informasi rahasia. Data tidak otomatis tersinkron antarperangkat/browser. Lakukan backup secara berkala.

Saldo awal semua rekening dimulai dari Rp0. Untuk memulai, catat saldo/pemasukan awal ke rekening yang sesuai. Transfer antar-rekening tidak dihitung sebagai pengeluaran.

Periode 30 hari: pemasukan pertama menjadi tanggal awal periode pertama. Periode berikutnya dimulai tepat 30 hari setelah awal periode sebelumnya. Pengeluaran periode berjalan ditampilkan pada dashboard; saldo akun dihitung terus dari seluruh transaksi.

## Revisi logo dan cetak PDF
- Logo BRI, SeaBank, GoPay, DANA, dan Cash menggunakan file gambar yang diberikan.
- Logo ditampilkan pada dashboard dan halaman Rekening & Dompet.
- Pada halaman Transaksi tersedia tombol Cetak / PDF.
- Tombol cetak membuka tampilan laporan bergaya struk dengan ringkasan dan tabel transaksi, termasuk pemasukan, pengeluaran, serta transfer.
- Di dialog print browser pilih printer "Save as PDF" untuk menyimpan PDF.
- Ukuran kertas A4 dengan margin atas 3 cm, kanan 4 cm, bawah 4 cm, kiri 4 cm.

## Revisi tampilan mobile dan tablet
- Desktop: sidebar navigasi tetap di sisi kiri.
- Tablet: sidebar dipadatkan menjadi ikon agar ruang konten lebih luas.
- Smartphone: sidebar diganti bottom navigation dengan menu Dashboard, Transaksi, Rekening, dan Laporan.
- Form transaksi menyesuaikan layar ponsel dan tombol dibuat lebih mudah disentuh.
- Konten dashboard, kartu saldo, filter, dan laporan menyesuaikan lebar layar.
