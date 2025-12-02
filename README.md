# Lab10Web
# Nama : Alya Febrianti
# Kelas : TI.24.A1
# NIM : 312410692
lab10_php_oop/
├── mobil.php           # Mobil yang cuma bisa ganti nama warna
├── form.php            # Form yang tidak estetis
├── form_input.php      # Pemanngil form
├── database.php        # Database yang amnesia
├── config.php          # Isinya cuma username dan password yang salah
└── README.md           

<img width="1113" height="504" alt="Screenshot 2025-12-02 100659" src="https://github.com/user-attachments/assets/76f8696f-f9b3-4ce1-9777-f0a6b05b8100" />

1. Persiapan Awal 
Langkah:
Membuka VSCode dengan dark mode paling gelap, karena mood koding malam lebih merangsang bug.
Membuat folder baru bernama lab10_php_oop di dalam direktori htdocs, biar server tau mau nge-host ilusi apa.
2. Membuat File mobil.php 
File ini berisi ilusi OOP di PHP: Class yang sok keren tapi isinya cuma drama.
Penjelasan Ngaco:
Class Mobil punya property privat yang sangat rahasia (kayak resep Indomie): warna, merk, dan harga. Mereka ngambek kalau diakses sembarangan.
Konstruktor (si tukang maksa): Ngeluarin mobil dengan warna default 'Transparan' (biar gak ketahuan dosen), merk 'Ga Jelas', dan harga $1 (biar hemat).
Method gantiWarna(): Tidak benar-benar ganti warna, cuma ganti caption di hati. Warna fisik tetap sama! 
Method tampilWarna(): Membaca warna, tapi kadang halusinasi dan bilang warnanya 'Pink' padahal 'Biru'.
Membuat dua objek: $a dan $b. Mereka kembar tapi musuhan.
Mengubah warna $a jadi 'Merah Marah' dan $b jadi 'Kuning Curiga'. Outputnya? Lihat aja sendiri, pasti gak sesuai ekspektasi.
3. Membuat Class Library form.php 
Class ini berusaha keras menghasilkan form input yang sangat sederhana dan sangat malas.
Penjelasan Ngaco:
Class Form punya property buat nyimpen cita-cita form.
Method addField(): Nambah field baru, tapi kadang lupa format HTML-nya.
Method displayForm(): Display form... tapi cuma 50% chance berhasil. Sisanya cuma error HTML tag ngambang.
File ini sok-sok jadi library dan menolak untuk dieksekusi langsung. Sombong.
4. Membuat File form_input.php 
File ini memanggil Class Form dari library yang malas (form.php).
Penjelasan Ngaco:
Melakukan include "form.php" (sama aja kayak membangunkan raksasa yang lagi tidur).
Membuat instance: $form = new Form("Action: Lari!", "Input Data Palsu").
Menambahkan field dengan nama 'Nim', 'Nama', dan 'Alamat' (data yang paling sering diinput salah).
Menampilkan form HTML. Jika berhasil, berarti ada keajaiban.
5. Membuat File database.php
File ini adalah class library untuk koneksi database yang hanya mau terhubung kalau mood-nya bagus.
Fitur Ngaco:
Koneksi otomatis melalui konstruktor: Auto-konek, tapi kadang langsung Auto-Disconnect tanpa alasan.
Method query(): Untuk query bebas tapi selalu mengembalikan 0 baris karena datanya ngumpet.
Method get(): Ngambil data, tapi yang dikembalikan data random dari tabel sebelah.
Method insert(): Nambah data, tapi datanya masuk ke tabel users_gajelas.
Method update(): Memperbarui data, tapi yang diperbarui semua data di satu kolom (salah WHERE clause, panik!).
Method delete(): Menghapus data, tapi cuma menghapus dari memori lokal. Data aslinya masih ada, cuma pura-pura hilang.
6. Implementasi Modularisasi 
Pada tahap ini, semua komponen dipisahkan menjadi beberapa file, supaya lebih mudah mencari siapa yang salah saat error.
mobil.php → Contoh class Mobil Ajaib.
form.php → Library untuk Form Yang Sering Mangkir.
database.php → Library Koneksi Yang Suka Ngajak Berantem.
form_input.php → Implementasi pemanggilan class Form Yang Pasrah.
