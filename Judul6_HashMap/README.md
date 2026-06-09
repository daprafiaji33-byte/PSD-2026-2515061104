# Sistem Kelola Data Buku Perpustakaan
Sistem ini berfungsi untuk mendata buku perpustakaan secara digital menggunakan metode Separate Chaining untuk menangani tabrakan data data pada Hash Map. Sistem ini memungkinkan petugas untuk menambahkan data buku baru, mencari buku berdasarkan kode uniknya, menghapus buku yang sudah tidak terpakai, serta menampilkan seluruh struktur penyimpanan beserta daftar buku yang sedang tersimpan di dalam perpustakaan. 
<img width="3676" height="12132" alt="image" src="https://github.com/user-attachments/assets/3e04de52-0b48-4740-9d83-1c0b2dc1728d" />

(Class Node)
Baris 10: Membuat class Node yang berfungsi sebagai cetakan dasar untuk menyimpan data buku dalam bentuk simpul penghubung (linked list).

Baris 11: Membuat fungsi inisialisasi __init__ untuk menyiapkan data awal setiap kali ada objek buku baru yang dibuat.

Baris 12: Menyimpan nilai kode buku ke dalam variabel self.key sebagai identitas unik pencarian.

Baris 13: Menyimpan nama atau judul buku ke dalam variabel self.value sebagai informasi isi dari buku tersebut.

Baris 14: Menyiapkan variabel penunjuk self.next yang awalnya diatur kosong (None) untuk menghubungkan ke buku selanjutnya jika terjadi tabrakan data (collision).

Class HashMapSeparateChaining
Baris 17: Membuat class HashMapSeparateChaining sebagai sistem utama untuk mengatur penyimpanan data buku dengan metode rantai terpisah.

Baris 18: Membuat fungsi awal __init__ untuk menentukan ukuran tabel hash saat pertama kali sistem perpustakaan diaktifkan.

Baris 19: Menentukan variabel ukuran kapasitas tabel hash self.SIZE yang diatur bawaannya bernilai 10 slot.

Baris 20: Bikin list atau array bernama self.table sebanyak jumlah SIZE yang semua slotnya diisi dengan nilai kosong None.

Baris 22: Membuat fungsi hash_function untuk menghitung dan menentukan di indeks nomor berapa data buku akan disimpan.

Baris 23: Mengembalikan hasil perhitungan matematika dari rumus operasi sisa bagi (modulo) kode buku dengan ukuran tabel agar indeksnya selalu valid.

Operasi Tambah Data Buku (Insert)
Baris 25: Membuat fungsi insert untuk memasukkan data kode buku beserta judul buku baru ke dalam tabel sistem.

Baris 26: Memanggil fungsi hash untuk mendapatkan nomor indeks lokasi penyimpanan berdasarkan kode buku yang diinput.

Baris 27: Membuat variabel acuan bernama current untuk memantau isi data pada slot indeks tabel tersebut.

Baris 28: Melakukan perulangan while untuk mengecek seluruh simpul buku yang terhubung di slot indeks tersebut selama posisinya tidak kosong.

Baris 29: Mengecek apakah kode buku yang mau dimasukkan ternyata sudah pernah terdaftar sebelumnya di dalam slot tersebut.

Baris 30: Memperbarui judul buku lama dengan judul buku baru yang dimasukkan jika kodenya terbukti sama (update data).

Baris 31: Keluar dari fungsi insert karena proses pembaruan data buku duplikat telah selesai dikerjakan.

Baris 32: Menggeser variabel current ke simpul buku berikutnya di dalam rantai list tersebut untuk melanjutkan pengecekan.

Baris 33: Membuat objek simpul baru new_node menggunakan cetakan class Node dari data kode dan judul buku baru jika kodenya belum ada.

Baris 34: Menyambungkan penunjuk next dari buku baru tersebut ke kumpulan buku yang sudah ada di slot indeks tersebut sebelumnya.

Baris 35: Memasukkan objek buku baru tersebut ke posisi paling depan dari slot indeks tabel hash sebagai ketua rantai yang baru.

Operasi Pencarian Data Buku (Search)
Baris 37: Membuat fungsi search untuk mencari informasi data buku di dalam perpustakaan berdasarkan kode bukunya.

Baris 38: Mencari tahu nomor indeks lokasi slot penyimpanan menggunakan fungsi hash dari kode buku yang dicari.

Baris 39: Membuat variabel acuan current yang dimulai dari data buku paling depan pada slot indeks hasil pencarian.

Baris 40: Melakukan perulangan while untuk menelusuri rantai buku di slot tersebut selama datanya masih ada.

Baris 41: Mengecek apakah kode buku pada simpul yang sedang diperiksa nilainya cocok dengan kode buku yang dicari pengguna.

Baris 42: Mengembalikan seluruh objek simpul data buku tersebut ke program utama jika kodenya berhasil ditemukan.

Baris 43: Menggeser penunjuk variabel current ke simpul buku berikutnya di dalam rantai untuk melanjutkan pencarian.

Baris 44: Mengembalikan nilai kosong None jika seluruh rantai di slot tersebut sudah diperiksa dan kode buku tetap tidak ditemukan.

Operasi Hapus Data Buku (Remove)
Baris 46: Membuat fungsi remove_key untuk menghapus data buku dari sistem perpustakaan berdasarkan kode buku yang dipilih.

Baris 47: Menghitung nomor indeks lokasi penyimpanan buku yang mau dihapus menggunakan bantuan fungsi hash.

Baris 48: Membuat variabel acuan current untuk memeriksa simpul buku dari urutan paling depan di slot indeks tersebut.

Baris 49: Menyiapkan variabel pembantu bernama prev yang diatur kosong untuk mencatat simpul buku yang berada tepat di urutan sebelum current.

Baris 50: Melakukan perulangan while untuk berjalan menelusuri rantai simpul buku selama posisinya belum habis.

Baris 51: Mengecek apakah kode buku pada simpul yang sedang diperiksa nilainya sama dengan kode buku yang ingin dihapus.

Baris 52: Mengecek apakah simpul buku yang mau dihapus posisinya berada di urutan paling pertama di dalam slot tabel.

Baris 53: Memindahkan penunjuk utama tabel di indeks tersebut langsung ke buku urutan kedua agar buku pertama otomatis terhapus.

Baris 54: Menjalankan blok perintah alternatif else jika buku yang mau dihapus posisinya berada di tengah atau di ujung rantai.

Baris 55: Menyambungkan penunjuk next dari buku sebelumnya (prev) langsung melompati current menuju ke buku setelahnya agar current terhapus.

Baris 56: Mengembalikan nilai True ke program utama sebagai tanda bahwa proses penghapusan data buku berhasil dilakukan.

Baris 57: Memperbarui isi variabel prev dengan data current saat ini sebelum bergeser maju ke simpul selanjutnya.

Baris 58: Menggeser posisi variabel current ke simpul buku berikutnya di dalam rantai untuk melanjutkan pencarian.

Baris 59: Mengembalikan nilai False jika sampai akhir rantai diperiksa ternyata kode buku yang mau dihapus tidak ditemukan.

Fungsi Penampilan Seluruh Data (Display)
Baris 61: Membuat fungsi display untuk menunjukkan struktur visual seluruh slot tabel hash beserta buku-buku di dalamnya ke layar.

Baris 62: Mencetak baris baru teks judul informasi berupa "Daftar Data Buku Perpustakaan:" ke layar terminal.

Baris 63: Melakukan perulangan for untuk berjalan melewati setiap nomor slot indeks dari angka 0 sampai batas ukuran maksimal tabel.

Baris 64: Mencetak nomor indeks slot saat ini ke layar terminal tanpa membuat baris baru di akhir cetakannya.

Baris 65: Menentukan variabel acuan current untuk memulai penelusuran dari simpul buku pertama di dalam slot indeks tersebut.

Baris 66: Melakukan perulangan while untuk mencetak semua isi buku yang terangkai di dalam slot tersebut selama datanya ada.

Baris 67: Mencetak informasi data kode buku dan judul buku saat ini dengan format panah penghubung ke layar terminal.

Baris 68: Menggeser posisi variabel current ke simpul data buku berikutnya agar bisa dicetak pada perulangan selanjutnya.

Baris 69: Mencetak teks tulisan "Kosong" sebagai penanda akhir dari rantai buku pada slot tersebut sekaligus membuat baris baru.

Fungsi Utama Sistem (Main Program)
Baris 72: Membuat fungsi bernama main yang bertindak sebagai jantung kendali utama jalannya seluruh program interaktif perpustakaan.

Baris 73: Membuat objek baru bernama hashmap yang dibangun menggunakan cetakan dari class HashMapSeparateChaining.

Baris 74-80: Memasukkan tujuh data buku contoh awal ke dalam objek hashmap menggunakan fungsi insert dengan berbagai variasi kode buku.

Baris 81: Memanggil fungsi display milik objek hashmap untuk memperlihatkan struktur data buku contoh yang baru saja dimasukkan.

Baris 82: Menginisialisasi variabel pilih dengan nilai awal angka 0 untuk menampung pilihan menu pengguna.

Baris 83: Melakukan perulangan while yang akan terus memunculkan pilihan menu selama pengguna tidak memilih menu nomor 5.

Baris 84-89: Mencetak teks judul sistem perpustakaan beserta daftar pilihan opsi menu nomor 1 sampai 5 ke layar terminal.

Baris 90: Memulai blok perintah try untuk mengantisipasi kesalahan ketik dari pengguna saat menginput pilihan menu.

Baris 91: Meminta pengguna memasukkan angka pilihan menu dan langsung mengubahnya menjadi tipe data integer ke variabel pilih.

Baris 92: Menjalankan blok except ValueError apabila pengguna salah memasukkan input yang bukan berupa angka bulat.

Baris 93: Mencetak pesan peringatan kesalahan "Input tidak valid!" ke layar terminal akibat kesalahan tipe data.

Baris 94: Melanjutkan langsung ke awal perulangan while menu tanpa mengecek perintah di bawahnya lagi.

Baris 95: Mengecek kondisi apabila pengguna mengetikkan angka 1 untuk memilih menu tambah buku baru.

Baris 96: Memulai blok perintah try untuk mengamankan proses input penambahan data buku baru.

Baris 97: Meminta pengguna memasukkan data kode buku baru (yang di sini variabelnya tertulis nama dan kode buku) melalui papan ketik.

Baris 98: Meminta pengguna memasukkan teks nama atau judul buku baru yang ingin disimpan ke dalam sistem.

Baris 99: Mengubah input kode buku menjadi integer lalu memasukkannya ke dalam tabel lewat fungsi insert.

Baris 100: Mencetak kalimat pemberitahuan berupa teks "\nDaftar Buku setelah ditambah:" ke layar terminal setelah berhasil.

Baris 101: Menangkap kesalahan input pada blok except jika kode buku yang dimasukkan pengguna ternyata bukan angka bulat.

Baris 102: Mencetak pesan kesalahan berupa kalimat "Input tidak valid!" ke layar terminal pengguna.

Baris 103: Mengecek kondisi alternatif apabila pengguna mengetikkan angka 2 untuk memilih menu pencarian buku.

Baris 104: Meminta input kode buku yang ingin dicari, mengubahnya jadi angka, lalu menyimpannya di variabel cari.

Baris 105: Jalankan fungsi search untuk mencari kode buku tersebut dan simpan hasil simpulnya di variabel hasil.

Baris 106: Mengecek kondisi jika isi data di dalam variabel hasil terbukti ada atau tidak bernilai kosong.

Baris 107: Mencetak informasi ke layar bahwa kode buku yang dicari ketemu beserta menampilkan judul bukunya.

Baris 108: Menjalankan perintah alternatif dari blok else apabila isi variabel hasil terbukti kosong.

Baris 109: Mencetak pesan ke layar terminal yang mengonfirmasi bahwa buku tersebut tidak ditemukan dalam sistem.

Baris 110: Mengecek kondisi alternatif apabila pengguna mengetikkan angka 3 untuk memilih menu hapus buku.

Baris 111: Memulai blok perintah try untuk menangani proses input penghapusan data buku dari pengguna.

Baris 112: Meminta input kode buku yang ingin dihapus dari sistem lalu menyimpannya dalam bentuk integer ke variabel x.

Baris 113: Mengecek terlebih dahulu apakah kode buku yang mau dihapus tersebut posisinya ada di dalam tabel lewat fungsi search.

Baris 114: Memanggil fungsi remove_key untuk menghapus rantai simpul kode buku tersebut dari sistem tabel hash jika ada.

Baris 115: Mencetak pesan konfirmasi ke layar terminal bahwa data kode buku beserta judulnya telah sukses dihapus.

Baris 116: Menjalankan perintah dari blok else jika kode buku yang mau dihapus ternyata tidak ditemukan sejak awal pencarian.

Baris 117: Mencetak pesan kesalahan ke layar terminal bahwa kode buku tersebut tidak ada di dalam daftar perpustakaan.

Baris 118: Menangkap kesalahan input pada blok except jika nilai kode buku yang mau dihapus diinput bukan berupa angka bulat.

Baris 119: Mencetak teks pemberitahuan kesalahan berupa kalimat "Kode tidak valid!" ke layar terminal.

Baris 121: Mengecek kondisi alternatif apabila pengguna mengetikkan angka 4 untuk memilih menu tampilkan daftar.

Baris 122: Memanggil fungsi display milik objek hashmap untuk mencetak struktur tabel hash saat ini ke layar.

Baris 123: Mengecek kondisi alternatif apabila pengguna mengetikkan angka 5 untuk memilih menu keluar aplikasi.

Baris 124: Mencetak kalimat pemberitahuan akhir berupa teks "Program selesai." ke layar terminal.

Baris 125: Menjalankan perintah terakhir dari blok else jika angka menu yang diketik bukan di antara rentang nomor 1 sampai 5.

Baris 126: Mencetak pesan peringatan berupa kalimat "Pilihan tidak valid!" ke layar terminal pengguna.

Baris 128: Mengecek kondisi utama apakah file script Python ini sedang dieksekusi secara langsung sebagai program pusat.

Baris 129: Memanggil dan memproses fungsi main() untuk mengaktifkan seluruh rangkaian jalannya program aplikasi perpustakaan.

# Output

Output sistem ini akan menampilkan data yang sudah tersimpan dan juga sebuah pilihan berupa tambah, mencari, menghapus, menampilkan daftar buku serta mengakhiri program.

# Link Youtube
https://youtu.be/Tt1hjcglvUQ
