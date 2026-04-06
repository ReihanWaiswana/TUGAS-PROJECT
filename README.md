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

## 📖 3. Studi Kasus

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

## ❓ 4. Rumusan Masalah dan Solusi
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
