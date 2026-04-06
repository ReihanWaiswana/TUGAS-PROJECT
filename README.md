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

➡ Jadi, tema ini relevan dengan kehidupan sehari-hari dan mudah dijelaskan

## ❓ 3. Rumusan Masalah dan Solusi
### ❓ Rumusan Masalah
Bagaimana cara menyimpan data playlist video secara dinamis tanpa batas ukuran tetap?
Bagaimana sistem dapat melakukan navigasi ke video berikutnya dan sebelumnya dengan efisien?
Bagaimana proses penambahan dan penghapusan video dapat dilakukan tanpa merusak urutan playlist?

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

- Add Video
- Next
- Previous
- Remove
- Display

(Struktur lengkap ada di file `playlist_video.py`)

## 7. Kesimpulan

Berdasarkan hasil implementasi, rumusan masalah yang diajukan telah berhasil diselesaikan dengan menggunakan Doubly Linked List. Struktur data ini mampu menyimpan data playlist video secara dinamis serta mendukung navigasi dua arah (next dan previous) dengan baik.

Sistem yang dibuat juga telah berjalan sesuai dengan teori struktur data, di mana setiap node saling terhubung menggunakan pointer next dan prev. Proses penambahan dan penghapusan video dapat dilakukan tanpa mengganggu urutan data, sehingga lebih efisien dibandingkan penggunaan array.

Dengan demikian, penggunaan linked list pada sistem playlist video memberikan manfaat berupa fleksibilitas dalam pengelolaan data serta kemudahan dalam navigasi, sehingga cocok digunakan untuk kasus serupa dalam pengembangan aplikasi nyata.

### 🚀 Penutup

Implementasi ini menunjukkan bahwa struktur data Linked List sangat cocok digunakan dalam sistem playlist video karena mendukung fleksibilitas dan efisiensi dalam pengelolaan data.
