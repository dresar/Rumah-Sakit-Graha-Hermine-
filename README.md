# BeliBeli Official - Web Profile Rumah Sakit

<p align="center">
  <img src="https://via.placeholder.com/800x400?text=BeliBeli+Official+Hospital+Profile" alt="BeliBeli Official Hospital Profile" width="800"/>
</p>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#tech-stack">Tech Stack</a> •
  <a href="#installation">Installation</a> •
  <a href="#usage">Usage</a> •
  <a href="#screenshots">Screenshots</a> •
  <a href="#database-structure">Database Structure</a> •
  <a href="#contributing">Contributing</a> •
  <a href="#license">License</a>
</p>

<p align="center">
  <a href="https://github.com/yourusername/belibeli-hospital/stargazers"><img src="https://img.shields.io/github/stars/yourusername/belibeli-hospital" alt="Stars Badge"/></a>
  <a href="https://github.com/yourusername/belibeli-hospital/network/members"><img src="https://img.shields.io/github/forks/yourusername/belibeli-hospital" alt="Forks Badge"/></a>
  <a href="https://github.com/yourusername/belibeli-hospital/issues"><img src="https://img.shields.io/github/issues/yourusername/belibeli-hospital" alt="Issues Badge"/></a>
  <a href="https://github.com/yourusername/belibeli-hospital/blob/master/LICENSE"><img src="https://img.shields.io/github/license/yourusername/belibeli-hospital" alt="License Badge"/></a>
</p>

## 🏥 About

**BeliBeli Official - Web Profile Rumah Sakit** adalah aplikasi web profil rumah sakit yang komprehensif, dirancang untuk memudahkan pasien dan pengunjung dalam mengakses informasi tentang layanan kesehatan, dokter, fasilitas, dan berita terkini dari rumah sakit. Aplikasi ini dibangun dengan Laravel 9, menawarkan antarmuka yang intuitif dan responsif untuk pengalaman pengguna yang optimal.

## ✨ Features

### 👥 Untuk Pengunjung
- **Informasi Poliklinik & Layanan**: Akses informasi lengkap tentang berbagai poliklinik dan layanan kesehatan yang tersedia
- **Profil Dokter**: Lihat profil dokter beserta spesialisasi dan jadwal praktik
- **Galeri Rumah Sakit**: Jelajahi galeri foto fasilitas dan kegiatan rumah sakit
- **Blog Kesehatan**: Baca artikel dan tips kesehatan terbaru
- **E-Library**: Akses perpustakaan digital dengan berbagai materi kesehatan
- **Video Edukasi**: Tonton video edukasi kesehatan dari YouTube
- **Pencarian**: Temukan informasi dengan cepat melalui fitur pencarian

### 👨‍💼 Untuk Admin
- **Dashboard Admin**: Panel kontrol untuk mengelola seluruh konten website
- **Manajemen Konten**: Kelola poliklinik, layanan, dokter, jadwal, blog, dan galeri
- **Upload Media**: Unggah dan kelola gambar dan video
- **Manajemen Pengguna**: Kelola akun admin dan hak akses
- **Analitik**: Pantau statistik pengunjung website

## 🛠️ Tech Stack

- **Backend**: Laravel 9, PHP 8.x
- **Frontend**: Blade Templates, JavaScript, Bootstrap
- **Database**: MySQL/SQLite
- **Media Storage**: Local Storage/AWS S3
- **Deployment**: Apache/Nginx

## 📋 Requirements

- PHP >= 8.0
- Composer
- Node.js & NPM
- MySQL/SQLite
- Web Server (Apache/Nginx)

## 🚀 Installation

### Menggunakan MySQL

1. **Clone repository**
   ```bash
   git clone https://github.com/yourusername/belibeli-hospital.git
   cd belibeli-hospital
   ```

2. **Install dependencies**
   ```bash
   composer install
   npm install
   npm run build
   ```

3. **Setup environment**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. **Konfigurasi database di file .env**
   ```
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=laravelcompany
   DB_USERNAME=root
   DB_PASSWORD=
   ```

5. **Migrasi dan seed database**
   ```bash
   php artisan migrate:fresh --seed
   ```

6. **Jalankan aplikasi**
   ```bash
   php artisan serve
   ```

### Menggunakan SQLite

1. **Buat file database SQLite**
   ```bash
   touch database/database.sqlite
   ```

2. **Konfigurasi database di file .env**
   ```
   DB_CONNECTION=sqlite
   # Hapus atau komentari baris DB_HOST, DB_PORT, DB_DATABASE, DB_USERNAME, DB_PASSWORD
   ```

3. **Migrasi dan seed database**
   ```bash
   php artisan migrate:fresh --seed
   ```

## 🔧 Usage

### Akses Frontend
Buka browser dan akses `http://localhost:8000` untuk melihat website rumah sakit.

### Akses Admin Panel
1. Buka `http://localhost:8000/login`
2. Login dengan kredensial admin:
   - Username: `admin`
   - Password: `admin123`
   
   atau
   
   - Username: `kusuka`
   - Password: `123456`

## 📷 Screenshots

<p align="center">
  <img src="https://via.placeholder.com/400x200?text=Homepage" alt="Homepage" width="400"/>
  <img src="https://via.placeholder.com/400x200?text=Doctor+Profiles" alt="Doctor Profiles" width="400"/>
</p>

<p align="center">
  <img src="https://via.placeholder.com/400x200?text=Services" alt="Services" width="400"/>
  <img src="https://via.placeholder.com/400x200?text=Admin+Dashboard" alt="Admin Dashboard" width="400"/>
</p>

## 📊 Database Structure

Aplikasi ini menggunakan beberapa model utama:

- **User**: Admin dan pengguna sistem
- **Layanan_poliklinik**: Informasi tentang poliklinik dan layanan
- **Dokter**: Data dokter dan spesialisasi
- **JadwalDokter**: Jadwal praktik dokter
- **Blog**: Artikel dan berita kesehatan
- **PostCategory**: Kategori untuk artikel blog
- **Galeri**: Foto kegiatan dan fasilitas
- **KategoriGaleri**: Kategori untuk galeri foto
- **Elibrary**: Materi edukasi digital
- **Folder**: Pengorganisasian materi e-library
- **YtLink**: Link video edukasi YouTube
- **Fasilitas_Layanan**: Informasi fasilitas rumah sakit
- **Partnership**: Data kerjasama dengan institusi lain

## 🤝 Contributing

Kontribusi selalu disambut! Jika Anda ingin berkontribusi:

1. Fork repository
2. Buat branch fitur baru (`git checkout -b feature/amazing-feature`)
3. Commit perubahan Anda (`git commit -m 'Add some amazing feature'`)
4. Push ke branch (`git push origin feature/amazing-feature`)
5. Buka Pull Request

## 📄 License

Didistribusikan di bawah Lisensi MIT. Lihat `LICENSE` untuk informasi lebih lanjut.

## 📞 Contact

Project Link: [https://github.com/yourusername/belibeli-hospital](https://github.com/yourusername/belibeli-hospital)

## 💖 Support

<p align="center">
  <a href="https://www.buymeacoffee.com/yourusername" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" height="50px">
  </a>
</p>

<p align="center">
  <a href="https://twitter.com/yourusername"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"/></a>
  <a href="https://www.linkedin.com/in/yourusername"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://www.instagram.com/yourusername"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram"/></a>
</p>

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/yourusername">Your Name</a>
</p>
