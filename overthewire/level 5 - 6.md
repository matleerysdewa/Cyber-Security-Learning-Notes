### Level 5 - 6

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi yang tersembunyi di dalam direktori inhere, dan memiliki kriteria seperti 
- size 1033 bytes
- human-reaeble
- not executable

Pada level ini masuk ke bandit5 dan password yang di gunakan adalah ``4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw``

---

#### Perintah yang di gunakan
| command | Fungsi |
| ----- | ---- |
| ssh | login jarak jauh pada server/komputer dengan aman melalui jaringan |
| ls | menampilkan isi direktori yang ada di home |
| cat | menggabungkan file dan mencetak output standar.
| cd | ubah direktori kerja  |
| file | menentukan jenis berkas |
| find | mencari file dalam hierarki direktori |

---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu tampilkan semua file yang ada dalam direktori menggunakan 

> **ls**

dan akan di tampilkan direktori ``inhere``. Setelah mengetahui itu, pindah direktori kerja dengan mengetik 

> **cd inhere**

lalu, kita telah masuk dalam direktori kerja nya inhere. untuk mengetahui isi nya apa saja kita ketik 

> **ls -a**

Disini akan di tampilkan beberapa direktori dan ga mungkin buka direktorinya satu-satu, maka dari itu kita menggunakan ``find``

> **find . -type f -size 1033c ! -executable**

``.`` berarti direktori saat ini

``-type f`` berarti bertipe file

``-size 1033c`` berarti yang berukuran 1033 bytes

``! -executable`` berarti yang tidak dapat di eksekusi

maka kita akan mendapatkan sebuah file yang berisi sesuai apa yang kita cari, lalu ambil outputnya 

>**cat ./maybehere07/.file2**

dan kita akan mendapatkan passwordnya.


#### Hasil 

pada level ini akan mendapatkan password level 6 
``password Level 6 : HWasnPhtq9AVKe0dmk45nxy20cvUa6EG``

---
#### Dokumentasi 
<img src = "dokumentasi/level 4 - 5.png">


