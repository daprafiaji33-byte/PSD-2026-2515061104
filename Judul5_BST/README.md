# Program untuk mendata ruangan kelas pada perkuliahan
Sistem ini merupakan sistem yang dapat digunakan oleh admn untuk mendata ruangan mana sajakah yang sedang digunakan dan yang sedang kosong, sistem ini dapat menambahkan ruangan yang ingin dipakai dan menghapus ruangan yang telah dipakai. Bisa juga untuk menampilkan ruangan terpakai, mencari ruangan terdekat baik di kanan maupun di kiri.

<img width="1626" height="878" alt="Screenshot (6)" src="https://github.com/user-attachments/assets/691895c5-fa94-4872-9475-0374b8493be9" />
<img width="1637" height="838" alt="Screenshot (7)" src="https://github.com/user-attachments/assets/9e5c2a13-a916-4b22-b9dc-d857d0d1c3c5" />
<img width="1640" height="795" alt="Screenshot (8)" src="https://github.com/user-attachments/assets/37aecf54-1edc-46e6-836f-7237441d4b02" />
<img width="1638" height="832" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/fde0a73d-3a10-433d-ab47-6e0e5c4a47dc" />
<img width="1616" height="835" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/3ea02a49-e12e-401f-997c-93dac17fbe21" />
<img width="1634" height="832" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/a12cc849-544f-4520-9d74-13ddc9ffb0b0" />

Baris 10: Membuat class Node, isinya key dimana berupa nomor inputan, serta left (nomor lebih kecil) dan right (nomor lebih besar).

Baris 17: Membuat class BSTLanjutan sebagai pengelola utama sistem pohon.

Baris 21: Fungsi insert_node untuk menentukan di mana posisi ruangan baru harus diletakkan. 

Baris 25-27: kalau nomor ruangan baru lebih kecil, arahkan ke cabang kiri, kalau lebih besar arahkan ke cabang kanan. Kalau nomornya sama (else), berarti ruangan tersebut sudah terdaftar/terpakai.

Baris 33: Fungsi insert untuk memastikan hanya nomor ruangan 1-20 saja yang bisa didaftarkan.

Baris 38: Fungsi find_min_node untuk mencari nomor ruangan paling kecil.

Baris 45: Fungsi delete_node untuk menghapus ruangan. kalau ada ruangan yang dihapus yang memiliki node anak, anak tersebut yang akan menggantikan posisi ruangan yang dihapus.

Baris 68: Fungsi find_successor untuk mencari ruangan terdekat yang nomornya lebih besar dari nomor yang dicari.

Baris 87: Fungsi find_predecessor untuk mencari ruangan terdekat yang nomornya lebih kecil dari nomor yang dicari.

Baris 108: Fungsi inorder untuk menampilkan daftar nomor yang sudah ada di bst, diurutkan dari nomor terkecil ke terbesar.

Baris 116: Menyiapkan menu program: (1) Tambah, (2) Hapus, (3) Tampilkan, (4) Cari ruangan lebih besar, atau (5) Cari ruangan lebih kecil .

Baris 132: Jika user pilih menu 1, program minta input nomor ruangan dan menambahkannya ke sistem.

Baris 139: Jika user pilih menu 2, program menghapus nomor ruangan yang sudah selesai dipakai.

Baris 149: Jika user pilih menu 3, program menampilkan daftar ruangan yang aktif pakai fungsi inorder.

Baris 153-172: Jika user pilih menu 4 atau 5, program menjalankan fungsi find_successor atau find_predecessor untuk menemukan  ruangan yang kosong atau terdekat. Kalau 4 untuk yang ada di kanan/lebih besar dan kalau 5 untuk ruangan yang ada di kiri/lebih kecil

Baris 173-174 : jika user memilih 6, maka program akan berhenti, karena diatas ada while != 6, jadi ketika memilih 6 program akan berhenti

Baris 175-176 : Akan berjalan ketika user memilih angka selain 1-6, dan menampilkan pilihan tidak valid

Baris 179-180 : untuk memastikan def main tetap berjalan

# Output
<img width="1920" height="1080" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/12c0132d-1f5a-4491-b426-60f4e88532a4" />
Seperti yang kta lihat disini, pengguna itu dapat memilih hal apa yang ingin dilakukan oleh sistem, seperti menambahkan, menghapus, menampilkan ruanganyang tersisa, dan mencari ruangan terdekat di bagian kanan maupun kiri.

# LINK YOutube
https://youtu.be/C6tCIsr4B1M?si=fiCM5TKhtaMuJSAO
