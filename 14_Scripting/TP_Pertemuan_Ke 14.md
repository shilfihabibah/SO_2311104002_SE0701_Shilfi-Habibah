# <h1 align="center">Laporan Praktikum Modul 14  <br> Scripting </h1>
<p align="center">SHILFI HABIBAH - 2311104002</p>

## A. Dasar Teori

### a. Bash
Bash (Bourne-Again Shell) adalah sebuah jembatan antara kita sebagai user dan sistem operasi. Setiap kali kita mengetikkan perintah di terminal, Bash akan menerjemahlan perintah tersebut supaya dapat dieksekusi oleh sistem. Hal yang menarik, Bash tidak hanya digunakan secara interaktif melalui terminal, tetapi juga dapat dijalankan melalui file script. File inilah yang biasa disebut bash script. Isinya sederhana, yaitu kumpulan perintah Linux yang dijalankan secara berurutan. Biasanya file ini berekstensi .sh

### b. Struktur Data Bash Script
Secara tampilan, bash script memang terlihat sederhana. Namun, ada beberapa bagian penting yang perlu diperhatikan :
- #!/bin/bash (shebang) : Ini adalah hal wajib yang ada di baris pertama. Fungsinya untuk memberi tahu sistem bahwa script harus dijalankan dengan Bash
- Komentar : Apapun perintah setelah # tidak akan dieksekusi
- Perintah : Isinya adalah perintah Linux itu sendiri, misalnya echo, ls, dan lain-lain
Supaya script dapat dijalankan, kita juga perlu untuk memberi izin eksekusi menggunakan chmod, misalnya chmod +x namascript.sh, lalu dijalankan dengan ./namascript.sh

## B. Unguided

### 1. PERMULAAN

a. Buatlah file bernama greeting.sh sesuai dengan template code.
   ![1a](Image/1a.jpeg)
b. Buatlah script pada greeting.sh sehingga:
   i. Dapat menyapa user
   ii. Menampilkan tanggal hari ini
   iii. Menampilkan user yang sedang login saat ini

   ![1b](Image/1b.jpeg)

   - date → menampilkan tanggal dan waktu
   - who → menampilkan user yang login

### 2. PENGONDISIAN

a. Buatlah file bernama greeting_1.sh sesuai dengan template code.

   ![2a](Image/2a.jpeg)

b. Buatlah script pada greeting_1.sh sehingga dapat menampilkan “selamat pagi” pada
pagi hari (05:01-10:00), “selamat siang” pada siang hari (10:01-15:00), “selamat sore”
pada sore hari (15:01-19:00) “selamat malam” pada malam hari (19:01-05:00).

   ![2b](Image/2b.jpeg)

   Script mengecek jam saat ini lalu menampilkan salam sesuai waktu.

### 3. PERULANGAN

a. Buatlah file bernama countdown.sh sesuai dengan template code.

   ![3a](Image/3a.jpeg)

b. Buatlah script sehingga menghasilkan countdown dimulai dari angka 10 hingga angka 1 lalu diikuti tulisan “GO!”.

   ![3b](Image/3b.jpeg)

### 4. INPUT PENGGUNA

a. Buatlah file bernama countdown_1.sh sesuai dengan template code.

   ![4a](Image/4a.jpeg)

b. Buatlah script sehingga menghasilkan countdown berdasarkan masukan dari user.

   ![4b](Image/4b.jpeg)

### 5. PARAMETER SCRIPT

a. Buatlah file bernama countdown_2.sh sesuai dengan template code.

   ![5a](Image/5a.jpeg)

b. Buatlah script sehingga menghasilkan countdown berdasarkan parameter script.
Pastikan kondisi-kondisi lain ditangani.

   ![5b](Image/5b.jpeg)

### 6. PENGONDISIAN (FOR, DIRECTORY)

a. Buatlah file bernama list_direktori.sh. Jangan lupa untuk mengubah ijin script
sehingga dapat dieksekusi.

   ![6a](Image/6a.jpeg)
b. Buatlah script sehingga menampilkan semua file pada direktori tersebut.
   
   ![6b](Image/6b.jpeg)
   
## D. Referensi

1. https://telkomuniversityofficial-my.sharepoint.com/shared?listurl=https%3A%2F%2Ftelkomuniversityofficial-my.sharepoint.com%2Fpersonal%2Fmaghaz_student_telkomuniversity_ac_id%2FDocuments&id=%2Fpersonal%2Fmaghaz_student_telkomuniversity_ac_id%2FDocuments%2F2026%2F00.+Modul+Praktikum+Sistem+Operasi+SE+2526-2.pdf&parent=%2Fpersonal%2Fmaghaz_student_telkomuniversity_ac_id%2FDocuments%2F2026&shareLink=1&ga=1
2. https://medium.com/@jejeproject32/mengenal-bash-scripting-untuk-otomasi-sistem-operasi-e834402c9030










