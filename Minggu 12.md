# Laporan Konfigurasi SMTP Server

### Dosen pengampu: Dr. Ferry Astika Saputra. S.T, M. Sc.
### Kelas : 2 D4 Teknik Informatika A

### 1. Sandy Pradana Putra (3121600017)

### 2. Obed Christian S (3121600022)

### 3. Muhammad Rizqy F (3121600024)

### 4. Daffa Ridwan R (3121600027)

**SMTP** merupakan singkatan dari Simple Mail Transfer Protokol berfungsi sebagai protokol yang memfasilitasi dalam hal transfer <u>e-mail</u>. 

SMTP menggunakan 3 port, Port 25 digunakan untuk non SSL, port 587 untuk TLS dan 465 untuk SSL. Namun oleh sebagian ISP, port 25 telah ditutup karena dianggap berbahaya dengan tidak adanya encryption module yang digunakan.

Berikut cara konfigurasi SMTP Server pada Sistem Operasi Linux:
1. Menginstall package Postfix 




2. Mengisi nama email sistem

Fase ini akan dijalankan secara otomatis sehingga user akan diminta mengisi email system name.



3. Lalu konfigurasi file **main.cf** seperti berikut ini



Setelah melakukan konfigurasi simpan perubahan, lalu restart konfigurasi postfix nya



4. Kemudian tambah CNAME untuk email pada file db-forward



## Membuat Contoh Mail

Semua package telah terinstall selanjutnya konfigurasi pada apache2 nya.





Kemudian tambahkan juga konfigurasi apache 2 di site-availables, 




Terakhir **restart** service apache2 agar bisa menggunakan Web Mail. 
