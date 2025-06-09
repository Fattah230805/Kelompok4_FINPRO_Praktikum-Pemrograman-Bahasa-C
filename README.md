# Kelompok4_FINPRO_Praktikum-Pemrograman-Bahasa-C

# Documentation 

#### File main.c

 > - **file_ada()** : Berguna untuk membatasi pembuatan header di file handling sehingga hanya membuat header sekali saja. function ini akan digunakan di simpan_pasien_terakhir_ke_file().

 > - **simpan_pasien_terakhir_ke_file()** : Berguna untuk menambahkan data pasien terbaru ke file **data_pasien.txt** setelah user selesai memasukkan input untuk data pasien tersebut.

 > - **simpan_semua_ke_file()** : Digunakan ketika user ingin mengubah salah satu data pasien sehingga ketika sudah diubah, program akan melakukan overwrite untuk mengganti data pasien yang lama di file dataset dengan data pasien yang baru.

 > - **muat_dari_file()** : Berguna untuk membaca file data_pasien sehingga bisa digunakan di program untuk mengubah, menambah , atau menampilkan data pasien di program.

 > - **cari_index_id()** :Berguna untuk mencari data pasien tertentu berdasarkan ID untuk ditampilkan atau diubah

> - **tampilkan_risiko()** : Menampilkan tingkat risiko terkena penyakit diabetes (Normal/rendah/sedang/berat) berdasarkan skor total.

> - **tampilkan_tabel_pasien()** : Menampilkan data pasien yang dibaca dari file data_pasien dalam bentuk tabel.

> - **muat_id_terakhir_dari_file()** : Berguna untuk memastikan setiap dibuat data pasien baru, ID yang dihasilkan untuk setiap data pasien tidak mulai dari satu, tetapi melanjutkan dari data pasien terakhir yang ada di file data_pasien .

> - **main()** : function utama dari seluruh program, berguna untuk membuat tampilan menu danmemanggil semua function yang sudah dibuat. 


#### File Input.c

> - **Struct gejala** : tempat untuk menyimpan input user untuk tingkat keparahan setiap gejala.

> - **Struct pasien** : tempat untuk menyimpan data pasien hasil dari dari input user yaitu terdiri dari nama,id,gender,umur, struct gejala, berat badan awal dan akhir, dan hasil lab (HbA1C dan glukosa).

> - **buat_id_pasien()** : berguna untuk membuat ID untuk setiap data pasien yang ada untuk menjadi penanda setiap data pasien.

> - **input_gejala_valid()** : berguna untuk mengambil input gejala dan mengecek apakah input oleh user untuk tingkat keparahan gejala valid atau tidak.

> - **inputPasien()** : berguna untuk mengambil input seluruh isi dari data pasien dan untuk input gejala akan memanggil function input_gejala_valid().

#### File LogikaSkoring.c

> - **enum risiko** : tempat untuk menyimpan tingkat risiko terkena penyakit (normal/rendah/sedang/tinggi).

> - **hitung_berat_badan()** : Melakukan skoring berat badan berdasarkan penurunan berat badan dengan mengurangi berat_badan_akhir dengan berat_badan_awal.

> - **hitung_HbA1c()** : Melakukan skoring risiko  berdasarkan input HbA1c dari user.

> - **hitung_glukosa()** : Melakukan skoring risiko  berdasarkan input glukosa dari user.

> - **hitung_umur()** : Melakukan skoring risiko  berdasarkan input umur dari user.

> - **hitung_gejala()** : Melakukan skoring risiko  berdasarkan input setiap gejala dari user.

> - **total_skoring()** : Menghitung total skor risiko dari skor total risiko dari gejala, skor risiko dari hasil lab (HbA1c dan glukosa), skor risiko dari penurunan berat badan, dan skor risiko dari umur dan menentukan tingkat risiko berdasarkan dari total tersebut.

> - **total_skoring_pasien()** : Memanggil semua function skoring yang ada file ini di dalam satu function sehingga di dalam function tersebut dilakukan semua penghitungan . Ketika berada di file main.c hanya perlu memanggil function ini saja.



