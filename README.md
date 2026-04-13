# TUGAS-PROJECT

## 🎬 1. Tema

Penerapan Linked List pada Playlist Video

## 📌 2. Alasan Memilih Tema

Saya memilih tema ini karena:

- Playlist video sering digunakan di platform seperti YouTube
- Mudah dipahami karena semua orang pernah menonton video berurutan
- Cocok untuk menjelaskan konsep Linked List, khususnya Doubly Linked List
- Memiliki fitur:
  - Next (video berikutnya)
  - Previous (video sebelumnya)

## ❓ 3. Rumusan Masalah dan Solusi
### ❓ Rumusan Masalah
1. Bagaimana cara menyimpan data playlist video secara dinamis tanpa batas ukuran tetap?
2. Bagaimana sistem dapat melakukan navigasi ke video berikutnya dan sebelumnya dengan efisien?
3. Bagaimana proses penambahan dan penghapusan video dapat dilakukan tanpa merusak urutan playlist?

### 💡 Solusi

Solusi yang digunakan adalah dengan menerapkan Doubly Linked List, di mana setiap video disimpan dalam node yang memiliki pointer next dan prev.

Dengan pendekatan ini:

- Data dapat ditambahkan dan dihapus dengan mudah
- Navigasi video dapat dilakukan dua arah (next & previous)
- Sistem menjadi lebih fleksibel dibandingkan array

## 📖 4. Studi Kasus

Misalnya pada sebuah playlist video:

Isi playlist:

1. Video A
2. Video B
3. Video C

Ketika pengguna:

- Klik Next → berpindah ke Video B lalu C
- Klik Previous → kembali ke video sebelumnya
- Menambahkan video baru → masuk ke urutan playlist
- Menghapus video → video hilang tanpa merusak urutan

➡ Sistem harus bisa:

- Menyimpan urutan video
- Navigasi maju dan mundur
- Menambah dan menghapus video secara fleksibel

## 5. Landasan Teori

Struktur data adalah cara untuk mengorganisasi dan menyimpan data agar dapat diakses dan dimanipulasi secara efisien. Pemilihan struktur data yang tepat sangat berpengaruh terhadap performa suatu sistem.

Stack dan queue merupakan struktur data linear yang memiliki aturan tertentu dalam pengolahan data. Stack menggunakan prinsip LIFO (Last In First Out), sedangkan queue menggunakan prinsip FIFO (First In First Out). Kedua konsep ini banyak digunakan dalam berbagai sistem, seperti manajemen memori dan antrian proses.

Linked List adalah struktur data yang terdiri dari kumpulan node yang saling terhubung menggunakan pointer. Berbeda dengan array, linked list bersifat dinamis sehingga memudahkan proses penambahan dan penghapusan data.

Dalam implementasinya, linked list dapat digunakan untuk membangun sistem yang membutuhkan fleksibilitas tinggi, seperti playlist video, karena mendukung navigasi dua arah menggunakan Doubly Linked List.

### 📚 Referensi
- Cormen, T. H. (2009). Introduction to Algorithms. MIT Press
- Weiss, M. A. (2014). Data Structures and Algorithm Analysis. Pearson
- Goodrich, M. T. (2013). Data Structures and Algorithms in Python. Wiley

## 6. Desain Sistem dan Implementasi
### 🔄 Alur Sistem

`Input → Proses → Output`

- Input:
Data video (judul video)
- Proses:
  - Menambahkan video ke playlist
  - Navigasi next dan previous
  - Menghapus video
- Output:
Tampilan daftar playlist video

### 🧠 Pseudocode
    Mulai
    Buat playlist kosong

    Tambah Video:
      Jika playlist kosong → jadikan head
      Jika tidak → tambah di akhir

    Next:
      Pindah ke node berikutnya

    Previous:
      Pindah ke node sebelumnya

    Hapus Video:
      Cari video
      Hapus dan sambungkan node

    Tampilkan Playlist
    Selesai

### ⚙️ Implementasi (Linked List)

Menggunakan Doubly Linked List dengan operasi:

- Add Video.
- Next.
- Previous.
- Remove.
- Display.

(Struktur lengkap ada di file `playlist_video.py`)

## 7. Kesimpulan

Berdasarkan hasil implementasi sistem playlist video menggunakan Doubly Linked List, dapat disimpulkan bahwa seluruh rumusan masalah telah berhasil diselesaikan.

Pertama, penyimpanan data playlist dapat dilakukan secara dinamis menggunakan linked list, sehingga tidak memiliki batas ukuran tetap seperti array. Kedua, sistem mampu melakukan navigasi ke video berikutnya dan sebelumnya dengan memanfaatkan pointer `next` dan `prev`, sehingga proses perpindahan menjadi lebih efisien. Ketiga, proses penambahan dan penghapusan video dapat dilakukan tanpa merusak urutan data, karena node dapat langsung disambungkan kembali setelah perubahan.

Selain itu, sistem yang dibuat telah berjalan sesuai dengan teori struktur data linked list, di mana setiap node saling terhubung dan memungkinkan manipulasi data secara fleksibel. Dengan demikian, penggunaan doubly linked list terbukti efektif dan sesuai untuk diterapkan pada sistem playlist video.

### 🚀 Penutup

Implementasi ini menunjukkan bahwa struktur data Linked List sangat cocok digunakan dalam sistem playlist video karena mendukung fleksibilitas dan efisiensi dalam pengelolaan data.
