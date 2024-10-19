#Event App

Aplikasi Event APP adalah aplikasi yang dirancang untuk menampilkan daftar acara menggunakan data dari Dicoding Events API. Pengguna dapat melihat acara yang akan datang dan acara yang sudah selesai, serta mendapatkan detail lengkap dari setiap acara.

Fitur Utama
Bottom Navigation
Aplikasi ini menampilkan dua jenis list event:

Acara Aktif/Akan Datang: Menampilkan acara yang akan datang.
Acara Sudah Selesai: Menampilkan acara yang telah selesai.
List Data Event
Menampilkan list data acara dari API dengan informasi minimal sebagai berikut:

Gambar (imageLogo/mediaCover)
Nama acara (name)
Halaman Detail Event
Pengguna dapat mengakses halaman detail untuk setiap acara, yang mencakup:

Gambar (imageLogo/mediaCover)
Nama acara (name)
Penyelenggara acara (ownerName)
Waktu acara (beginTime)
Sisa kuota (quota - registrant)
Deskripsi acara (description)
Tombol untuk membuka link acara (link)
Indikator Loading
Terdapat indikator loading yang muncul saat aplikasi memuat data dari API di semua bagian.

API yang Digunakan
Dokumentasi API Dicoding Events dapat ditemukan di sini. Berikut adalah endpoint yang digunakan dalam aplikasi ini:

Event yang Aktif (Akan Datang):
GET https://event-api.dicoding.dev/events?active=1

Event yang Sudah Selesai:
GET https://event-api.dicoding.dev/events?active=0

Search Event:
GET https://event-api.dicoding.dev/events?active=-1&q={keyword}

Detail Event:
GET https://event-api.dicoding.dev/events/{id}

Instalasi
Clone repositori ini ke dalam direktori lokal Anda:

bash
Copy code
git clone https://github.com/username/repository-name.git
Buka proyek di IDE pilihan Anda.

Jalankan aplikasi di emulator atau perangkat fisik.

Kontribusi
Jika Anda ingin berkontribusi pada proyek ini, silakan buat fork repositori ini, lakukan perubahan yang diinginkan, dan ajukan pull request.

