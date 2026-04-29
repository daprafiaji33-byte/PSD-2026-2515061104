**SISTEM ANTREAN GACOAN**
Program ini berfunsi untuk mendata antrean pelanggan pada restoran gacoan secara digital. Sistem ini memungkinkan petugas untuk menambah pelanggan baru ke dalam antrean, melayani pelanggan berdasarkan urutan pertama yang datang, dan melihat daftar seluruh pasien yang sedang menunggu/mengantre. Program  yang digunakan menggunakan struktur data linked list.


<img width="920" height="828" alt="Screenshot 2026-04-29 201951" src="https://github.com/user-attachments/assets/7c5ec8d7-529c-4f6f-b58b-7bd641973038" />
<img width="983" height="775" alt="Screenshot 2026-04-29 202051" src="https://github.com/user-attachments/assets/75b30b41-eac0-412d-8cd1-67552278c522" />
<img width="976" height="804" alt="Screenshot 2026-04-29 202110" src="https://github.com/user-attachments/assets/e6612706-6cc6-4fa4-81ee-52534eb18ebb" />
<img width="984" height="203" alt="Screenshot 2026-04-29 202125" src="https://github.com/user-attachments/assets/89c0cbf2-5dd3-43ac-9f6b-6d346caa6126" />
Baris 12: Membuat class Node, sebagai cetakan untuk setiap elemen atau orang dalam antrean.

Baris 13: Fungsi awal untuk menyiapkan data saat elemen baru dibuat.

Baris 14: Menyimpan data (nama orang) ke dalam objek tersebut.

Baris 15: Menyiapkan next sebagai penghubung ke orang berikutnya, awalnya kosong (None).

Baris 17: Membuat class LinkedList, pengelola utama yang mengatur alur masuk dan keluar antrean.

Baris 18: Fungsi awal untuk menentukan kondisi awal antrean saat program dijalankan.

Baris 19: Menandai start sebagai posisi paling depan antrean, awalnya kosong.

Baris 20: Menandai rear sebagai posisi paling belakang antrean, awalnya kosong.

Baris 22: Fungsi pembantu untuk membuat objek orang baru (Node) dari nama yang diberikan.

Baris 23: Proses pembuatan objek Node baru di dalam memori.

Baris 24: Mengembalikan hasil pembuatan objek tersebut untuk digunakan fungsi lain.

Baris 26: Fungsi untuk memasukkan orang baru di posisi paling depan (ujung kiri antrean).

Baris 27: Cek apakah antrean masih kosong.

Baris 28-29: Jika kosong, orang baru tersebut menjadi yang paling depan sekaligus paling belakang.

Baris 30: Jika sudah ada isinya.

Baris 31: Orang baru menyambungkan "talinya" ke orang yang saat ini ada di paling depan.

Baris 32: Status "paling depan" berpindah ke orang yang baru masuk tadi.

Baris 34: Fungsi untuk menambah antrean ke urutan paling belakang (urutan normal).

Baris 35: Cek apakah antrean masih kosong.

Baris 36-37: Jika kosong, orang baru menjadi yang pertama (depan) sekaligus terakhir (belakang).

Baris 39: Jika sudah ada isinya, orang di posisi belakang menyambungkan "tali" ke orang baru.

Baris 40: Status "paling belakang" resmi berpindah ke orang yang baru saja datang tersebut.

Baris 42: Fungsi untuk menghapus orang di urutan depan (orang yang selesai dilayani).

Baris 43: Cek apakah antrean sedang kosong.

Baris 44: Jika kosong, tampilkan pesan Underflow!!!.

Baris 46: Mengambil data (nama) orang yang akan dihapus untuk disimpan sementara.

Baris 47: Memindahkan posisi "paling depan" ke orang di belakangnya.

Baris 48: Mencetak pesan konfirmasi bahwa orang tersebut sudah dihapus/dilayani.

Baris 49: Cek jika setelah dihapus, antrean ternyata jadi benar-benar kosong.

Baris 50: Jika kosong, pastikan posisi rear juga ikut dikosongkan (None).

Baris 52: Fungsi untuk menampilkan seluruh daftar orang dalam antrean.

Baris 53: Cek apakah antrean sedang kosong.

Baris 54-55: Jika kosong, cetak tulisan (kosong) dan keluar dari fungsi.

Baris 57: Mulai menelusuri dari orang paling depan (start).

Baris 58: Selama posisi saat ini masih ada orangnya (bukan None).

Baris 59: Mencetak nama orang tersebut dengan tanda panah ->.

Baris 60: Bergeser mengikuti "tali penghubung" ke orang berikutnya.

Baris 61: Mencetak tulisan None untuk menandai akhir dari antrean.

Baris 62: Fungsi main sebagai pusat kendali seluruh program.

Baris 63: Membuat satu sistem antrean nyata dari class LinkedList.

Baris 64: Mencetak judul program "Antrian Gacoan".

Baris 66: Melakukan pengulangan terus-menerus (looping) agar menu selalu muncul.

Baris 67-70: Mencetak pilihan menu 1 sampai 4.

Baris 72: Meminta input angka pilihan dari pengguna.

Baris 74: Jika memilih menu '1' (Tambah antrean).

Baris 75: Meminta input nama orang yang ingin masuk antrean.

Baris 76: Menyiapkan objek orang baru dari nama tersebut.

Baris 77: Cek apakah objek berhasil dibuat.

Baris 78: Memasukkan orang tersebut ke posisi paling belakang.

Baris 79: Menampilkan pesan sukses tambah antrean.

Baris 82: Jika memilih menu '2' (Layanin orang depan).

Baris 83: Cek apakah antrean kosong.

Baris 84: Jika kosong, beri tahu bahwa tidak ada yang bisa dilayani.

Baris 86: Jika ada, jalankan fungsi hapus orang paling depan.

Baris 87: Jika memilih menu '3' (Tampilkan antrean).

Baris 88-89: Mencetak status antrean saat ini menggunakan fungsi display.

Baris 90: Jika memilih menu '4' (Keluar).

Baris 91-92: Mencetak pesan program selesai dan menghentikan perulangan.

Baris 94: Jika input menu salah atau tidak sesuai angka.

Baris 96: Cek jika pilihan bukan tampilkan atau keluar.

Baris 97-98: Otomatis menampilkan sisa antrean setelah aksi tambah atau hapus.

Baris 100: Mengecek apakah file dijalankan sebagai program utama.

Baris 101: Memanggil fungsi main() untuk mulai menjalankan aplikasi.


**OUTPUT**
<img width="686" height="532" alt="Screenshot 2026-04-29 204412" src="https://github.com/user-attachments/assets/3bea619e-7e80-4d50-858c-97a75bf99eb6" />
<img width="671" height="220" alt="Screenshot 2026-04-29 204426" src="https://github.com/user-attachments/assets/58d806c7-b624-4f80-9638-1d111a17896d" />
Output program ini memberikan pilihan kepada pengguna berupa 4 fungsi, dimana fungsi 1 yang memiliki fungsi sebagai menambahkan nama pelanggan ke antrean, fungsi 2 sebagai hapus antrean/ melayani pelanggan paling depan, fungsi 3 sebagai menunjukan/menampilkan antrean yang ada dan fungsi 4 untuk keluaur dari program.


**LINK YOUTUBE**
https://youtu.be/Io6nC1D97kg?si=D6rXB7S__Iai1E72
