### Level 13 - 14

---
### Tujuan Level

Tujuan level ini adalah Anda tidak mendapatkan kata sandi berikutnya, tetapi Anda mendapatkan kunci SSH pribadi yang dapat digunakan untuk masuk ke level berikutnya. 

Pada level ini masuk ke bandit13 dan password yang di gunakan adalah ``FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn``

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
| scp | salinan aman (program penyalinan file jarak jauh) |
| chmod | mengatur atau mengubah hak akses (permissions) dari sebuah file atau direktori |


---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu untuk mengetahui apakah ada file yang di maksud apakah ada dalam direktori atau tidak, ketikan ini 

> **ls**

lalu akan ada dua file yaitu `HINT` dan `sshkey.private`. karena `sshkey.private` adalah kunci untuk masuk di bandit14, maka kita harus mendownload atau menyalin dari server ke home kita menggunakan `scp`

>**scp -P 2220 bandit13@bandit.labs.overthewire.org:~/sshkey.private ~/**
`~/` adalah tujuan mau di taruh di mana file sshkey.private

setelah itu, karena belum di berikan izin, mka kita gunakan `chmod`

>**chmod 600 sshkey.private**

masuk ke bandit14 dengan cara ini

>**ssh -i ~/sshkey.private bandit14@bandit.labs.overthewire.org -p 2220**
`-i  file identitas`
        Memilih berkas tempat identitas (kunci privat) untuk otentikasi kunci publik dibaca.

maka kita bisa login ke bandit14.

#### Hasil 

pada level ini akan mendapatkan password level 14 
``password Level 14 : -``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 13 -14.png">



