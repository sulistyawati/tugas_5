# tugas_5

* Buat program sederhana yang akan menampilkan daftar nilai mahasiswa, dengan ketentuan :


* 1. Program dibuat dengan menggunakan Dictionary
* 2. Tampilkan menu pilihan: (Tambah Data, Ubah Data, Hapus Data, Tampilkan Data, Cari Data)
* 3. Nilai Akhir diambil dari perhitungan 3 komponen nilai (tugas: 30%, uts: 35%, uas: 35%)
* 4. Buat flowchart dan penjelasan programnya pada README.md.
* 5. Commit dan push repository ke github.

# Pembahasan
Berikut adalah dictionary yang di definisikan terlebih dahulu :
        
        daftar = {}
Selanjutnya adalah perulangan yang digunakan :

        while True:
                statement

Perulangan di atas adalah perulangan yang akan berjalan terus menerus, dan akan berhenti jika kode berikut di eksekusi :

        if perintah.lower() == 'k':
             break
Kode di atas berfungsi untuk menghentikan perulangan yang berlangsung terus menerus tanpa ada kondisi untuk dipenuhi, di tulis di dalam kondisi ``if``

**Output :**

Jika ``k`` di input dan ``lower()`` digunakan untuk mengkonversi input yang dimasukan ke bentuk *lower case* dan Input ``k`` digunakan berdasarkan perintah yang sudah di masukan dalam keterangan pada fungsi input di bawah ini :

        perintah = input("(L) Lihat, (T) Tambah, 
			  (U) Ubah, (H) Hapus, 
	                  (C) Cari, (K) Keluar: ")

**Output :**

**1. Input Data**
Kondisi berikut digunakan untuk melakukan input data seperti Nama, NIM, Nilai Tugas, UTS dan UAS :
`elif perintah.lower() == 't':
	print("Masukan data mahasiswa")
        print("...")
        nama = input("Masukan nama: ")
        nim = input("Masukan NIM: ")
        n_tugas = int(input("Masukan nilai tugas: "))
        n_UTS = int(input("Masukan nilai UTS: "))
        n_UAS = int(input("Masukan nilai UAS: "))
        a = n_tugas * 30 / 100
        b = n_UTS * 35 / 100
        c = n_UAS * 35 / 100
        n_akhir = a + b + c
        daftar[nama] = [nama, nim, n_tugas, n_UTS, n_UAS, n_akhir]
