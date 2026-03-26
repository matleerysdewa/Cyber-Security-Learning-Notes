### Level 11 - 12

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi di dalam data.txt, file ini berisi hexadump dan di kompres berkali-kali. Buatkan juga direktori dibawah /tmp tempat anada bekerja. Bisa menggunakan `mkdir` atau `mktemp -d` saling menggunakan `cp` dan ganti namanya menggunakan `mv`.

Pada level ini masuk ke bandit12 dan password yang di gunakan adalah ``7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4``

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
| base64 | metode encoding (pengkodean) untuk mengubah data menjadi teks ASCII (teks biasa). |
| tr | menerjemahkan / menukar setiap huruf dari himpunan 1 dengan huruf yg sesuai di himpunan 2 | 
| xxd | membuat hexdump ataupun sebaliknya |
| cp | mencopy file |
| mv | memindahkan ( menggnti nama ) file |


---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu untuk mengetahui apakah ada file yang di maksud apakah ada dalam direktori atau tidak, ketikan ini 

> **ls**

lalu akan muncul `data.txt` dan ketika saya `cat` menampilkan hexadump, oleh karena itu, kita akan mengubah menjadi binary.

saya membuat direktori terlebih dahulu seperti apa yang di perintahkan dalam teka-teki.

> **mkdir /tmp/matlee**
ketika sudah membutat langsung saja masuk ke direktorinya dengan `cd`.

lalu copy file data.txt yg ada di home ke tmp/matlee, dengan menggunakan perintah `cp`

> **cp ~/data.txt /tmp/matlee**
maksud dari `~` adalah home direktorinya.

setelah muncul di direktori saat ini, kita ubah menjadi binary dengan mengetik 

> **xxd -r data.txt > data**
`-r` berarti kembalikan dari hexadump ke binary atau sebaliknya.
`>` menjadi ...

setelah itu kita `ls` dan akan muncul 2 nama data, gunakan yang data tadi, lalu ketahui jenis file nya apa dengan `file data`.

> **gzip : mv data data.gz && gzip -d data.gz**
**bzip2 : mv data data.bz2 && bzip2 -d data.bz2**
**POSIX TAR : mv data data.tar && tar -xvf data.tar**
`-x , --extract , --get`
      mengekstrak file dari arsip
`-v , --verbose` 
      menampilkan daftar file yang diproses secara detail
`-f , --file  ARCHIVE`
      gunakan file arsip atau perangkat ARCHIVE

sampailah muncul data8 dan ambil dengan     `cat`  muncul passwordnya.
#### Hasil 

pada level ini akan mendapatkan password level 13 
``password Level 13 : FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\bandit 12 - 13.jpg">



