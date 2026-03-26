### Level 7 - 8

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi di dalam data.txt lalu kata sandinya beraada di sebelah kata millionth.

Pada level ini masuk ke bandit7 dan password yang di gunakan adalah ``morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj``

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

---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu untuk mengetahui apakah ada file yang di maksud apakah ada dalam direktori atau tidak, ketikan ini 

> **ls -a**

lalu akan muncul sebuah berkas dengan  ekstensi ``unicode text`` dari ``data.txt``, lalu kita ambil dengan ``cat``.

> **cat data.txt**

maka akan tampil barisan code dan tentunya akan pusing, sehingga dibutuhkan ``grep`` untuk lebih cepat, karena akan mencari kata sandinya dekat kata ``millionth``

> **cat data.txt | grep millionth**
***cara bacanya*** : Tampilkan isi data.txt, LALU kirim hasilnya ke grep untuk disaring yang mengandung kata millionth

maka akan muncul sebuah kata sandi.


#### Hasil 

pada level ini akan mendapatkan password level 8 
``password Level 8 : dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 7 - 8.png">



