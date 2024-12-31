# 5230411219_Hakiki_Faturrahman_Responsi_pbo

Aplikasi ini adalah sistem manajemen produk dan transaksi berbasis GUI menggunakan Python (dengan pustaka tkinter) dan MySQL sebagai basis data. Aplikasi ini mendukung operasi CRUD (Create, Read, Update, Delete) untuk produk dan transaksi. Pengguna dapat mengelola data produk, menambah transaksi, serta memantau stok produk secara otomatis.

Fitur Produk:
                     -Tambah produk baru
                     -Ubah data produk.
                     -Hapus produk beserta transaksi terkait.

Fitur Transaksi:
                     -Tambah transaksi baru.
                     -Hapus transaksi dan pembaruan stok otomatis.

Cara menjalankan sistem ini:
            1. kita menambahkan produk terlebih dahulu
            2. lalu kita ke bagian menu transaksi, lalu pilih produk yang ingin kita beli
            3. kita masukan produk yang  ingin kita beli
  
Struktur tabel database:

    1. Tabel product memiliki empat kolom:
                  -id (integer, tidak boleh null, merupakan primary key, dan auto-increment).
                  -name (varchar dengan panjang 100 karakter, tidak boleh null).
                  -price (decimal dengan 10 digit, 2 di antaranya adalah angka setelah koma, tidak boleh null).
                  -stock (integer, defaultnya adalah 0).

     2. Tabel transactions memiliki lima kolom:
                 -id (integer, tidak boleh null, merupakan primary key, dan auto-increment).
                 -product_id (integer, bisa null, yang merujuk pada kolom id di tabel products).
                 -quantity (integer, bisa null).
                 -total_price (decimal dengan 10 digit, 2 di antaranya adalah angka setelah koma, bisa null).
                 -transaction_date (date, bisa null).
                 -Tabel transactions juga memiliki foreign key (product_id) yang merujuk pada kolom id di tabel products.


Note : maaf mas refresh nya harus close tampilan gui nya dulu, ketika ingin nambah transaksi dan lihat produk yg dihapus pada bagian transaksi ketika menghapus dari menu produk

