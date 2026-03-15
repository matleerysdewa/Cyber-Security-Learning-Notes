### Level 1 - 2

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi yang ada pada file bernama ``-`` terletak pada direktori home. 

Pada level ini masuk ke bandit1 dan password yang di gunakan adalah ``ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If``.

---

#### Perintah yang di gunakan
| command | Fungsi |
| ----- | ---- |
| ssh | login jarak jauh pada server/komputer dengan aman melalui jaringan |
| ls | menampilkan isi direktori yang ada di home |
| cat | menggabungkan file dan mencetak output standar.

---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu tampilkan semua file yang ada dalam direktori menggunakan 
> ls

dan akan di tampilkan file ``-`` pada direktori. 

> cat

Pada saat saya ingin mencetak output yang ada di dalam file ``-`` terjadi kesulitan, karena pada dasarnya saat level sebelumnya cukup mengetik seperti ini 
> cat file

nah dari situlah ``man cat`` sangat berfungsi untuk di gunakan, sehingga dapatlah dengan cara mengetik  ini

>cat ./-

kenapa ``./-``, karena komputer tidak bisa membaca ``-`` dan mengira bahwa itu nanti bagian dari gabungan cat itu sendiri ``cat -`` dalam man.

#### Hasil 

pada level ini akan mendapatkan password level 2 
``password Level 2 : 263JGJPfgU6LtdEvgfWU1XP5yac29mFx``

---
#### Dokumentasi 
<img src = "dokumentasi/level 1 - 2.png">


