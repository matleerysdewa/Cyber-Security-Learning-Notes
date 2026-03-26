### Level 8 - 9

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi di dalam data.txt dan kata sandinya hanya muncul 1 kali dari barisn yang berulang.

Pada level ini masuk ke bandit8 dan password yang di gunakan adalah ``dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc``

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
| grep | cetak garis yang sesuai dengan pola atau mencari kata yang ada di sebelah nya |
| uniq | menghapus/memfilter baris yang double atau berduplikat |
| sort | mengurutkan baris teks pada file ataupun kode |

---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu untuk mengetahui apakah ada file yang di maksud apakah ada dalam direktori atau tidak, ketikan ini 

> **ls**

lalu akan muncul sebuah berkas dengan  ekstensi ``ASCII`` dari ``data.txt``, lalu jika kita ambil outputnya akan muncul barisan kode yang beracak.

untuk mengatasi ini maka kita membutuhkan ``sort`` yang berfungsi untuk mengurutkan kode

> **sort data.txt**

maka kita akan melihat urutan file yang banyak, untuk mengatasi agar tidak terduplikat maka kita gunakan ``uniq``.

> **sort data.txt | uniq -u**
``-u`` pada uniq berfungsi untuk menampilkan baris yang muncul hanya sekali saja.
sedangkan ``uniq`` menghapus kata atau file yang berulang.

maka setelah itu akan muncul sebuah password jawabannya.

#### Hasil 

pada level ini akan mendapatkan password level 9 
``password Level 9 : 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM ``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 8 - 9.jpg">



