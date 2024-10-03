Nama : CAHAYA HIJRUN

Nim : 09030282327014

Kelas : TK 3 C

Mata Kuliah : Arsitektur Dan Organisasi Komputer

# 1.	Buatlah laporan proses instalasi di computer mahasiswa dan tampilkan screenshotnya.


# a. Download Virtual Box di https://www.virtualbox.com/Downloads, laluinstall di komputer anda sampai selesai dengan sukses.
![Cuplikan layar 2024-10-03 230509](https://github.com/user-attachments/assets/1cc09634-d850-4f6a-90d8-aa07e22dd4d7)


# b. Langkah kedua yaitu membuat mesin baru dengan menekan tombol New, setelah itu akan muncul isian tentang mesin baru yang telah dibuat.
![Cuplikan layar 2024-10-03 235342](https://github.com/user-attachments/assets/6a7ac9be-e026-4fdc-8e5f-89520a39b1e1)


# c. Langkah ketiga adalah menentukan besaran memory pada virtual machine, cukup berikan memory dengan ukuran memory pada virtual machine hendaknya tidak melebihi ukuran memori fisik sebenarnya.
![Cuplikan layar 2024-10-03 235535](https://github.com/user-attachments/assets/4545afef-4621-4b67-922d-51620b0755be)


# d. Langkah berikutnya adalah membuat hard drive virtual.
![Cuplikan layar 2024-10-03 235550](https://github.com/user-attachments/assets/27b65536-2966-413a-8962-e34be38b2c3d)

Dalam membuat hard drivevirtual, opsi yang dipilih adalah Create a virtual hard drive now lalu tekan tombol Create. Langkah berikutnya adalah memilih jenis hard drive apakah ukurannya dinamis atau fix. Yang dipilih adalah dynamically Alocated. Langkah berikutnyamenentukan ukuran hard drive virtual, yang diperlukan adalah 8 GB kemudian tekan tombol Create.

# e. Langkah berikutnya memuat file instalasi dalam format .iso untuk dimuat di dalam CD/DVD Drive. Klik Storage lalu pada Storage tree arahkan pada Empty CD/DVD lalu pada Attributes pilih Choose a CD/DVD disk file. Muat file dengan ekstensi .iso ke dalam Empty CD/DVD.
![Cuplikan layar 2024-10-04 000136](https://github.com/user-attachments/assets/b6464bad-f265-4183-bbe2-79b4d097c805)

# f. Setelah menentukan besaran memory virtual dan membuat hard drive virtual,langkah berikutnya adalah mulai menjalankan mesin baru dengan menekan tombol "Start".
![Cuplikan layar 2024-10-04 001449](https://github.com/user-attachments/assets/3dfa0000-e9f1-4e5f-8c6e-60390ad5db24)

# g. Proses menginstall ubuntu.
![Cuplikan layar 2024-10-04 004726](https://github.com/user-attachments/assets/b376dc3e-5271-48f3-9609-9bb1811f31ed)

# h. Pengisian Username dan Password.
![Cuplikan layar 2024-10-04 005208](https://github.com/user-attachments/assets/f65c3503-f9b9-4db8-ba0e-9c0830bf1763)

# i. Ketika sudah muncul seperti di bawah maka kita memasukkan Password dan Linux siap di gunakan.
![WhatsApp Image 2024-10-04 at 00 55 51](https://github.com/user-attachments/assets/df8faa3c-e650-4a56-a20e-f2fe5a91a273)


# 2. Analisislah pada gambar kenapa saat instalasi perlu dipilih “/” pada opsi Mount Point ?


Sangat penting untuk memilih titik pemasangan yang benar “/” saat memasang sistem operasi seperti linux. Berikut penyebabnya:

# 1).	Direktori Root:
- Direktori utama sistem operasi linux untuk semua file dan direktori adalah “/”, yang juga     dikenal sebagai direktori root. Dimulai dari root, setiap program dan file sistem akan diatur dalam hierarki.
- Saat memilih “/” sebagai titik pemasangan selama pemasangan sistem operasi, sistem operasi dan file utamanya akan disimpan di disk ini.

# 2). Organisasi Berkas Linux:
- Struktur direktori di linux bersifat hierarkis dan dimulai dari akar. Direktori akar memuat semua direktori lain, termasuk /home, /var, /etc, dan seterusnya.
- Sistem operasi tidak akan dapat berfungsi dengan benar tanpa partisi yang dipasang pada “/” karena tidak memiliki tempat untuk menyimpan berkas sistemnya.

# 3).	Menyiapkan partisi:
- Partisi baru dibuat dalam instalasi ini untuk berfungsi sebagai partisi utama. “/’ adalah partisi yang diperlukan untuk sistem operasi, sementara kita dapat memilih untuk membuat partisi lain untuk folder tertentu, sperti /home.

# 4).	Memanfaatkan sistem berkas:
- Karena keandalan dan kinerjanya yang kuat, pengguna linux sering memilih sistem berkas Ext4, yang merupakan partisi yang dikonfigurasi untuk digunakan dalam citra ini.

Karena disinilah sistem operasi akan diinstal, memilih “/” pada opsi Mount Point selama instalasi merupakan langkah yang diperlukan untuk menjamin bahwa sistem operasi dapat berfungsi dengan baik.


# 3. Berikan penjelasan tentang ext4, ext3, swap, ntfs, fat32,btrfs!
Berikut ini menjelaskan berbagai jenis sistem berkas yang sering ditemukan dalam sistem operasi:


# 1). Ext4
•	Iterasi terbaru dari sistem berkas Linux yang populer, Ext4, disebut Ext4.

•	Ext4 lebih stabil, berkinerja lebih baik, dan mendukung kapasitas penyimpanan yang lebih besar daripada Ext3.

•	Fitur Unggulan:

 _1. Dukungan untuk berkas dan volume hingga 16 terabyte dan hingga 1 exabyte._
 
_2. Menggunakan penjurnalan untuk melindungi dari kerusakan data jika terjadi penghentian atau kerusakan sistem yang tidak terduga._

_3. Memiliki fitur ekstensi yang mempercepat akses berkas dan menurunkan fragmentasi disk._

•	Penggunaan: Sistem operasi Linux terkini (Ubuntu, Fedora, Debian, dll.).

# 2). Ext3
•	Ext3 adalah sistem berkas penjurnalan pertama untuk Linux dan cikal bakal Ext4.

•	Fitur Utama :

_1. Dengan mencatat perubahan sebelum ditulis ke disk, penjurnalan meningkatkan keamanan terhadap kegagalan sistem._

_2. Meskipun lebih lambat dari Ext4, sistem ini lebih stabil dan terbukti dapat diandalkan dalam berbagai pengaturan produksi._

_3. Karena partisi Ext2 kompatibel dengan Ext3, data tidak akan hilang selama pemutakhiran dari Ext2 ke Ext3._

•	Penggunaan : Sering digunakan pada server yang stabil atau sistem Linux lama yang tidak memerlukan fitur Ext4 yang lebih baru.

# 3).	Swap
•	Swap adalah area hard drive yang digunakan sistem operasi untuk menambah memori virtual, ini bukanlah sistem file.

•	Data dari memori akan ditukar dengan (swapped) saat RAM habis.

•	Fungsi: Meskipun RAM fisik memiliki keterbatasan, ini memungkinkan sistem operasi untuk mengelola lebih banyak proses.

•	penggunaan: Sebagai memori virtual tambahan dalam sistem Linux dan Unix.

# 4). Ntfs 
•	Ntfs adalah sistem file yang dikembangkan oleh Microsoft untuk digunakan pada sistem operasi Windows.

•	Fitur utama :

_1. Memungkinkan partisi hingga 256 TB dan mendukung berkas besar hingga 16 TB._

_2. Memiliki dukungan metadata, keamanan data, enkripsi berkas, dan kemampuan pemulihan kesalahan._

_3. Mendukung fungsi termasuk kompresi data, penjurnalan, dan izin berkas (ACL)._

•	Penggunaan: Hard drive eksternal, USB yang digunakan dengan Windows, dan sistem operasi Windows terkini (Windows 2000 dan yang lebih baru).

# 5).	Fat32
•	Sistem file FAT yang disebut FAT32 sering digunakan dalam perangkat penyimpanan seperti kartu memori dan flashdisk USB.

•	Fitur :

_1. Memungkinkan ukuran partisi hingga 32 GB dan ukuran file hingga 4 GB._

_2. Lebih kompatibel dengan berbagai sistem operasi, tetapi tidak menyertakan fitur penjurnalan atau keamanan seperti NTFS._

•	Penggunaan: Drive USB dan kartu SD, yang merupakan perangkat penyimpanan portabel yang perlu bekerja dengan sistem operasi Linux, macOS, dan Windows.

# 6).	Btrfs
•	Btrfs adalah sistem berkas canggih yang dirancang untuk Linux yang memprioritaskan snapshot, manajemen volume besar, dan integritas data.

•	Fitur Utama :

_1. Mendukung fitur-fitur termasuk dukungan volume besar, verifikasi integritas data, kompresi, dan snapshot._

_2. Dengan snapshot, pengguna dapat dengan cepat dan mudah membuat salinan data tanpa menghabiskan banyak ruang._

_3. Sangat baik dalam menangani data dalam jumlah besar dan mampu memperbaiki data yang rusak secara otomatis._

•	Penggunaan : Sistem cadangan, server Linux, dan pengguna yang membutuhkan alat manajemen volume dan snapshot yang efektif.

# Ringkasan Penggunaan : 

•	Ext4  : Sistem file default di sebagian besar distribusi Linux modern.

•	Ext3  : Sistem file penjurnalan Linux lama yang lebih andal.

•	Swap  : Dalam sistem operasi Linux, swap digunakan sebagai memori virtual tambahan.

•	NTFS  : Volume besar dan fitur keamanan didukung oleh sistem berkas bawaan Windows.

•	FAT32 : sistem file digunakan dalam perangkat penyimpanan portabel yang perlu bekerja dengan sistem operasi yang berbeda.

•	Btrfs : Sistem file Linux canggih dengan fungsionalitas untuk kompresi dan snapshot
