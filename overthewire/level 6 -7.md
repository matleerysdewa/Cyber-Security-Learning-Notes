### Level 6 - 7

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi yang yang berada di suatu tempat server dan memiliki properti seperti ini :
- size 33 bytes
- dimiliki oleh user bandit7
- dimiliki oleh grup bandit6

Pada level ini masuk ke bandit6 dan password yang di gunakan adalah ``HWasnPhtq9AVKe0dmk45nxy20cvUa6EG``

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

lalu untuk mengetahui apakah ada file yang di maksud apakah ada dalam direktori atau tidak, ketikan ini 

> **ls -a**

di karenakan tidak ada, maka kita mencari dengan menggunakan ``find``, ketik dalam terminal seperti ini 

> **find / -size 33c -user bandit7 -group bandit6**

maka, akan ditampilkan sederet file yang banyak, namun karena premssion denied dan tidak ingin membuang waktu, maka kita ketikan seperti ini 

> **find / -size 33c -user bandit7 -group bandit6 -exec file {} \; 2>/dev/null**

``-exec file {}`` sebagai Temukan semua file, lalu untuk setiap file yang ditemukan — jalankan perintah file pada file tersebut.

``find          → "Cari semua file di direktori ini"``

``-exec         → "Untuk setiap file yang ditemukan, lakukan..."``

``file          → "...jalankan perintah FILE (pendeteksi tipe)"``

``{}            → "...pada FILE INI (nama filenya diisi otomatis)"``

``\;            → "Selesai, lanjut ke file berikutnya"``

``2>/dev/null`` memiliki arti Semua pesan error, buang saja — jangan tampilkan ke layar.

lalu akan di ketahui filenya, dan di sini jenis filenya ASCII text. Dan kita atau menampilkan output file tersebut dengan menggunakan ``cat``

> **Cat /var/lib/dpkg/info/bandit7.password**

dan kita mendapatkan passwordnya.

#### Hasil 

pada level ini akan mendapatkan password level 7 
``password Level 7 : morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 6 - 7a.png">
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 6 - 7b.png">


