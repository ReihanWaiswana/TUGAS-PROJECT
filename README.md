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

## ❓ 4. Rumusan Masalah
1. Bagaimana menyimpan data playlist video secara dinamis?
2. Bagaimana pengguna bisa berpindah ke video berikutnya dan sebelumnya?
3. Bagaimana cara menambah dan menghapus video tanpa mengganggu urutan?
4. Struktur data apa yang paling sesuai untuk sistem playlist video?

### Pembahasan Rumusan Masalah
1. Penyimpanan Data Playlist
   
   Data playlist disimpan menggunakan Linked List, di mana setiap video adalah node yang memiliki next dan prev.
   ➡ Memungkinkan data disimpan secara dinamis tanpa batas tetap
2. Navigasi Video (Next & Previous)
   
   Navigasi dilakukan dengan:

   - next → ke video berikutnya
   - prev → ke video sebelumnya

   ➡ Perpindahan menjadi cepat tanpa harus mencari dari awal

3. Penambahan dan Penghapusan Video

   Tambah → node baru ditambahkan ke akhir playlist
   Hapus → node dihapus lalu node lain langsung disambungkan

   ➡ Tidak perlu menggeser data, sehingga lebih efisien

4. Struktur Data yang Digunakan

   Menggunakan Doubly Linked List karena:

   Bisa maju dan mundur
   Mudah tambah dan hapus data

   ➡ Paling cocok untuk sistem playlist video
