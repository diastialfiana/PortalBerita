# Fullstack_Portal-Berita
 
Biodata Mahasiswa universitas Krisnadwipayana dalam melaksanakan magang mandiri kampus merdeka batch 7 selama 4 bulan di PT. Winnicode Garuda Teknologi Devisi Fullstack Developer.
Kelompok :

Nama 	: Alka Prayoga, Email : alkhaprayogha15@gmail.com 

Nama 	: Muhamad Rifki Aulia Rahman, Email : 123rifky88@gmail.com

Software yang diperlukan Visual Studio Code, Xampp, Browser.
Download semua software di atas, serta download semua file dan masukan kedalam folder local : C terus pilih ke folder Xampp - dan pilih folder Htdoc.

Tutorial Menjalankan Proyek Fullstack Portal Berita

Berikut adalah langkah-langkah untuk menjalankan proyek Fullstack Portal Berita secara lengkap dan terstruktur:

1. Persiapan Software

Unduh dan instal software berikut:

Visual Studio Code: Digunakan sebagai editor kode.

XAMPP: Menyediakan server lokal yang mencakup Apache dan MySQL.

Browser: Contoh: Chrome, Firefox, atau browser lainnya.

Download semua file proyek dan simpan ke dalam folder:

C:\xampp\htdocs\fullstack_portalBerita

2. Menjalankan XAMPP

Buka XAMPP Control Panel.

Klik tombol "Start" pada bagian Apache dan MySQL untuk menjalankan server.

3. Membuat Database

Buka Command Prompt (CMD), lalu masukkan perintah berikut satu per satu:

c:
cd \xampp\mysql\bin
mysql -u root

Setelah masuk ke MySQL shell, buat database dan tabel dengan perintah berikut:

CREATE DATABASE user_db;

USE user_db;

CREATE TABLE users (
    id INT(11) AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    password VARCHAR(255) NOT NULL,
    full_name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL
);

lalu buat database admin dan tabel admin dengan perintah berikut :

CREATE DATABASE admin_db;

USE admin_db;

CREATE TABLE admin (
    id INT(11) AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    password VARCHAR(255) NOT NULL,
    full_name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL
);
4. Menjalankan Proyek

Pastikan Apache dan MySQL pada XAMPP masih dalam keadaan aktif.

Buka browser, lalu akses URL berikut:

Halaman utama: http://localhost/Fullstack_PortalBerita/index.html

Halaman politik: http://localhost/Fullstack_PortalBerita/Politik.html

Ganti nama file terakhir sesuai dengan halaman yang ingin dibuka, misalnya home.html atau Politik.html.

Catatan Penting

Koneksi ke Database:
Pastikan file PHP Anda memiliki konfigurasi koneksi database yang benar. Biasanya, file koneksi terletak di direktori proyek, misalnya config.php. Berikut adalah contoh konfigurasi koneksi:

<?php
$servername = "localhost";
$username = "root";
$password = "";
$dbname = "use_db";

// Membuat koneksi
$conn = new mysqli($servername, $username, $password, $dbname);

// Mengecek koneksi
if ($conn->connect_error) {
    die("Koneksi gagal: " . $conn->connect_error);
}
?>

Cek Error:
Jika terjadi error, pastikan:

Database dan tabel telah dibuat dengan benar.

Semua file proyek telah diunggah ke folder htdocs di XAMPP.
