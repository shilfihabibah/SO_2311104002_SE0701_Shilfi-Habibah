# <h1 align="center">Laporan Praktikum Modul 2  <br> Instalasi Xinu </h1>
<p align="center">SHILFI HABIBAH - 2311104002</p>

## A. Dasar Teori

### a. File .OVA
File OVA (Peralatan Virtual Terbuka) adalah jenis berkas yang digunakan dalam virtualisasi sistem. Paket-paket ini memungkinkan Anda mendistribusikan dan menerapkan mesin virtual dengan mudah di berbagai hypervisor seperti VirtualBox, VMware, dan lainnya. File OVA terutama digunakan untuk mendistribusikan dan menyebarkan mesin virtual dengan cara yang sederhana. File-file ini memungkinkan Anda untuk berbagi lingkungan kerja yang lengkap tanpa perlu mengonfigurasinya dari awal, memfasilitasi replikasi sistem yang tepat di berbagai komputer atau lingkungan.

## B. Guided

### 1. Import dan Setting Development-System VM

![Import OVA](Image/import-ova.jpeg)
Setelah instalasi selesai, import file development-system.ova pada VirtualBox.

Langkah - langkah setting :
- Pilih "Setting"
- Masuk ke menu "Network" dan ubah setting jaringan menjadi "NAT" ( ![Network](Image/Network_development-system.ova.jpeg) )
- Masuk ke menu "Serial Ports" dan ubah setting pada Path/Address jadi '\\.\pipe\com_1' ( ![Serial Ports](Image/Serial-Ports_development-system.ova.jpeg) )
- Masuk ke menu "Display" dan centang 'Enable 3D Acceleration' ( ![Display](Image/Display_development-system.ova.jpeg) )
- setelah selesai semua setting klik ok untuk menyimpan perubahan setting 

### 2. Import dan Setting Backend VM

![Import OVA](Image/import-ova.jpeg)
Setelah instalasi selesai, import file development-system.ova pada VirtualBox.

Langkah - langkah setting : 
- Pilih "Setting"
- Masuk ke menu "Network" dan ubah setting jaringan menjadi "NAT" ( ![Network](Image/Network_backend.ova.jpeg) )
- Masuk ke menu "Serial Ports" dan ubah setting pada Path/Address harus sama dengan development-system ( ![Serial Ports](Image/Serial-Ports_backend.ova.jpeg) )
- Mask ke menu "Sistem" ubah setting CPU jadi 2 ( ![Sistem](Image/Sistem_backend.ova.jpeg) )
- setelah selesai semua setting klik ok untuk menyimpan perubahan setting

### 3. Menjalankan Xinu

![Run Xinu](Image/run-xinu.jpeg)

Langkah - langkah run:
- Run development-system , nanti akan loading dan proses berjalan sampai muncul tampilan awal xinu , kemudian kita masukan sandi “xinurocks” sampai muncul seperti ss an diatas
- Run backend juga setelah proses loading selesai juga tampil seperti ss an diatas


## C. Referensi

1. https://www.polimetro.com/id/apa-itu-file-ova/
