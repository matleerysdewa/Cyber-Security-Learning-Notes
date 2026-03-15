### Level 2 - 3

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi yang ada pada file bernama ``--spaces in this filename--`` terletak pada direktori home. 

Pada level ini masuk ke bandit1 dan password yang di gunakan adalah ``263JGJPfgU6LtdEvgfWU1XP5yac29mFx``

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

dan akan di tampilkan file ``--spaces in this filename--`` pada direktori. 

> cat

Pada saat ingin mencetak tidak bisa, karena file memiliki karakter khusus berupa spasi, maka itu saya ingin melihat lebih jelas menggunakan perintah ini.

> ls -b
menampilkan nama file yang lebih jelas/karakter aneh.

lalu setelah di ketahui karakter aslinya adalah ``--spaces\ in\ this\ filename--``

kita tampilkan outputnya dengan mengetik

> cat spaces\ in\ this\ filename

atau

> cat "--spaces in this file name--"

di karenakan dari kedua tersebut saya belum bisa dan menampilkan error, maka saya menggunakan/ mengetik seperti ini

> cat ./--spaces\ in\ this\ filename--

dan akhirnya muncul juga jawabannya.

#### Hasil 

pada level ini akan mendapatkan password level 3 
``password Level 3 : MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx``

---
#### Dokumentasi 
<img src = "dokumentasi/level 2 - 3.png">


