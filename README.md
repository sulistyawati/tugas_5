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

		elif perintah.lower() == 't':
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
			
* Untuk nilai akhir n_akhir, di buat berdasarkan operasi dari variabel n_tugas, n_UTS dan n_UAS yang mewakili Nilai Tugas, UTS dan UAS.

![nambah data](https://user-images.githubusercontent.com/57305570/72215215-d1ab4e80-3542-11ea-9c8f-b57b485d16ad.png)

* 6. Melihat data
Selanjutnya adalah kode yang digunakan untuk melihat input yang sudah dimasukan :


![lihat data](https://user-images.githubusercontent.com/57305570/72215244-4ed6c380-3543-11ea-9e21-88f74d770494.png)



* Data dalam perulangan for di ambil dari variabel dictionary daftar pada bagian value yang berbentuk list. variabel no diguanakan untuk membuat nomor. Data yang akan ditampilkan adalah **Nama, NIM, Nilai Tugas, UTS, UAS, dan Nilai Akhir**.

![output lihat data](https://user-images.githubusercontent.com/57305570/72215269-a412d500-3543-11ea-9478-beecbb20cc04.png)

* 7. Mengubah data
* Perintah dijalankan jika input yang di masukan adalah u, di dalam kondisi ini terdapat input dan kondisi, dimana jika input nama ada di dalam variabel daftar.keys maka akan muncul beberapa pilihan untuk mengubah semua data atau data tertentu saja.
* Selanjutnya adalah kode yang digunakan untuk menggubah input yang sudah dimasukan :

![4](https://user-images.githubusercontent.com/57305570/72215300-fa801380-3543-11ea-8c3b-d67ae9b2eff7.png)

* Berikut kondisi yang digunakan untuk memasukan pilihan :

![output](https://user-images.githubusercontent.com/57305570/72215330-534fac00-3544-11ea-99cb-5572a8b44f8e.png)

* 8. Mencari Data
* Perbandingan untuk mencari data yang akan diubah sama seperti cara mengubah data, hanya saja perintah ini digunakan untuk menampilkan data yang di input berdasarkan nama.
* Berikut bagaimana mencari data yang sudah di inputkan sebelumnya :

![8](https://user-images.githubusercontent.com/57305570/72215345-872ad180-3544-11ea-8082-31adf0c6aae0.png)

** Output ** 

![cari](https://user-images.githubusercontent.com/57305570/72215359-bb9e8d80-3544-11ea-846a-66386e7f545c.png)

* 9. Menghapus data
* Sama seperti mengubah dan mencari data, untuk menghapus data yang dipilih :

![9](https://user-images.githubusercontent.com/57305570/72215391-264fc900-3545-11ea-82a2-fcb4054dd1e5.png)

* Data yang di hapus adalah data yang di input dalam variabel nama dimana berisi nama (string) yang mewakili data **NIM, Nilai Tugas, UTS dan UAS**.

![9](https://user-images.githubusercontent.com/57305570/72215391-264fc900-3545-11ea-82a2-fcb4054dd1e5.png)

