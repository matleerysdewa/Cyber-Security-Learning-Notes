### Level 3 - 4

---
### Tujuan Level

Tujuan level ini adalah menemukan kata sandi yang tersembunyi di dalam direktori inhere

Pada level ini masuk ke bandit3 dan password yang di gunakan adalah ``MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx``

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
> ls

dan akan di tampilkan direktori ``inhere``. Setelah mengetahui itu, pindah direktori kerja dengan mengetik 

> cd inhere

lalu, kita telah masuk dalam direktori kerja nya inhere. untuk mengetahui isi nya apa saja kita ketik 

> ls -a

di situlah terdapat beberapa direktori dan file yang tersembunyi, untuk mengetahui itu direktori atau file dengan mengetik 

> file (nama file)

di situ akan muncul jenis berkas yang di gunakan. lalu, kita output file tersebut dengan ketik

> cat ...Hidding-From-you

maka muncullah passwordnya.

#### Hasil 

pada level ini akan mendapatkan password level 4 
``password Level 4 : 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ``

---
#### Dokumentasi 
<img src = "dokumentasi/level 3 - 4.png">


