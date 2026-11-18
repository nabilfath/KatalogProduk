# Katalog Produk

## Deskripsi

Katalog Produk merupakan aplikasi desktop berbasis Java yang dibuat untuk mengelola dan menampilkan daftar produk dalam bentuk katalog. Aplikasi ini menggunakan JavaFX sebagai antarmuka pengguna dan SQLite sebagai database untuk menyimpan data produk.

Aplikasi ini memungkinkan pengguna untuk menambahkan, melihat, mengedit, dan menghapus data produk dengan tampilan yang sederhana dan mudah digunakan.

## Fitur Aplikasi

1. Tambah Produk
   Menambahkan produk baru dengan mengisi nama produk, harga, dan memilih foto produk.

2. Tampilkan Produk
   Menampilkan daftar produk dalam bentuk kartu katalog yang berisi foto, nama, harga, dan ID produk.

3. Edit Produk
   Mengubah informasi produk yang sudah tersimpan, seperti nama, harga, dan foto.

4. Hapus Produk
   Menghapus produk dari katalog dengan konfirmasi sebelum penghapusan.

5. Jumlah Produk
   Menampilkan total produk yang tersimpan di dalam katalog.

6. Validasi Data
   Memastikan nama produk tidak kosong dan harga harus berupa angka lebih dari nol.

## Teknologi yang Digunakan

- Java JDK 17
- JavaFX 21
- JavaFX FXML
- SQLite Database
- SQLite JDBC 3.49.1.0
- Apache Maven
- NetBeans IDE

## Struktur Project

```text
KatalogProduk/
│
├── data/
│   └── katalog.db
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── controller/
│   │   │   │   └── KatalogController.java
│   │   │   ├── data/
│   │   │   │   └── ProdukRepository.java
│   │   │   ├── db/
│   │   │   │   └── Database.java
│   │   │   ├── main/
│   │   │   │   └── MainApp.java
│   │   │   └── model/
│   │   │       └── Produk.java
│   │   │
│   │   └── resources/
│   │       ├── image/
│   │       │   ├── kopi.png
│   │       │   ├── roti.png
│   │       │   └── susu.png
│   │       └── view/
│   │           ├── katalog.fxml
│   │           └── styles/
│   │               └── app.css
│   │
│   └── test/
│
├── pom.xml
└── README.md
```

## Cara Menjalankan Aplikasi

1. Pastikan Java JDK 17 atau lebih baru dan Maven sudah terpasang.

2. Clone repository GitHub:

   ```bash
   git clone https://github.com/nabilfath/KatalogProduk.git
   ```

3. Buka folder project menggunakan NetBeans IDE.

4. Tunggu hingga dependency Maven selesai diunduh.

5. Jalankan aplikasi melalui NetBeans atau terminal menggunakan perintah:

   ```bash
   mvn clean javafx:run
   ```

6. Aplikasi Katalog Produk siap digunakan.

## Screenshot Aplikasi

Berikut merupakan tampilan aplikasi Katalog Produk:

screenshot/Screenshot 2026-11-18 112323.png

## Database

Aplikasi menggunakan SQLite sebagai sistem penyimpanan data. Database disimpan dalam folder `data` dengan nama `katalog.db`.

Data produk yang disimpan meliputi:

- ID Produk
- Nama Produk
- Harga Produk
- Nama File Foto Produk

Database akan dibuat secara otomatis apabila belum tersedia ketika aplikasi pertama kali dijalankan.

## Developer

Nama: Nabil Fathurahman

Project: Katalog Produk

**GitHub Repository:** [https://github.com/nabilfath/KatalogProduk](https://github.com/nabilfath/KatalogProduk)
