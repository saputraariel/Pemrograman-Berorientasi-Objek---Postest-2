# Pemrograman-Berorientasi-Objek-Postest-2

TEMA : Sistem Manajemen ALat2 Musik Tradisional

Mohamad Ariel Saputra D Loi

Sistem Informasi C 2024

2409116087

## Penjelasan Program

Pnjelasan Sinngkat Dari Program CRUD yang saya buat, dengan tema saya "Sistem Manajemen Alat2 Musik Tradisional"

## Class Main

<img width="849" height="260" alt="image" src="https://github.com/user-attachments/assets/828dc2c8-02ba-48f6-b6e2-6bf8398e57d0" />

Bagian ini adalah pembuka program. Pertama dibuat objek Scanner untuk membaca input dari pengguna, objek Service untuk mengakses logika pengolahan data. dan menyiapkan Variabel pilihan untuk menampung peng inputan angka menu yang dipilih.

<img width="901" height="305" alt="image" src="https://github.com/user-attachments/assets/a3bc5701-94ee-4a1c-8e60-965181df4aa3" />

Bagian ini untuk menampilkan output dari setiap pilihan untuk memudahkan pengguna tau, jika dia meng inputkan nomor ini untuk masuk ke bagian tertentu.

<img width="835" height="373" alt="image" src="https://github.com/user-attachments/assets/cb5fe5bf-f4e3-4691-b648-68a0e06e6163" />

Bagian terakhir berisi pengendalian menu menggunakan switch-case. Setiap pilihan akan memanggil method yang sesuai dari class Service. Program hanya berhenti jika pengguna memilih angka 0.

## Class Model

<img width="490" height="201" alt="image" src="https://github.com/user-attachments/assets/65157b37-2b5f-494f-b09e-3b82a71ffe40" />

Bagian awal ini mendefinisikan atribut dari class Model, yaitu nama, daerahAsal, dan tahunPembuatan. Atribut dibuat private supaya tidak bisa terakses public jadi hanya di class itu saja.

<img width="985" height="194" alt="image" src="https://github.com/user-attachments/assets/e2f49065-49ba-4385-ac5a-0fea24c58a17" />

membuat objek Model baru dengan langsung memberikan nilai awal pada ketiga atribut.ini untuk mempermudah saat menambahkan data alat musik baru.

<img width="800" height="659" alt="image" src="https://github.com/user-attachments/assets/d5d265a4-f1b9-4b2e-ad7c-f3ef42737e45" />

Bagian ini berisi getter dan setter yang digunakan untuk mengakses atau mengubah nilai dari atribut secara aman tanpa melanggar enkapsulasi.

<img width="1036" height="154" alt="image" src="https://github.com/user-attachments/assets/b8c4efd3-18f6-4c12-bb0d-0a010bcb4331" />

Method toString() dipakai untuk mengubah objek Model menjadi bentuk teks yang lebih mudah dibaca ketika ditampilkan ke layar.

## Class Service

<img width="873" height="229" alt="image" src="https://github.com/user-attachments/assets/935726b9-4cb5-4c5d-98da-29851e2247f9" />

Bagian awal ini mendeklarasikan daftarAlat sebagai list penyimpan semua data alat musik, serta Scanner untuk membaca input dari pengguna

<img width="972" height="189" alt="image" src="https://github.com/user-attachments/assets/28e05244-ed26-4d47-ba12-553a0200ad17" />

Constructor pada class Service berfungsi untuk mengisi daftarAlat dengan beberapa data awal, sehingga program tidak kosong saat pertama kali dijalankan.

<img width="896" height="343" alt="image" src="https://github.com/user-attachments/assets/77776e18-2004-4662-94f7-e4ace069430b" />

Method tambahAlat() digunakan untuk menambahkan data baru ke dalam list. Program akan meminta input nama, daerah asal, dan tahun pembuatan dari pengguna

<img width="989" height="310" alt="image" src="https://github.com/user-attachments/assets/2279a558-61f7-4de3-b436-0180b84c9005" />

Method tampilkanAlat() berfungsi menampilkan semua data alat musik yang ada dalam list. Jika list kosong, maka akan muncul pesan bahwa tidak ada data.

<img width="1046" height="611" alt="image" src="https://github.com/user-attachments/assets/04b6dd9c-6b43-4022-80af-e95b4b9c3821" />

Method editAlat() dipakai untuk memperbarui data yang sudah ada. Pengguna memilih nomor data, lalu memasukkan nilai baru yang akan menggantikan data lama.

<img width="994" height="403" alt="image" src="https://github.com/user-attachments/assets/01d069ef-93a7-44e0-a3ed-713dc3e5de85" />

Method hapusAlat() digunakan untuk menghapus data dari list berdasarkan nomor yang dipilih pengguna.

<img width="1045" height="508" alt="image" src="https://github.com/user-attachments/assets/656ab54f-08e1-4302-995e-6e838f2310d4" />

Method cariAlat() digunakan untuk mencari data berdasarkan nama atau daerah asal dengan menggunakan kata kunci tertentu. Jika ada kecocokan, data akan ditampilkan; jika tidak, akan muncul pesan bahwa data tidak ditemukan.

## Penjelasan Alur Programa

Program dimulai dari Main.java dengan menampilkan menu utama secara berulang menggunakan perulangan do-while. Pengguna memasukkan pilihan menu, kemudian program memanggil method pada class Service sesuai input.

  -Jika memilih 1, program menjalankan tambahAlat() untuk menambah data baru.

  -Jika memilih 2, program menjalankan tampilkanAlat() untuk menampilkan seluruh data.

  -Jika memilih 3, program menjalankan editAlat() untuk mengubah data yang sudah ada.

  -Jika memilih 4, program menjalankan hapusAlat() untuk menghapus data.

  -Jika memilih 5, program menjalankan cariAlat() untuk mencari data berdasarkan nama atau daerah asal.

Proses ini terus berulang hingga pengguna memilih 0 untuk keluar, kemudian program berhenti dan menutup scanner.

<img width="960" height="344" alt="alur_program" src="https://github.com/user-attachments/assets/79aaf1cc-8209-4909-bfb3-e43dab525343" />
