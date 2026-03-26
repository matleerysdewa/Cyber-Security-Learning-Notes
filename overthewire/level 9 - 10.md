### Level 9 - 10

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi di dalam data.txt, dengan di awali karakter =, serta bisa di baca oleh manusia.

Pada level ini masuk ke bandit9 dan password yang di gunakan adalah ``4CKMh1JI91bUIZZPXDqGanal4xvAg0JM``

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
| strings | menampilkan teks yang bisa dibaca manusia |

---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu untuk mengetahui apakah ada file yang di maksud apakah ada dalam direktori atau tidak, ketikan ini 

> **ls**

lalu akan muncul sebuah berkas dengan  ekstensi ``DATA`` dari ``data.txt``, lalu jika kita ambil outputnya akan muncul barisan kode yang tidak dapat di baca oleh manusia.

untuk mengatasi ini maka kita membutuhkan ``Strings`` yang berfungsi untuk menampilkan teks yang dapat di baca oleh manusia.

> **stirngs data.txt**

maka kita dapat melihat teks yang dapat dibaca oleh manusia, namun kata sandi tersebut memiliki kata kunci/ karakter ``=``.

kita akan mencarinya dengan  menggunakan ``grep``

> **strings data.txt | grep =**
dibaca : cari strings pada data.txt, lalu jika sudah ketemu maka carilah karakter =.

maka akan muncul sebuah barisan teks dan salah satunya adalah password.

#### Hasil 

pada level ini akan mendapatkan password level 10 
``password Level 10 : FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 9 - 10.jpg">



