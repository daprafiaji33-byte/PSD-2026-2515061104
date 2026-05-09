# Sistem Pencari Nama Mahasiswa dalam database Universitas
Sistem ini berfungsi untuk mencari nomor dari daftar nama yang sudah dimiliki dengan cara memasukan/inputkan sebuah nama yang ingin dicari.

<img width="1143" height="828" alt="Screenshot 2026-05-08 192240" src="https://github.com/user-attachments/assets/81c373f5-e19f-4066-ae31-28ea2a0f1c6a" />

<img width="1150" height="295" alt="Screenshot 2026-05-08 192309" src="https://github.com/user-attachments/assets/4f62c551-53d0-440e-af4e-e7c006b4df3e" />

Baris 10: Membuat fungsi binary_search untuk mencari data di dalam list yang sudah terurut.

Baris 11: Menentukan batas kiri (l) pencarian, dimulai dari indeks 0.

Baris 12: Menentukan batas kanan (r) pencarian, yaitu jumlah data dikurangi satu.

Baris 13: Menyiapkan variabel pos dengan nilai -1 sebagai tanda jika data belum ditemukan.

Baris 14: Melakukan perulangan selama batas kiri tidak melewati batas kanan.

Baris 15: Menghitung titik tengah (m) atau median dari jangkauan pencarian saat ini.

Baris 16: Mencetak indeks median dan nilai yang ada di titik tersebut untuk memantau proses.

Baris 17: Mengecek apakah nilai di titik tengah sama dengan nama yang dicari (target).

Baris 18-19: Jika cocok, simpan posisi indeksnya ke pos dan hentikan pencarian (break).

Baris 20: Mengecek apakah nilai di tengah lebih kecil dari nama yang dicari.

Baris 21-22: Jika lebih kecil, berarti target ada di sebelah kanan, maka batas kiri berpindah ke kanan median.

Baris 23: Jika nilai di tengah lebih besar dari nama yang dicari.

Baris 24-25: Berarti target ada di sebelah kiri, maka batas kanan berpindah ke kiri median.

Baris 26: Mengembalikan hasil akhir berupa indeks posisi atau -1 jika tidak ketemu.

Fungsi Utama dan Input dari nama yang ingin dicari

Baris 29: Membuat fungsi main sebagai pusat jalannya program.

Baris 30: Menentukan jumlah elemen dalam list (n = 7).

Baris 31: Daftar nama yang sudah diurutkan tergantung dari urutan alfabet yang ada di nama tersebut.

Baris 32: Menampilkan seluruh daftar nama ke layar.

Baris 33: Melakukan perulangan while True untuk validasi input.

Baris 34-35: Meminta pengguna memasukkan nama yang ingin dicari.

Baris 36: Mengubah input nama menjadi format Title Case (huruf kapital di awal) agar cocok dengan isi list.

Baris 37: Keluar dari loop input jika data sudah dimasukkan dengan benar.

Baris 38-39: Jika terjadi kesalahan input, tampilkan peringatan untuk tidak menggunakan angka/karakter unik.

Baris 40: Memanggil fungsi binary_search untuk mencari posisi nama tersebut.

Baris 41: Mengecek apakah variabel pos bukan -1, yang artinya data ditemukan karena nilai -1 sudah digantikan.

Baris 42: Menampilkan nomor urut penemuan (indeks + 1 karena biasanya penomoran dimulai dari nomor 1 sedangkan indeks 0).

Baris 43-44: Jika pos tetap -1, tampilkan pesan bahwa nama tidak ditemukan.

Baris 47-48: Menjalankan fungsi main() jika file ini adalah program utama yang dibuka.

# Output

<img width="874" height="120" alt="Screenshot 2026-05-08 194102" src="https://github.com/user-attachments/assets/11eaf8a2-1d99-4e80-b42a-6ec5d068f3c3" />
Output program ini menampilkan data yang ada, lalu memunta nama yang ingin dicar. Setelah user menginputkan nama maka sistem akan berjalan sesuai dengan logika yang ada. Terakhir sistem akan menampilkan hasil dari pencarian yang akan menampilkan nomer dari nama tersebut jika nama yang di cari ada di data, dan akan menampilkan "data tidak ditemukann" jika nama tersebut tidak ada di dalam data.

# Link Youtube
https://youtu.be/hQXf5v1Z4oU
