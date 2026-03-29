### Level 14 - 15

---
### Tujuan Level

Tujuan level ini adalah mengirimkan kata sandi saat ini ke localhost port 30000.

Pada level ini masuk ke bandit14 dan password yang di gunakan adalah ``-``

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
| nc | mentransfer data dari satu host ke host lain dengan membuat model klien/server dasar |


---

#### Prosesnya

Setelah tadi masuk menggunakan `ssh -i`, maka kita mencari password level 14 ini dengan cara melihat soal teka-teki sebelumnya yang di sebutkan di `/etc/bandit_pass/bandit14 dan hanya dapat dibaca oleh pengguna bandit14`.

maka kita ketikan saja langsung dengan cara ini

> **cat /etc/bandit_pass/bandit14 | nc localhost 30000**
`|` di baca *lalu*
cara baca keseluruhan : ambil yang ada di /etc/bandit_pass/bandit14, lalu kirimkan ke localhost port 30000.

maka setelah itu akan muncul password level 15.

#### Hasil 

pada level ini akan mendapatkan password level 15 
``password Level 15 : 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo``

---
#### Dokumentasi 
<img src = "E:\Cyber-Security-Learning-Notes\overthewire\dokumentasi\level 14 - 15.png">



