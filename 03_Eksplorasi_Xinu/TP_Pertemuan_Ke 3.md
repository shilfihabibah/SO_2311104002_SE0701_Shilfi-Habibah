# <h1 align="center">Laporan Praktikum Modul 3  <br> Eksplorasi Xinu </h1>
<p align="center">SHILFI HABIBAH - 2311104002</p>

## A. Dasar Teori

### a. Command line interface (CLI)
Tampilan berbasis teks yang memungkinkan pengguna berkomunikasi langsung dengan sistem operasi melalui perintah yang diketik menggunakan keyboard. Biasanya digunakan melalui terminal, command prompt, atau shell, dan hingga kini masih menjadi alat utama untuk banyak administrator sistem, developer, dan pengguna tingkat lanjut.
### b. Shell
Merupakan komponen krusial yang berfungsi sebagai perantara antara pengguna dan kernel dari sistem operasi. Ia bertindak sebagai pengurai dan penafsir perintah yang biasanya dimasukkan melalui terminal, mengubah instruksi tekstual menjadi tindakan eksekusi oleh sistem.
### c. Struktur Direktori pada Sistem Operasi
Direktori root yaitu akar dari semua direktori dan file di sistem Linux. Semua direktori lain berada di bawah direktori ini. Perintah seperti cd digunakan untuk berpindah dari satu direktori ke direktori lain.
### d. Proses Kompilasi Program
Proses menerjemahkan kode sumber yang ditulis oleh seorang programmer menjadi kode mesin yang dapat dieksekusi oleh komputer. Penerjemahan ini dilakukan oleh program khusus yang disebut kompiler.
### e. Proses Booting Sistem Operasi
Proses menyalakan komputer dan memuat sistem operasi ke dalam memori utama (RAM) sehingga komputer siap digunakan. Istilah “booting” berasal dari kata bootstrap, yang bermakna memulai sesuatu dari awal.

## B. Guided

Langkah - langkah : 
1. Buka VirtualBox dan start development-system.ova 
2. Login pada development-system vm menggunakan password (xinurocks)
3. setelah berhasil login muncul terminal seperti di gambar ![Terminal development-system](image/Terminal_development-system.jpeg) 
4. ketik "cd xinu/compile" pada terminal untuk pindah ke directory xinu dan enter untuk menjalankan perintah. Fungsi nya untuk pindah direktori ke xinu, tampilan seperti gambar berikut : ![pindah ke directory xinu](image/pindah_ke_directory_xinu.jpeg)
5. ketik "make clean" pada terminal untuk menghapus file kompilasi sebelumnya, tampilan seperti gambar berikut : ![make clean](image/make_clean.jpeg)
6. ketik "make" pada terminal untuk melakukan proses kompilasi source code jadi file yang bisa dijalankan sistem, tampilan seperti gambar berikut : ![make](image/make.jpeg)
7. ketik "sudo minicom" untuk menjalankan aplikasi minicom sebagai alat komunikasi melalui serial port sehingga kita bisa interaksi dengan sistem xinu yang berjalan pada backend vm, ketika sudah dienter akan diarahkan ke isi password yaitu kita isi xinurocks. Tampilan seperti gambar berikut : ![sudo minicom](image/sudo_minicom.jpeg)
8. setelah itu jalankan backend di virtualbox 
9. ketik perintah "help" di terminal untuk menampilkan semua perintah xinu, tampilan seperti gambar berikut : ![help](image/help.jpeg)

## C. Unguided

1. Berapa jumlah perintah pada Xinu?
jawab : 23 perintah (dapat di lihat menggunakan perintah help pada shell xinu) 
2. Sebutkan 2 perintah yang mempunyai fungsi yang sama! 
jawab : perintah help dan ?, keduanya digunakan untuk menampilkan bantuan atau daftar perintah pada xinu
3. Berapa IP address Xinu?
jawab : 10.0.3.15 (dapat dilihat mengggunakan perintah netinfo pada shell xinu)
4. Perintah apa yang digunakan untuk mengetahui IP address? 
jawab : netinfo
5. Berapa IP DNS server yang digunakan oleh Xinu? 
jawab : 192.168.18.1 (dapat dilihat mengggunakan perintah netinfo pada shell xinu)
6. Terdapat berapa proses yang sedang berjalan pada Xinu? 
jawab : 7 (dapat dilihat menggunakan perintah ps pada shell xinu)
7. Proses apa yang mempunyai prioritas paling rendah? 
jawab : prnull
8. Proses apa yang mempunyai ukuran paling besar? 
jawab : Main process dengan Stack Size 65536
9. Proses apa yang berada dalam state current? 
jawab : ps
10. Proses apa yang berada dalam state suspend? 
jawab : Pada hasil ps yang terlihat tidak ada proses yang berada pada state suspend, yang ada hanya ready, wait, recv dan curr
11. Berapa PID (Process ID) dari Main process?
jawab : 4
note : 
- ![jawaban n0 3-5](image/jawaban_3-5.jpeg)
- ![jawaban n0 6-11](image/jawaban_6-11.jpeg)

## C. Referensi

1. https://blog.dewaweb.com/mengenal-cli-adalah/
2. https://www.pojokata.com/2025/07/memahami-shell-dalam-komputasi-sebagai.html
3. https://www.linuxid.net/post/memahami-struktur-direktori-linux-untuk-pemula/
4. https://www.hobon.id/apa-arti-kompilasi-dalam-pemrograman/artikel/432
5. https://server.co.id/proses-booting-komputer-tahapan-dari-post-hingga-os-load/
