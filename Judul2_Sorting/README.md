**Sistem pengurutan besar file dari terkecil hingga terbesar**

Sistem ini berfungsi untuk menyusun urutan file berdasarkan ukuran dari inputan user, sistem ini memungkinkan user untuk menentukan akan ada berapa file yang ingin dimasukkan, lalu user dapat memasukan ukuran dari setiap file yang ada, lalu sistem akan secara otomatis mengatuurutan file tersebut dari yang terkecil hingga yang terbesar.

<img width="917" height="826" alt="Screenshot 2026-05-03 122851" src="https://github.com/user-attachments/assets/db0c7041-4492-4789-9752-1888e4488192" />
<img width="918" height="285" alt="Screenshot 2026-05-03 122911" src="https://github.com/user-attachments/assets/daab0f00-38c7-4302-8415-371a83585abc" />

Baris 10: Membuat fungsi tukar, gunanya untuk memindahkan posisi dua angka dalam list.

Baris 11: Menyimpan nilai sementara dari angka pertama ke variabel temp.

Baris 12: Mengisi posisi angka pertama dengan nilai dari angka kedua.

Baris 13: Mengisi posisi angka kedua dengan nilai yang tadi disimpan di temp.

Fungsi diatar memiliki fungsi sebaagi penukar antara satu list dengan list lainnya. Menambahkan variable temp berfungsi sebagai penyimpan sementara suatu list sebelum dimasukkan ke tempat yang sesuai, hal ini dilakukan karena array hanya dapat menyimpan satu data di setiap tempatnya.

Baris 16: Membuat fungsi bubble_sort untuk mengurutkan list dari yang terkecil ke terbesar.

Baris 17: Perulangan utama (i) untuk menentukan berapa kali pengecekan seluruh list dilakukan dengan n-1.

Baris 18: Perulangan kedua (j) untuk membandingkan angka yang bersebelahan.

Baris 19: Mengecek apakah angka di kiri lebih besar daripada angka di kanannya.

Baris 20: Jika benar lebih besar, maka posisi kedua angka tersebut ditukar menggunakan fungsi tukar.

Baris 23: Membuat fungsi main sebagai jantung jalannya program.

Baris 24: Menggunakan blok try untuk mengantisipasi kesalahan input .

Baris 25: Meminta pengguna memasukkan jumlah file yang ingin dihitung.

Baris 26-28: Jika pengguna tidak memasukkan angka, tampilkan pesan error dan hentikan program.

Baris 29: Menyiapkan list kosong bernama arr untuk menampung ukuran-ukuran file.

Baris 30: Menampilkan instruksi untuk memasukkan besar file dalam satuan KiloByte.

Baris 31: Melakukan perulangan sebanyak jumlah file (n) yang sudah ditentukan tadi.

Baris 32: Menggunakan while True agar program terus bertanya sampai inputnya benar.

Baris 33-34: Meminta input besar file dan mengubahnya menjadi tipe data integer (angka).

Baris 35: Memasukkan angka tersebut ke dalam list arr.

Baris 36: Keluar dari loop while jika input sudah berhasil masuk.

Baris 37-38: Jika input bukan angka, beri peringatan dan minta masukkan ulang.

Baris 39: Menampilkan list ukuran file ke layar sebelum dilakukan pengurutan.

Baris 40: Menjalankan fungsi bubble_sort untuk merapikan urutan angka di dalam list.

Baris 41: Menampilkan string utuk output akhir, menggunakan syntax end agar yang dipanggil selanjutnya menggunakan fungsi print tidak pindah baris.

Baris 42-43: Melakukan perulangan untuk mencetak angka-angka yang sudah urut satu per satu.

Baris 44: Mencetak baris baru agar tampilan terminal lebih rapi.

Baris 47: Mengecek apakah file ini dijalankan sebagai program utama.

Baris 48: Memanggil fungsi main() untuk mulai menjalankan seluruh alur program.

**Output**

<img width="863" height="201" alt="Screenshot 2026-05-03 125321" src="https://github.com/user-attachments/assets/b802d2a8-2b81-4529-bf42-8763c7619ef8" />

Output program ini meiminta user untuk memasukan jumlah data yang aa, lalu sistem akan meminta user untuk menentukan besar ukuran dari setiap file yang diinputkan. Selanjutnya sistem akan melihatkan file dengan urutan sesuai dengan inputan user dan juga akan menampilkan urutan besar file dari terkecil hingga terbesar.

**Link Youtube**
