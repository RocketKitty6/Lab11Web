# Pemograman Web
~~~
Nama  : Galang Rintang Widya Pratama
NIM:  : 312010299
Kelas : TI.20.B.2
~~~

## Praktikum 11: PHP Framework (Codeigniter)

### Buat folder baru lab11_php_ci lalu Jalankan XAMPP Ubah file php.ini seperti berikut :

![image](https://user-images.githubusercontent.com/101440705/176886927-c5e6a39d-7a39-4c36-bffa-af16c25727c5.png)

![image](https://user-images.githubusercontent.com/101440705/176887466-e28ede1e-74e8-452e-9064-3e3b359a4fb6.png)

### Instal Codeigniter 4 simpan pada htdocs dan Buka http://localhost/lab11_php_ci/ci4/public/ , hasilnya :

![image](https://user-images.githubusercontent.com/101440705/177772156-4aaa6b7f-3cbc-4f60-89b1-108bf90bdd3c.png)

### Buka cmd pada XAMPP Shell lalu buka php spark, untuk menjalankan server ketik "php spark serve" :

![image](https://user-images.githubusercontent.com/101440705/177773157-a3172f14-de75-4213-99bc-e56e0f8579b7.png)

Hasil error/kesalahan

![image](https://user-images.githubusercontent.com/101440705/177773240-5dd17831-0e33-486c-893f-c24024267ae8.png)

### Mengaktifkan mode Debugging dengan mengubah file .env menjadi = development, seperti berikut :

![image](https://user-images.githubusercontent.com/101440705/177773282-392e3f35-b7bc-40cc-a683-454e5d4813c8.png)

### Untuk mencoba Error hilangkan tanda ; (titik koma) pada Home.php, seperti berikut :

![image](https://user-images.githubusercontent.com/101440705/177773319-2787b0c3-e2c9-4eed-8414-e188c0cffd96.png)

Contoh error/kesalahan akan ditampilkan secara detail

![image](https://user-images.githubusercontent.com/101440705/177773099-c6820112-b7f3-4b9f-9a4f-ac26e7c0a537.png)

### Mengarahkan router pada controller, kemudian Membuat Route Baru Tambahkan kode berikut pada Route.php :

![image](https://user-images.githubusercontent.com/101440705/177773550-3857f51b-f272-4286-9bba-84546cf03413.png)

### Cek pada CMD dengan memasukan "php spark routes", Akses route yang telah dibuat dengan http://localhost:8080/about, hasilnya :

![image](https://user-images.githubusercontent.com/101440705/177773817-0c12dbfe-9b26-4a05-a538-67e8126c673b.png)

### Membuat Controller Page, dengan membuat file baru bernama page.php seperti berikut :

![image](https://user-images.githubusercontent.com/101440705/177774404-e54f8575-9308-48c2-aa0a-fb88587b2580.png)

### Mengaktifkan AutoRouting dengan men set nilai true/false, jika true maka fungsi akan aktif

![image](https://user-images.githubusercontent.com/101440705/177774513-d2596dac-853d-4a12-b2fb-d46fff21a832.png)

### Tambahkan method baru pada Controller Page seperti berikut untuk page Term of Services

![image](https://user-images.githubusercontent.com/101440705/177774633-347d4208-c7fc-48e7-80b7-9ea9c2ed17e0.png)

### Membuat View, dengan membuat file baru bernama about.php dan masukan kode berikut :

![image](https://user-images.githubusercontent.com/101440705/177775281-fe4899eb-73ab-4564-8f42-df3c3512f738.png)

Ubah method about pada class Controller Page menjadi seperti berikut:

![image](https://user-images.githubusercontent.com/101440705/177775356-eafa661d-8dd2-470e-81fc-5d1b652dbf4d.png)

### Membuat Layout Web dengan CSS
Buat file css pada direktori public dengan nama style.css

![image](https://user-images.githubusercontent.com/101440705/177775506-855960d9-acfb-4884-ab83-eafa404cf36a.png)

Kemudian buat folder template pada direktori view kemudian buat file header.php dan footer.php

`header.php`

![image](https://user-images.githubusercontent.com/101440705/177775774-48cc544b-fecf-476c-8940-d573fcf44149.png)

`footer.php`

![image](https://user-images.githubusercontent.com/101440705/177775832-047de56e-b8ae-4e21-b0d1-38ba0d114e83.png)

Kemudian ubah file app/view/about.php seperti berikut

![image](https://user-images.githubusercontent.com/101440705/177776008-75c1d125-ed79-4e25-b1ba-c1192f07bf34.png)

Selanjutnya refresh tampilan pada alamat http://localhost:8080/about

![image](https://user-images.githubusercontent.com/101440705/177776096-01e8f033-d97c-4d7d-aab3-d2fb4d7aca94.png)

## Pertanyaan dan Tugas
Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga semua link pada navigasi header dapat menampilkan tampilan dengan layout yang sama.

Tambahkan kode berikut di dalam Routes.php

![image](https://user-images.githubusercontent.com/101440705/177776256-7309aa15-c318-4723-bd18-c5162b91dbb3.png)

edit page control pada page.php

![image](https://user-images.githubusercontent.com/101440705/177776649-0b174964-0bc6-4420-ab93-faf3b9371c75.png)

Buat file artikel.php dan contact.php pada direktori app/view/.....

![image](https://user-images.githubusercontent.com/101440705/177776927-308eb1d0-4d04-473a-9c65-4a273138437b.png)

![image](https://user-images.githubusercontent.com/101440705/177777122-b599d472-ded9-4615-bc62-2c551269348e.png)

saat kita membuka halaman artikel dan kontak maka tampilan akan menuju page artikel dan kontak

![image](https://user-images.githubusercontent.com/101440705/177777282-e29ef130-7e54-437c-85fd-078ea8d47223.png)

![image](https://user-images.githubusercontent.com/101440705/177777330-6d0a56b9-9ecc-42db-927d-e20caa9a38e1.png)

================================================================================================================================================
## Praktikum 12: Framework Lanjutan (CRUD)

### Jalankan MySQL pada program XAMPP berjalan dan buat database seperti berikut :

![ss 1](img/ss11-1.PNG)

### Mengkonfigurasi koneksi database pada file .env seperti berikut :

![ss 1](img/ss11-2.PNG)

### Membuat file Model pada direktori app/Models dengan nama ArtikelModel.php seperti berikut :

![ss 1](img/ss11-3.PNG)

### Membuat file Controller baru dengan nama Artikel.php pada direktori app/Controllers. seperti berikut :

![ss 1](img/ss11-4.PNG)

### Membuat file Views baru dengan nama artikel pada direktori app/views, kemudian buat filebaru dengan nama index.php, seperti berikut 

![ss 1](img/ss12-1.PNG)

Jalankan server dan akses link : http://localhost:8080/artikel

![ss 1](img/ss12-2.PNG)

### Masukan data berikut pada database :

![ss 1](img/ss12-3.PNG)

Refresh dan lihat kembali browser :

![ss 1](img/ss12-4.PNG)

### Menambahkan Detail pada Artikel.php seperti berikut :

![ss 1](img/ss13.PNG)

### Membuat file baru baru untuk halaman detail dengan nama app/views/artikel/detail.php. seperti berikut :

![ss 1](img/ss13-1.PNG)

### Tambahkan rute baru pada Routes.php :

![ss 1](img/ss13-2.PNG)

Tampilan Artikel setelah di Klik :

![ss 1](img/ss13-3.PNG)

### Membuat Menu Admin

Buat method baru pada Controller Artikel dengan nama admin_index() :

![ss 1](img/ss14-1.PNG)

Buat file baru dengan nama admin_index.php pada folder artikel :

![ss 1](img/ss14-2.PNG)

Tambahkan Routing baru pada Routes.php seperti berikut :

![ss 1](img/ss14-3.PNG)

Akses menu admin dengan url http://localhost:8080/admin/artikel :

![ss 1](img/ss14-4.PNG)

### Menambah Data Artikel

Tambahkan fungsi/method baru pada Controller Artikel dengan nama add() :

![ss 1](img/ss15-1.PNG)

Lalu buat file baru dengan nama form_add.php pada folder artikel :

![ss 1](img/ss15-2.PNG)

tampilan saat klik artikel :

![ss 1](img/ss15-3.PNG)

### Mengubah DAta Artikel

Tambahkan fungsi/method baru pada Controller Artikel dengan nama edit() :

![ss 1](img/ss16-1.PNG)

Lalu buat file baru dengan nama edit_add.php pada folder artikel :

![ss 1](img/ss16-2.PNG)

Tampilan saat mengubah artikel :

![ss 1](img/ss16-3.PNG)

### Menghapus Data

Tambahkan fungsi/method baru pada Controller Artikel dengan nama delete() :

![ss 1](img/ss17-1.PNG)

=================================================================================

## Praktikum 13: Framework Lanjutan (Modul Login)

### Membuat Tabel: User Login

![ss 1](img/ss18-1.PNG)

### Membuat Model User
Selanjutnya adalah membuat Model untuk memproses data Login. Buat file baru pada direktori app/Models dengan nama UserModel.php

![ss 1](img/ss19-1.PNG)

### Membuat Controller User
Buat Controller baru dengan nama User.php pada direktori app/Controllers. kemudian tambahkan fungsi index() sebagai berikut :

![ss 1](img/ss19-2.PNG)

![ss 1](img/ss19-3.PNG)

### Membuat View Login
Buat direktori baru dengan nama user pada direktori app/views, kemudian buat file baru dengan nama login.php. Dengan kode berikut 

![ss 1](img/ss19-4.PNG)

### Membuat Database Seeder
Buka CLI dan masukan kode "php spark make:seeder UserSeeder", Hasilnya :

![ss 1](img/ss20-1.PNG)

Lalu buka file UserSeeder.php yang berada di lokasi direktori /app/Database/Seeds/UserSeeder.php kemudian isi dengan kode berikut

![ss 1](img/ss20-2.PNG)

Selanjutnya buka kembali CLI dan ketik perintah "php spark db:seed UserSeeder" , Hasilnya :

![ss 1](img/ss20-3.PNG)

Hasilnya

![ss 1](img/ss20-4.PNG)

### Menambahkan Auth Filter
Selanjutnya membuat filer untuk halaman admin. Buat file baru dengan nama Auth.php pada direktori app/Filters. berikut :

![ss 1](img/ss21-1.PNG)

Selanjutnya buka file app/Config/Filters.php tambahkan kode berikut:

![ss 1](img/ss21-2.PNG)

Selanjutnya buka file app/Config/Routes.php dan sesuaikan kode berikut :

![ss 1](img/ss21-3.PNG)

### Percobaan menu akses LOGIN
Buka url dengan alamat http://localhost:8080/admin/artikel ketika alamat tersebut diakses maka akan ditarik ke halaman login berikut :

![ss 1](img/ss21-4.PNG)

### Membuat Fungsi LOGOUT
Tambahkan method logout pada Controller User seperti berikut :

![ss 1](img/ss22.PNG)


=================================================================================

## Praktikum 14: Pagination dan Pencarian

### Membuat Pagination
Untuk membuat pagination, buka Kembali Controller Artikel, kemudian modifikasi kode pada method admin_index seperti berikut

![ss 1](img/ss23-1.PNG)

Kemudian buka file views/artikel/admin_index.php dan tambahkan kode berikut dibawah deklarasi tabel data

![ss 1](img/ss23-2.PNG)

Selanjutnya buka kembali menu daftar artikel, tambahkan data lagi untuk melihat hasilnya.

![ss 1](img/ss23-3.PNG)

### Membuat Pencarian
Untuk membuat pencarian data, buka kembali Controller Artikel, pada method admin_index ubah kodenya seperti berikut

![ss 1](img/ss24-1.PNG)

Kemudian buka kembali file views/artikel/admin_index.php dan tambahkan form pencarian sebelum deklarasi tabel seperti berikut

![ss 1](img/ss24-2.PNG)

Dan pada link pager ubah seperti berikut

![ss 1](img/ss24-3.PNG)

Selanjutnya ujicoba dengan membuka kembali halaman admin artikel, masukkan kata kunci tertentu pada form pencarian.

![ss 1](img/ss24-4.PNG)

### Upload Gambar
Menambahkan fungsi unggah gambar pada tambah artikel. Buka kembali Controller Artikel, sesuaikan kode pada method add seperti berikut

![ss 1](img/ss25-1.PNG)

Kemudian pada file views/artikel/form_add.php tambahkan field input file dan sesuaikan tag form dengan menambahkan ecrypt type seperti berikut

![ss 1](img/ss25-2.PNG)

Ujicoba file upload dengan mengakses menu tambah artikel.

![ss 1](img/ss25-3.PNG)
