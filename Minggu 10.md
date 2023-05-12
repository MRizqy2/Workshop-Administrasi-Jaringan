# Laporan Install Web Server di Linux

### Dosen pengampu: Dr. Ferry Astika Saputra. S.T, M. Sc.
### Kelas : 2 D4 Teknik Informatika A

### 1. Sandy Pradana Putra (3121600017)

### 2. Obed Christian S (3121600022)

### 3. Muhammad Rizqy F (3121600024)

### 4. Daffa Ridwan R (3121600027)

# Install Web Server di Linux

Berikut langkah - langkah untuk menginstall web server: 

1. pastikan dns server menggunakan dns server yang sudah  disediakan dan juga pastikan gateway sesuai dengan router
[![Whats-App-Image-2023-05-12-at-19-17-15.jpg](https://i.postimg.cc/SNwJNVmc/Whats-App-Image-2023-05-12-at-19-17-15.jpg)](https://postimg.cc/MvmW97MG)

2. Cek apakah jaringan sudah benar
[![Whats-App-Image-2023-05-12-at-19-18-12.jpg](https://i.postimg.cc/2ySBh5tv/Whats-App-Image-2023-05-12-at-19-18-12.jpg)](https://postimg.cc/CB91VwSL)
 
3. Kemudian dilanjutkan dengan menginstall **Nginx**, **MariaDB**, **Php**.
[![Whats-App-Image-2023-05-12-at-20-29-36.jpg](https://i.postimg.cc/vm40cQFD/Whats-App-Image-2023-05-12-at-20-29-36.jpg)](https://postimg.cc/1gZGd1zZ)

4. Setelah itu menginstall package utility yang digunakan untuk menginstall composer nantinya.

[![Whats-App-Image-2023-05-12-at-19-22-49.jpg](https://i.postimg.cc/851Fg5N3/Whats-App-Image-2023-05-12-at-19-22-49.jpg)](https://postimg.cc/HJhWQTJ4)

5. Download **composer.phar**, lalu pindah ke folder usr/bin agar bisa diakses sebagai program linux

[![Whats-App-Image-2023-05-12-at-19-29-26.jpg](https://i.postimg.cc/90sF0FHc/Whats-App-Image-2023-05-12-at-19-29-26.jpg)](https://postimg.cc/GTJ1SRpf)

6. Cek hasilnya dengan melihat version dari **composer**

[![Whats-App-Image-2023-05-12-at-19-29-50.jpg](https://i.postimg.cc/XYSY0Jg8/Whats-App-Image-2023-05-12-at-19-29-50.jpg)](https://postimg.cc/nC2J4ngj)

### Mencoba menginstall contoh projek laravel(php) dan dijalankan menggunakan Server

**Pertama**, clone dari github terlebih dahulu.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/p240y43qmk6i1vxcmw5f.png)
 
**Kedua** lakukan install package menggunakan composer

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/d2oi33urt57piry4wexf.png)

**Ketiga** Tambahkan konfigurasi project pada **Nginx**

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fs5i0hquroi1ohhbjuo5.png)

**Keempat** Setelah melakukan konfigurasi restart **service** nginx.


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rpg8yl9ft7n1vk032zoh.png)

**Kelima** melakukan instalasi RDBMS (Relational Database Management Software) PhpMyAdmin di server

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/60lvfwoo010dlj3cx7y3.png)

Setelah itu dapat kita lihat pada phpmyadmin susunan table pada database seperti berikut ini:

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ipgnqdzsql1rx52q0nvv.png)

Langkah **Terakhir** adalah dengan menginstall **_FTP_**

FTP merupakan protokol yang bisa menyimpan file pada server. Untuk menginstall nya cukup via apt lalu nama package nya _proftpd_. Seperti pada gambar berikut ini:

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/w0xqhgf54njyteahyfc8.png)

Setelah terpasang check service dari ftp apakah berjalan dengan baik, dengan menggunakan command **systemctl**

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ld0op0ut67q3cvcvyt2s.png)

Jika berjalan dengan baik maka akan seperti gambar diatas. Jalankan ftp mengkoneksikannya dengan localhost


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/qo9r5eibizfn5qtocfh4.png)

Hasil akhirnya akan menampilkan halaman website seperti ini

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/wtrigt7rmu08vwlhdvyr.png)
