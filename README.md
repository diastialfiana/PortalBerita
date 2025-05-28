Portal Berita Digital Berbasis Laravel
Deskripsi
Proyek ini merupakan hasil magang di PT. Winnicode Garuda Teknologi sebagai bagian dari pengembangan kompetensi profesional dalam bidang web development.
Portal Berita Digital ini dibuat untuk menyediakan akses informasi yang cepat, akurat, dan mudah dijangkau oleh masyarakat melalui berbagai perangkat digital.
Selama proses pengembangan, digunakan framework Laravel untuk backend, TailwindCSS untuk styling, serta JavaScript dan integrasi API eksternal untuk fitur-fitur interaktif.
![image](https://github.com/user-attachments/assets/c60f90f9-76b9-4f2f-9ef9-6d012c10b76f)
![image](https://github.com/user-attachments/assets/a9d85e05-dde3-49c8-99da-eca60a747978)

Cara Instalasi
Clone repository ini:
git clone https://github.com/username/portal-berita.git  
Masuk ke direktori proyek:
cd portal-berita  
Install dependencies menggunakan Composer:
composer install  
Copy file .env.example menjadi .env dan sesuaikan konfigurasi database serta API keys:
cp .env.example .env  
Generate application key:
php artisan key:generate  
Migrasi database dan seeding data awal (jika ada):
php artisan migrate --seed  
Jalankan server development:
php artisan serve  
Buka browser dan akses http://localhost:8000
