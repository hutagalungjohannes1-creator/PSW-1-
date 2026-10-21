Nama: Johannes Hutagalung
NIM: 41426034
PRODI: D4 Teknologi Rekayasa Perangkat Lunak

1. Peran ID = identitas untuk elemen
   Peran Name = Nama variabel/label data saat dikirim.
   Peran Type = Menentukan jenis kolom input.

2. 1 Pilih prodi dan satu mode kehadiran. 
2 Uji bergantian Daring dan Luring; hanya satu boleh aktif. 
3 Isi catatan opsional. 
4 Klik Daftar dan lihat query URL. 
5 Tulis pasangan nama-nilai yang terlihat.

Penyelesaian:
nama = Johannes
email = hutagalungjohannes1@gmail.com
prodi = trpl (D4 TRPL)
mode = luring
catatan = hadir

3. Pertanyaan laporan 
1 Mengapa telepon bukan kuantitas number? 
2 Apa beda label pilihan dan legend kelompok? 
3 Apa beda id dan name? 
4 Apa yang terjadi pada checkbox tidak dicentang?

1 Nomor telepon digunakan sebagai identitas/teks biasa, bukan untuk perhitungan matematika (tidak perlu dijumlahkan, dikurangi, atau dirata-rata).
2 <label> memberi keterangan untuk satu elemen input spesifik (misal: satu checkbox atau satu radio button tertentu).

<legend> memberi judul/keterangan untuk satu kelompok elemen input yang dibungkus di dalam elemen <fieldset>

3 id: Identitas unik untuk satu elemen spesifik di halaman HTML (digunakan untuk menghubungkan <label for=""> atau styling CSS/JavaScript). Nilainya tidak boleh ganda.
  name: Nama variabel/kunci (key) yang dikirimkan ke server/URL saat formulir di-submit. name bisa bernilai sama pada beberapa input (seperti pada radio button atau checkbox) untuk mengelompokkan data.

4 Jika checkbox tidak dicentang, nama variabel (name) beserta nilainya (value) tidak akan ikut terkirim sama sekali ke dalam Query URL saat formulir di-submit.

