Nama: Johannes Hutagalung
NIM: 41426034
Prodi: D4 TRPL

1. RESET UKURAN KOTAK
 Deskripsi Perubahan Kode
Pada tahap ini, dilakukan reset ukuran kotak secara global menggunakan box-sizing: border-box pada semua elemen dan pseudo-element (before, after). Selain itu, dilakukan penyesuaian aturan pada elemen utama <main> agar lebih fleksibel dan responsif di berbagai ukuran layar.
2. TOKEN WARNA DAN JARAK
Apa yang Dikerjakan?
Membuat "variabel" warna dan jarak di bagian root pada file style.css. Jadi, warna utama, warna latar, dan ukuran jarak disimpan di satu tempat di paling atas CSS
Catatan Pengamatan:
- **Kemudahan**: Kalau mau ganti warna tema web (misal dari biru ke merah), cukup ganti kode warna di bagian root satu kali saja, lalu tombol dan teks warna di seluruh web akan langsung berubah otomatis.
- **Bebas Masalah**: Perubahan warna dan jarak berjalan lancar tanpa perlu memaksa pake kode.
3. TIPOGRAFI DAN UNIT
Apa yang Dikerjakan?
1. Mengatur font dasar pada body menggunakan font-size: 1rem dan line-height: 1.6 tanpa satuan agar jarak antar-baris lebih alami.
2. Membatasi panjang paragraf dengan `p { max-width: 65ch;}supaya baris kalimat tidak terlalu panjang saat dibaca.

catatan Pengamatan:**Pemeriksaan DevTools**: Ukuran 1rem terhitung senilai 16px, sedangkan 1.5rem terhitung 24px
**Uji Zoom 200%**: Ketika browser di-zoom hingga 200%, seluruh teks membesar secara proporsional, layout tetap rapi, dan tidak ada teks yang terpotong atau hilang.

4. Organisasi Kode & Audit Aksesibilitas
Apa yang Dikerjakan?
1. Merapikan struktur file CSS ke dalam 4 kelompok terpisah: Base, Wadah/Layout, Komponen, dan Interaction States
2. Menambahkan efek focus-visible dengan garis batas (outline: 3px solid var(--brand); outline-offset: 3px;)
3. Membuang seluruh kode CSS eksperimen lama yang tidak terpakai
Catatan Pengamatan & Audit:
**Navigasi Keyboard**: Saat berpindah antar-input menggunakan tombol Tab, posisi fokus terlihat sangat jelas berkat garis batas luar (outline-offset), membantu pengguna keyboard/screen-reader
Warna utama (brand: #175cd3`) pada tombol dan teks notice memenuhi standar kontras keterbacaan di atas latar belakang putih
**Konflik yang Diperbaiki**: Menyelesaikan konflik spesifisitas pada gaya fokus elemen form dengan menyatukan aturan focus-visible pada kelompok Interaction States di bagian paling bawah CSS
Laporan Troubleshooting & Diagnosis
Isu Overflow Lebar Input Formulir:
Gejala: Elemen input teks memanjang melewati batas bingkai .card saat dikonfigurasi width: 100%.
Penyebab: Perhitungan bawaan peramban (content-box) menambahkan ukuran padding di luar total lebar elemen.
Solusi: Menyisipkan deklarasi box-sizing: border-box pada selektor reset universal.
Analisis Hirarki Gaya & Specificity:
Pemeriksaan: Memastikan letak aturan :focus-visible berada di bawah deklarasi dasar input dan button agar efek gaya dapat mereset aturan awal tanpa harus mengandalkan !important.

Pernyataan Penggunaan AI (AI Use Statement)
Alat AI: Gemini
Tujuan Penggunaan: Membantu perancangan struktur dokumen README.md serta memvalidasi kriteria pengujian sesuai acuan WCAG/W3C.
Bagian Bantuan: Penyusunan tabel matriks uji coba, penulisan narasi analisis box model, dan pemodelan langkah-langkah kerja.
Verifikasi Mandiri: Seluruh baris kode HTML dan CSS telah dites dan dikonfirmasi fungsinya secara langsung menggunakan peramban modern dan Live Server.