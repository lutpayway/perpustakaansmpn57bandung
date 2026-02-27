📚 Sistem Informasi Perpustakaan Digital SMPN 57 Bandung
PHP Version CodeIgniter MySQL License

📖 Tentang Proyek
Sistem Informasi Perpustakaan Digital untuk SMPN 57 Bandung adalah aplikasi berbasis web yang dirancang untuk memudahkan pengelolaan perpustakaan sekolah secara digital. Aplikasi ini dibangun menggunakan CodeIgniter 4 dengan tampilan modern menggunakan AdminLTE.

✨ Fitur Utama
👨‍💼 Admin/Petugas
✅ Dashboard dengan statistik perpustakaan
✅ Manajemen Buku (Tambah, Edit, Hapus)
✅ Manajemen E-Book dengan upload file
✅ Manajemen Anggota Perpustakaan
✅ Pendaftaran Anggota Baru
✅ Manajemen Peminjaman Buku
✅ Manajemen Kategori, Penerbit, dan Penulis
✅ Manajemen Rak Buku
✅ Manajemen Kelas
✅ Pengaturan Sistem (Logo, Slider)
✅ Laporan dan Statistik
👨‍🎓 Anggota/Siswa
✅ Dashboard Anggota
✅ Gallery Buku dan E-Book
✅ Peminjaman Buku
✅ Pencarian Buku
✅ Riwayat Peminjaman
✅ Download E-Book
✅ Edit Profile
🌐 Public
✅ Halaman Home dengan Slider
✅ Katalog Buku
✅ Detail Buku
🛠️ Teknologi yang Digunakan
Framework: CodeIgniter 4
Frontend: AdminLTE 3, Bootstrap 4, jQuery
Database: MySQL/MariaDB
Web Server: Apache (XAMPP)
PHP Version: 7.4+
📋 Prasyarat
Sebelum menginstall, pastikan sistem Anda sudah memiliki:

PHP >= 7.4
MySQL/MariaDB
Apache Web Server
Composer
Extension PHP yang dibutuhkan:
intl
mbstring
json
mysqlnd
libcurl
🚀 Cara Instalasi
1. Clone Repository
git clone https://github.com/RakaAprianto/library-management-smpn57bandung.git
cd library-management-smpn57bandung
2. Install Dependencies
composer install
3. Konfigurasi Database
Buat database baru di MySQL:

CREATE DATABASE perpustakaan_smpn57;
4. Konfigurasi Environment
Copy file env menjadi .env:

cp env .env
Edit file .env dan sesuaikan konfigurasi database:

CI_ENVIRONMENT = development

database.default.hostname = localhost
database.default.database = perpustakaan_smpn57
database.default.username = root
database.default.password = 
database.default.DBDriver = MySQLi
database.default.port = 3306
5. Import Database
Import file SQL database (jika tersedia) atau jalankan migration:

php spark migrate
6. Konfigurasi Web Server
Arahkan document root ke folder public:

XAMPP (httpd.conf atau httpd-vhosts.conf):

<VirtualHost *:80>
    DocumentRoot "C:/xampp/htdocs/perpustakaan_smp57bandung/public"
    ServerName perpustakaan.local
    
    <Directory "C:/xampp/htdocs/perpustakaan_smp57bandung/public">
        Options Indexes FollowSymLinks
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>
7. Akses Aplikasi
Buka browser dan akses:

http://localhost/perpustakaan_smp57bandung/public
atau jika menggunakan virtual host:

http://perpustakaan.local
👤 Default Login
Admin/Petugas
Username: admin
Password: admin123
Anggota
Username: (sesuai yang didaftarkan)
Password: (sesuai yang didaftarkan)
⚠️ Penting: Segera ubah password default setelah login pertama kali!

📁 Struktur Folder
perpustakaan_smp57bandung/
├── app/
│   ├── Config/          # File konfigurasi
│   ├── Controllers/     # Controller
│   ├── Models/          # Model database
│   ├── Views/           # Tampilan
│   └── Filters/         # Filter autentikasi
├── public/
│   ├── AdminLTE/        # Template AdminLTE
│   ├── cover/           # Cover buku
│   ├── ebooks/          # File e-book
│   ├── foto/            # Foto anggota
│   ├── logo/            # Logo sistem
│   └── slider/          # Gambar slider
├── writable/            # Folder untuk cache & logs
├── vendor/              # Dependencies
└── .env                 # Konfigurasi environment
🔒 Keamanan
File .env sudah di-exclude dari Git untuk keamanan kredensial
Gunakan HTTPS untuk production
Ubah password default
Aktifkan CSRF protection
Gunakan prepared statements untuk query database
📝 Lisensi
Proyek ini dilisensikan di bawah MIT License.

👨‍💻 Developer
Dikembangkan oleh Raka Aprianto untuk SMPN 57 Bandung.

🙏 Kontribusi
Kontribusi selalu welcome! Silakan:

Fork repository ini
Buat branch fitur baru (git checkout -b feature/FiturBaru)
Commit perubahan (git commit -m 'Menambahkan fitur baru')
Push ke branch (git push origin feature/FiturBaru)
Buat Pull Request
📞 Kontak & Dukungan
Jika ada pertanyaan atau issue, silakan:

Buat Issue di GitHub
Email: -
🌟 Support
Jika proyek ini bermanfaat, berikan ⭐ di GitHub!
