### Level 10 - 11

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi di dalam data.txt tetapi di kodekan dengan base64.

Pada level ini masuk ke bandit9 dan password yang di gunakan adalah ``FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey``

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
| base64 | metode encoding (pengkodean) untuk mengubah data menjadi teks ASCII (teks biasa).

---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu untuk mengetahui apakah ada file yang di maksud apakah ada dalam direktori atau tidak, ketikan ini 

> **ls**

lalu akan muncul sebuah berkas dengan  ekstensi ``ASCII`` dari ``data.txt``, lalu jika kita ambil outputnya akan muncul barisan kode beracak.

untuk mengubah dari pengkodean tersebut kita menggunakan sebuah  ``base64`` agar pesan yang di kodekan dapat dipahami oleh manusia. 

> **base64 -d -i data.txt**
base64 [option] [file]
``-d`` : mengembalikan data base64 ke data aslinya ( dekode > aslinya).
``-i`` : mengabaikan karakter yang tidak valid dalam base64, mulai dari spasi aatau lainnnya.

setelah itu akan di dapatkan sebuah kode kata sandi. 

#### Hasil 

pada level ini akan mendapatkan password level 11 
``password Level 11 : dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 10 - 11.jpg">



