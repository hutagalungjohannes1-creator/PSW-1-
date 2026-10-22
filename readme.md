1. **Menyiapkan Halaman (Multipage Setup)**

A. Struktur Berkas dan Kode
Halaman web disusun dengan struktur tiga file HTML utama yang terhubung ke satu file stylesheet CSS bersama:
* `index.html` (Beranda)
* `kegiatan.html` (Kegiatan)
* `daftar.html` (Daftar)
* `css/style.css` (Stylesheet Bersama)

B. Konfigurasi Dasar HTML
Pada ketiga file HTML, telah diterapkan aturan dasar sesuai ketentuan:

Pada ketiga file HTML, telah diterapkan aturan dasar sesuai ketentuan:
1. **Title Unik:** Memiliki elemen `<title>` yang berbeda pada setiap halaman untuk identifikasi tab browser (misal: "Beranda - IT Del", "Daftar Kegiatan - IT Del", "Form Pendaftaran - IT Del").
2. **Atribut Bahasa & Viewport:** Menggunakan `<html lang="id">` untuk mendukung aksesibilitas bahasa Indonesia serta tag `<meta name="viewport" content="width=device-width, initial-scale=1.0">` untuk responsivitas layar.
3. **Shared Stylesheet:** Semua halaman dihubungkan ke stylesheet bersama melalui tag `<link rel="stylesheet" href="css/style.css">`.

C. Catatan Pengamatan & Hasil Uji
Tindakan yang Dilakukan:Saya membuat tiga file HTML baru di folder proyek, yaitu index.html untuk halaman beranda, kegiatan.html untuk halaman kegiatan, dan daftar.html untuk halaman daftar.   Menambahkan judul (<title>) yang berbeda-beda di setiap file HTML supaya bisa dibedakan saat dibuka di tab browser. Memasang atribut bahasa Indonesia (lang="id") dan meta viewport di bagian <head> agar halaman rapi dan pas di layar HP maupun laptop. Menghubungkan ketiga halaman tersebut ke satu file CSS yang sama yaitu css/style.css agar gaya tampilannya seragam. Hasil Nyata (Actual Result):

Saat dijalankan menggunakan Live Server, ketiga halaman berhasil terbuka dengan mulus.

2. **NAVIGASI KONSISTEN**

A. Tindakan

Menyalin pola navigasi ke semua halaman (index.html, kegiatan.html, dan daftar.html) menggunakan elemen <nav aria-label="Navigasi utama">.

Menambahkan atribut aria-current="page" khusus pada halaman yang sedang aktif.

Melakukan pengujian navigasi dengan cara:
Mengklik semua tautan tujuan dari setiap halaman.

Memeriksa penandaan halaman aktif via DevTools.

Menguji tombol Back (Kembali) dan Forward (Maju) pada browser.

B. Hasil Nyata

Semua jalur navigasi bekerja dengan lancar tanpa ada tautan yang rusak (404), penandaan aria-current berpindah sesuai halaman yang dibuka, serta fungsi navigasi riwayat browser (Back dan Forward) berjalan normal.

3. 

