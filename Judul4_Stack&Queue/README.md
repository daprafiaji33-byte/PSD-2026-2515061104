# Sistem Antrean Klinik Unila
Sistem ini berfungsii untuk mengatur antrean klinik Unila agar lebih mudah dan simple, sistem ini dapat memberikan beberapa pilihan yaitu menambah pasien, melayani pasien, melihat pasien yang paling depan, dan menampilkan sisa pasien yang ada.

<img width="1048" height="820" alt="Screenshot 2026-05-14 203046" src="https://github.com/user-attachments/assets/1796e762-e4e2-4040-84e2-5cd8f27a0b8c" />
<img width="1064" height="766" alt="Screenshot 2026-05-14 203151" src="https://github.com/user-attachments/assets/12296d59-5bcd-4f33-b67b-e4c0f868252f" />
<img width="1066" height="776" alt="Screenshot 2026-05-14 203223" src="https://github.com/user-attachments/assets/8a600cf6-452c-4fd6-ac1b-10a5e6f28a4b" />
<img width="1117" height="346" alt="Screenshot 2026-05-14 203237" src="https://github.com/user-attachments/assets/a236bdc8-2336-4a6a-86c5-24cf32e5a73f" />


Baris 10: Membuat class QueueArray, wadah utama untuk sistem antrean pasien.

Baris 11: Fungsi awal untuk nyiapin kapasitas antrean (defaultnya 100 orang).

Baris 12-13: Menentukan batas maksimal (MAXN) dan membuat list kosong (q) sebanyak batas tersebut.

Baris 14-15: Menyiapkan penanda indeks depan (front) dan belakang (rear), awalnya diisi -1 karena masih kosong.

Baris 17-18: Fungsi is_empty buat ngecek apakah antrean lagi kosong atau nggak.

Baris 20-21: Fungsi is_full buat ngecek apakah antrean sudah mentok penuh (pake rumus modulo % supaya bisa muter).

Baris 23: Fungsi enqueue buat masukin pasien baru ke barisan.

Baris 24-26: Cek dulu, kalau penuh ya nggak bisa masuk dan muncul pesan "Antrean penuh".

Baris 27-29: Kalau antrean bener-bener kosong, orang pertama ini bakal ditaruh di indeks 0.

Baris 30-31: Kalau sudah ada orang, posisi rear (belakang) bakal geser satu langkah ke depan (pake modulo biar kalau sudah di ujung bisa balik ke awal).

Baris 32: Masukin nama pasien x ke posisi paling belakang tadi.

Baris 33-36: Mennampilkan konfirmasi pasien masuk, lengkap sama estimasi waktu nunggu (5 menit per orang di depannya).

Baris 38: Fungsi dequeue buat manggil pasien paling depan buat dilayani.

Baris 39-41: Cek kalau kosong, ya nggak ada yang bisa dipanggil.

Baris 42: Menampilkan perintah supaya pasien di urutan front menuju loket obat.

Baris 43-45: Kalau ternyata itu adalah orang terakhir di antrean, posisinya direset lagi ke -1 (kosong total).

Baris 46-47: Kalau masih ada orang lain di belakangnya, posisi front (depan) geser satu langkah ke orang berikutnya.

Baris 49: Fungsi peek cuma buat "nengok" siapa sih orang yang paling depan sekarang.

Baris 53: Menampilkan nama pasien yang ada di urutan terdepan tanpa menghapusnya dari antrean.

Baris 55: Fungsi display buat ngeliat seluruh isi barisan dari depan ke belakang.

Baris 60: Mulai penelusuran dari indeks paling depan (front_idx).

Baris 61-62: Pake perulangan while True buat nyetak nama pasien satu per satu.

Baris 63-64: Kalau sudah sampai ke orang paling belakang (rear), perulangan berhenti.

Baris 65: Geser ke indeks selanjutnya (pake modulo supaya tetap melingkar).

Baris 69-71: Fungsi main buat jalanin program, bikin objek queue dan variabel pilih.

Baris 72-78: Selama nggak pilih nomor 5 (Keluar), menu Klinik Unila bakal terus muncul.

Baris 79-83: Minta input pilihan menu dan pake try-except biar kalau inputnya bukan angka nggak langsung force close.

Baris 84-90: Logika menu 1 (Tambah Pasien), minta input nama lalu jalanin enqueue.

Baris 91-96: Logika menu 2 (Layani), menu 3 (Intip depan), dan menu 4 (Tampilkan semua).

Baris 97-100: Keluar dari program atau peringatan kalau pilihan angkanya salah.

Baris 103-104: Perintah buat mulai jalanin fungsi main saat file dibuka.

# OUTPUT
<img width="1477" height="507" alt="Screenshot 2026-05-14 204812" src="https://github.com/user-attachments/assets/e6eded60-160f-45e7-8d8e-b8ad187a2284" />
<img width="1462" height="476" alt="Screenshot 2026-05-14 204852" src="https://github.com/user-attachments/assets/3d6eb9ae-f82b-4862-b646-8c6388473329" />
Output ini menampilkan sebuah inputan kepada user untuk memilih fungsi apa yang ingin di gunakan, seperti menambah pasien, melayani pasien, melihat pasien paling depan, melihat seluruh pasien dan keluar dari program tersebut.

# LINK YOUTUBE
https://youtu.be/_tD3kY_q8mw
