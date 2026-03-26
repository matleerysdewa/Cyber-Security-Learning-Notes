### Level 11 - 12

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi di dalam data.txt, dimana semua huruf kecil dan huruf besar telah di putar sebanyak 13 kali.

Pada level ini masuk ke bandit11 dan password yang di gunakan adalah ``dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr``

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

---

#### Prosesnya

langkah pertama adalah dengan masuk ke hostnya menggunakan ``ssh``

lalu untuk mengetahui apakah ada file yang di maksud apakah ada dalam direktori atau tidak, ketikan ini 

> **ls**

lalu akan muncul sebuah berkas dengan  ekstensi ``ASCII`` dari ``data.txt``, lalu jika kita ambil outputnya dengan ``cat`` akan di tampilkan barisan yang acak.

karena tadi di soal telah di beritahu bahwa di acak/ di putar sebanyak 13x, maka kita ketik seperti ini

> **cat  data.txt | tr 'a-zA-Z'  'n-za-mN-ZA-M'**
kita ambil data.txt lalu putar kembali 13x
`a-zA-Z` : mewakili huruf besar dan huruf kecil
`n-za-mN-ZA-M` : Ini menggeser setiap huruf ke depan sebanyak 13 tempat dalam alfabet

maka kita akan mendapatkan passwordnya.

#### Hasil 

pada level ini akan mendapatkan password level 12 
``password Level 12 : 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 11 - 12.jpg">



