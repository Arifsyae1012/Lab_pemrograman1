Tutorial Menggunakan GIT

Apa itu GiT? Pada tahun 2005, Linus Torvalds (orang yang membuat kernel Linux) membuat GIT dan sejak itu GIT secara aktif dikelola oleh Junio Hamano, programmer Jepang. Saat ini, GIT menjadi salah satu version control system yang paling terkenal dan ada jutaan project di seluruh dunia yang menggunakan GIT untuk version control nya (termasuk project komersil dan open source). GIT sepenuhnya gratis dan bisa di-download di Mac, Linux, Windows, dan Solaris, dari website resminya. 


1.	Install GIT (Windows)
Menginstall GIT di Windows sangat mudah, cukup dengan mendownload dan menjalankan instalasinya.
1.	Download Git, buka website resminya Git (git-scm.com).
Setelah download, buka file tersebut untuk menjalankan proses instalasi. Ikuti semua instruksi, klik Next dan Finish hingga semua proses instalasi selesai.
 
2.	untuk mengetahui git sudah terinstall dengan baik buka cmd lalu ketikkan
	“git –-version”
 



4. Pertama kita buat terlebih dahulu username dan password. Untuk membuatnya jalankan perintah berikut ini di terminal:
	git config --global user.name "Arif Syaefuloh"
	git config --global user.email "Arif_syaefuloh10"

 
note: ubah username dan password sesuai keinginan.
Setelah itu, GIT di Windows Anda siap digunakan.

Menggunakan GIT
Sekarang, setelah GIT di-install di komputer Anda, mari kita pelajari dasar GIT dan bagaimana cara menggunakan GIT.
1.	Membuat Repository local
1.	Buat dan masuk ke direktory aktif, misal: d:\labs_pemrograman1 (buka menggunakan Windows Explorer)
2.	Lalu klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash command
         
3.	Buat direktory pertama dengan nama “latihan1”, atau sesuai keninginan di git bash command.
Ketikkan command berikut. 
1.	“Mkdir latihan1” 
4.	Lalu masuk ke direcktory tersebut dengan command (cd= change directory).
1.	 “Cd latihan1”
Lalu hasilnya akan seperti dibawah ini. direktory aktif menjadi: d:\Lab_Pemrograman1\latihan1
 

5.	Jalankan perintah git init intuk membuat repository local dengan mengetik 
1.	 “$ git init”
Setelah itu repository baru berhasil di-inisialisasi dengan terbentuknya satu directory hidden berformatkan .git pada direktori yang sebelumnya dibuat yang berisi kerangka Git.
Pada directory tersebut semua perubahan pada working directory akan tersimpan.

2.	Menambahkan file baru pada repository
1.	Disini kita akan coba buat satu file bernama README.md (text file), dan akan kita simpan
filenya pada direktori aktif(repository) yang sebelumnya kita buat. Ketikkan perintah berikut:
	“$ echo “# Latihan 1” >> README.md”

 

2.	Ketik “$ ls -l” untuk melihat file README.md
 

3.	Lalu kita tambahkan file baru untuk mengisi file yang sebelumnya kita buat dengan perintah: 
	$ git add README.md
	$ git status

 

3.	Menyimpan perubahan ke database (commit)
Setelah perubahan adanya perubahan data kita bisa menyimpannya kedalam database repository local, perintah untuk menyimpan perubahan ke database adalah git commit –m “komentar commit” (“komentar commit” bisa kita ubah sesuai keinginan kita).

 
4.	Membuat repository server
Github adalah layanan yang paling populer untuk menyimpan (hosting) repository secara remote. Banyak proyek open source tersimpan di sana. Dan kali ini kita akan menggunakan Github sebagai repository server. 
1.	Pertama kita harus memiliki akun di laman web http://github.com.
2.	Setelah itu klik tanda + (plus) di kanan atas sebelah logo akun. Lalu klik new repository seperti gambar berikut.

 

 

3.	Isi repository name “Lab_pemrograman1” (bisa di isi sesuai keinginan kita). Lalu klik create repository.
 


	Dan hasilnya adalah seperti berikut.

 

5.	Menambahkan remote repository
1.	Perintah git remote akan membuat user terhubung ke remote repository,
sehingga dapat diakses oleh banyak user.
(url diisi sesuai dengan url/link git repository server yang dibuat sebelumnya)
	$ git remote add origin [url]

 

6.	Mengirim perubahan ke server repository (push)
1.	Perintah push berfungsi untuk mengirim perubahan pada local repository ke server repository.
	$ git push –u origin master
2.	Saat kita menggunakan perintah ini kita akan diminta untuk memasukan username dan password dari akun github yang telah dibuat.

 

3.	Lalu kita bisa melihat hasilnya pada repository server dengan membuka laman github.com dan kita akan bisa melihat hasilnya.

 








7.	Clone Repository
1.	Clone disini dimaksudkan untuk menduplikat sebuah repository, Proses clone ini biasanya digunakan oleh para developer untuk berkolaborasi di dalam sebuah project, jadi sebuah project dikerjakan oleh lebih dari 1 orang dan project tersebut disimpan di 1 repository saja. Dan perintah untuk clone repository adalah seperti berikut (url diisi sesuai dengan url/link git repository server yang dibuat sebelumnya)
	git clone [url]
 
Dan clone repository berhasil di lakukan. Anda dapat mengecek project yang sudah anda clone di directory yang anda pilih tadi.


8.	Kesimpulan
Cara menggunakan Git ini wajib diketahui dan dikuasai oleh semua developer karena akan sangat membantu dalam mengerjakan project pembuatan website. Demikian penjelasan tentang cara menggunakan Git.
