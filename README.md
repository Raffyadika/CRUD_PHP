# Student Management (PHP CRUD)

Aplikasi web sederhana untuk mengelola data mahasiswa, dibuat untuk praktikum Web Programming.

## Fitur

- CRUD data mahasiswa (tambah, lihat, ubah, hapus)
- Relasi satu-ke-banyak antara tabel `majors` dan `students` (FOREIGN KEY + JOIN)
- Login dengan password ter-hash (`password_hash` / `password_verify`) dan session
- Role `admin` dan `staff`, dengan pembatasan akses di sisi server

## Tools

PHP, MySQL, Bootstrap 5, XAMPP

## Cara menjalankan di komputer sendiri

1. Install [XAMPP](https://www.apachefriends.org/), lalu jalankan **Apache** dan **MySQL**.
2. Download atau clone repo ini, lalu letakkan isi foldernya di `C:\xampp\htdocs\(Folder Baru)`.
3. Buka `http://localhost/phpmyadmin`, buat database kosong bernama `db_school`, pilih database itu, buka tab **Import**, lalu pilih file `database.sql` dari repo ini.
4. Buka `http://localhost/(Folder Baru)/` di browser.
5. Login dengan:
   - Username: `admin`
   - Password: `admin123`

## Hak akses

| Aksi | admin | staff |
|---|---|---|
| Lihat dashboard | Ya | Ya |
| Tambah / ubah mahasiswa | Ya | Ya |
| Hapus mahasiswa | Ya | Tidak |
| Kelola user (`users.php`) | Ya | Tidak |

## Catatan

Akun `admin` / `admin123` defaultnya bisa diganti passwordnya.