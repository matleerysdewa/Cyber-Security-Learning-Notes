### Level 4 - 5

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi yang tersembunyi di dalam direktori inhere

Pada level ini masuk ke bandit4 dan password yang di gunakan adalah ``2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ``

---

#### Perintah yang di gunakan
| command | Fungsi |
| ----- | ---- |
| ssh | login jarak jauh pada server/komputer dengan aman melalui jaringan |
| ls | menampilkan isi direktori yang ada di home |
| cat | menggabungkan file dan mencetak output standar.
| cd | ubah direktori kerja  |
| file | menentukan jenis berkas |

---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu tampilkan semua file yang ada dalam direktori menggunakan 

> **ls**

dan akan di tampilkan direktori ``inhere``. Setelah mengetahui itu, pindah direktori kerja dengan mengetik 

> **cd inhere**

lalu, kita telah masuk dalam direktori kerja nya inhere. untuk mengetahui isi nya apa saja kita ketik 

> **ls -a**

di situlah terdapat beberapa file yang kita dapat. Namun, kita hanya ingin mengetahui file mana yang berisi password. Kita akan menggunakan dan mengetik seperti ini

> **file ./***
fungsi ``*`` di gunakan untuk mengetahui semua file atau folder pada direktori.

setelah di ketahui bahwa ada jenis file ASCII text, maka kita cetak outputnya dengan mengetik

> **cat ./-file07**

dan setelah itu kita akan mendapatkan passwordnya.

#### Hasil 

pada level ini akan mendapatkan password level 5 
``password Level 5 : 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw``

---
#### Dokumentasi 
<img src = "dokumentasi/level 4 - 5.png">


