Latihan 1

Menambahkan Global Config

• Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email 

• konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository. 

• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit

• Config Global Repository $ git config --global user.name “nama_user”

    $ git config --global user.email “nama_user”
    
  Membuat Reposiory Local

• Buka direktory aktif, misal: d:\labs_pemrograman1 (buka menggunakan Windows Explorer) 

• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad 

• Buat direktory project praktikum pertama dengan nama latihan1

• Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory) 

• direktory aktif menjadi: d:\labs_pemrograman1\latihan1

    
   $ mkdir latihan1 $ cd latihan1

 Membuat Reposiory Local

• Jalankan perintah git init, untuk membuat repository local.

• Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git 

• Pada direktori tersebut, semua perubahan pada working directory akan disimpan. 

    $ git init
 Menambahkan File baru pada repository

• Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository) • disini kita akan coba    buat satu file bernama README.md (text file)

• File README.md berhasil dibuat. 

    $ echo “#Latihan 1” >> README.md

 
Menambahkan File baru pada repository

• Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

• File README.md berhasil ditambahkan. 

     $ git add README.md

Commit (Menyimpan perubahan ke database)

• Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”

• Perubahan berhasil disimpan.

    $ git commit -m “File pertama saya”

 Membuat repository server

• Server reopsitory yang akan kita gunakan adalah http://github.com 

• Anda harus membuat akun terlebih dahulu. 

• Pada laman github, klik tombol start a project, atau 

• Dari menu (icon +) klik New Repository

 Membuat repository server

• Isi nama repositorynya, misal: labpy1. 

• lalu klik tombol Create repository

 Menambahkan Remote Repository

• Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga    dapat diakses oleh banyak user. 

• Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]

    $ git remote add origin https://github.com/abuazzam/labpy1.git
 
 Push (Mengirim perubahan ke server)

• Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.

• Perintah ini akan meminta memasukkan username dan password pada akun github.com 
