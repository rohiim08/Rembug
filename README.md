# Rembug - Platform Diskusi Berbasis Gambar

Rembug adalah aplikasi web media sosial yang memungkinkan pengguna untuk berbagi pemikiran dan momen mereka melalui gambar dan teks. Proyek ini dibangun dengan framework Laravel dan menggunakan MongoDB sebagai databasenya, memberikan platform yang dinamis dan interaktif bagi pengguna untuk terhubung dan berdiskusi.

## Fitur Utama

* **Autentikasi Pengguna:** Sistem pendaftaran dan login yang aman untuk pengguna.
* **Berbagi Postingan:** Pengguna dapat membuat, mengedit, dan menghapus postingan dengan gambar dan caption.
* **Sistem Interaksi:**
    * **Like:** Pengguna dapat menyukai dan tidak menyukai postingan.
    * **Coment:** Pengguna dapat berkomentar di postingan dan menghapus komentar mereka sendiri.
    * **Follow:** Sistem mengikuti (follow/unfollow) untuk tetap terhubung dengan pengguna lain.
* **Profil Pengguna:** Halaman profil yang dapat disesuaikan dengan gambar profil, bio, dan galeri postingan.
* **Pencarian:** Fungsi pencarian untuk menemukan pengguna dan postingan.

## Teknologi yang Digunakan

* **Backend:** Laravel 12
* **Database:** MongoDB
* **Frontend:**
    * Bootstrap 5
    * Sass
    * Vite
* **Lainnya:**
    * Composer
    * NPM

## Instalasi dan Setup

Ikuti langkah-langkah berikut untuk menjalankan proyek ini secara lokal:

1.  **Clone Repositori**
    ```bash
    git clone [https://github.com/nama-pengguna-anda/rembug-project.git](https://github.com/nama-pengguna-anda/rembug-project.git)
    cd rembug-project
    ```

2.  **Instal Dependensi**
    Pastikan Anda memiliki Composer dan NPM terinstal.
    ```bash
    composer install
    npm install
    ```

3.  **Konfigurasi Lingkungan**
    Salin file `.env.example` menjadi `.env` dan sesuaikan variabel lingkungan, terutama koneksi database MongoDB.
    ```bash
    cp .env.example .env
    ```
    Pastikan untuk mengisi variabel berikut di file `.env` Anda:
    ```
    DB_CONNECTION=mongodb
    DB_URI=mongodb://127.0.0.1:27017
    DB_DATABASE=rembug
    ```

4.  **Generate Kunci Aplikasi**
    ```bash
    php artisan key:generate
    ```

5.  **Migrasi Database**
    Jalankan migrasi untuk membuat koleksi yang diperlukan di MongoDB.
    ```bash
    php artisan migrate
    ```

6.  **Jalankan Aplikasi**
    Gunakan Vite untuk meng-compile aset frontend dan jalankan server pengembangan Laravel.
    ```bash
    npm run dev
    php artisan serve
    ```

    Aplikasi Anda sekarang akan berjalan di `http://localhost:8000`.

## Penggunaan

Setelah instalasi selesai, Anda dapat mendaftar untuk akun baru dan mulai menggunakan fitur-fitur berikut:
* Buat postingan baru dengan gambar dan caption.
* Jelajahi postingan dari pengguna lain di halaman utama.
* Cari pengguna dan postingan melalui bilah pencarian.
* Lihat dan edit profil Anda.
* Ikuti pengguna lain untuk melihat postingan mereka di feed Anda.
