# Apa Itu Jaringan 
---
- **Room Link :** [What Is Networking](https://tryhackme.com/room/whatisnetworking)
- **Ctegory :** [Network Fundamental](https://tryhackme.com/module/network-fundamentals)
- **Difficulty :** Easy

---

## Overview

Room ini membahas mengenai fundamental jaringan yaitu mengenai apa itu Jaringan, Internet, cara berkomunikasi, dan cara menguji konektivitas (Ping).

---

### Networking
```Jaringan``` adalah kumpulan perangkat yang saling terhubung baik untuk berbagi informasi atau lainnya.
Jaringan dapat di temui di mana-mana, mulai dari kehidupan sosial, rumah,  digital, dan sebagainya.

> ###### Analogi
> Ana memiliki teman bernama Bob dan Sandi, karena mereka memiliki kesamaan dalam berbicara bahasa daerah sehingga mereka saling berkomunikasi dan koneksi.

---

### Internet

```Internet``` adalah Jaringan raksasa yang terjadi dari kumpulan jaringan kecil.

<p align="left">
  <img src="../../Asset/internet2.png" alt="Internet" width="400" alt="internet2">
</p>

| Nama | Jenis |
|-----|----------|
|**Bob, Sandi ,Dian ,May**| **Network #n**|
| Ana | Internet |

> ###### *Analogi*
> Ana memiliki teman bernama Bob dan Sandi dari tempat tinggal yang sama, lalu si Ana juga memiliki teman bernama May dan Dian, mereka berdua berasal dari luar kota. Karena si Ana ingin memperkenalkan mereka ke Bob dan Sandi, Ana harus menerjemahkan atau meneruskan pesan ( percakapan ) dari si May dan Dian, sehingga dari situlah terjadinya dan mereka dapat berkomunikasi dengan baik.


`Internet disebut juga Jaringan Publik`

---

### Identifying Devices On Network

untuk mengetahui dan di kenali jaringan pada perangkat, maka di butuhkan identitas berupa **IP** dan **MAC**. 

#### IP
Internet Protocol ibaratkan seperti `Alamat Rumah`.
| Versi | Format | Kapasitas | Contoh |
|-------|--------|-----------|--------|
|IPv4| 4-oktet, 32bit| 4,3 Miliar| 192.168.1.1|
|IPv6| 8 klmp Heksadimal, 64 Bit| ~ | 2001:0db8:85a3:0000:0000:8a2e:0370:7334 |

> Analogi 
>IPv4 adalah perumahaan yang terbatas stoknya. 
>IPv6 adlah perumahan yang luas dan tidak hampir tidak terbatas.

#### MAC
Media Acces Control ibaratkan seperti `Nomor Seri Rumah` yang sudah ditentukan oleh arsitek (pabrik).

| Fungsi | perangkat bisa di kenali oleh jaringan dan mengirim ke tujuan |
|--------|----------|
| Contoh | 00:1A:2B:3C:4D:5E |
| Karakter | Heksadimal 12 karakter, : tanda pemisah |
| Kelemahan | perangkat dapat di palsukan dengan **Spoofing**, alamat MAC di gunakan pihak ketiga |


---

### Ping
cara mengecek suatu perangkat di jaringan apakah bisa dihubungi dan kecepatannya.

Menggunakan **ICMP (Internet Control Message Protocol)** untuk menentukan kinerja koneksi.

<p align="center">
  <img src="../../Asset/ping.png" alt="ping" width="400">  
</p>







