# 🌿 LMSense – Leave Management System

**LMSense** adalah aplikasi manajemen cuti kerja berbasis Laravel yang membantu perusahaan mengelola proses pengajuan cuti karyawan secara efisien dan transparan.

## ✨ Fitur Utama
- Pengajuan cuti online dengan form yang mudah digunakan  
- Persetujuan cuti berdasarkan **role-based access control**:  
  - **Karyawan** dapat mengajukan cuti dan melihat statusnya  
  - **Manajer** dapat menyetujui atau menolak pengajuan cuti bawahan di departemennya  
  - **HRD** mengelola seluruh pengajuan dan laporan cuti secara menyeluruh  
  - **Superadmin** memiliki akses penuh ke seluruh sistem dan pengaturan  
- Manajemen **departemen** untuk mengelompokkan karyawan sesuai divisi/struktur perusahaan  
- Riwayat pengajuan cuti lengkap per karyawan dan departemen  
- Notifikasi otomatis untuk status pengajuan cuti  
- Dashboard Admin untuk manajemen user, role, departemen, dan pengajuan cuti  

## 🛠️ Teknologi
- Laravel 10+  
- MySQL / MariaDB dengan relasi antar karyawan, role, dan departemen  
- Blade Template  
- Middleware Laravel untuk implementasi Role-Based Access Control (RBAC)  


## 🚀 Cara Menjalankan
```bash
git clone https://github.com/kibieptr/LMSense.git
cd LMSense
composer install
cp .env.example .env
php artisan key:generate
# Atur database di .env
php artisan migrate
php artisan serve
