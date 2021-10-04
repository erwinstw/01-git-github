# Tugas MDPL Praktik
<h2> Daftar isi : </h2>


1. [Install GIT](https://github.com/erwinstw/erwinstw-01-git-github#-instalasi-git-di-windows)
2. [Konfigurasi GIT]()
3. [Mengelola Repositori]()
* [Mengelola repositori di akun sendiri]()
* [Mengelola repositori di organisasi]()

<h2> Instalasi Git di Windows</h2>

Setelah download Git, double click pada file yang di-download. Akan dimunculkan lisensi. Klik Next untuk lanjut.

![image.png](img/1.png)

Setelah itu, pilih lokasi instalasi. Secara default akan terisi C:\Program Files\Git. Ganti lokasi jika memang anda menginginkan lokasi lain, klik Next

![image.png](img/tambahan.jpg)

Pilih komponen. Tidak perlu diubah-ubah, sesuai dengan default saja. Klik pada Next.

![image.png](img/2.png)

Mengisi shortcut untuk menu Start. Gunakan default (Git), ganti jika ingin mengganti - misalnya Git VCS.

![image.png](img/3.png)

Pilih editor yang akan digunakan bersama dengan Git. Pada pilihan ini, digunakan Notepad++.

![image.png](img/4.png)

Pilih Let Git decide. 

![image.png](img/5.png)

Pilih Git from command line and also from 3rd-party software

![image.png](img/6.png)

Pilih pilihan pertama

![image.png](img/7.png)

Pilih OpenSSL untuk HTTPS. Git menggunakan https untuk akes ke repo GitHub atau repo-repo lain (GitLab, Assembla).

![image.png](img/8.png)

Pilih pilihan pertama untuk konversi akhir baris (CR-LF).

![image.png](img/9.png)

Untuk opsi ekstra, pilih serta aktifkan 1 dan 2.

![image.png](img/10.png)

Kemudian klik Install

![image.png](img/11.png)

Setelah itu proses instalasi akan dilakukan.

![image.png](img/12.png)

Jika selesai akan muncul dialog pemberitahuan. Klik pada Finish.

![image.png](img/13.png)

Untuk menjalankan, dari Start menu, ketikkan "Git", akan muncul beberapa pilihan. Pilih "Git Bash" atau "Git GUI".

![image.png](img/14.png)

Tampilan jika akan menggunakan "Git Bash"

![image.png](img/15.png)

Tampilan jika akan menggunakan "Git GUI"

![image.png](img/16.png)

Untuk mencoba dari command prompt, masuk ke command prompt, setelah itu eksekusi "git --version" untuk melihat apakah sudah terinstall atau belum. Jika sudah terinstall dengan benar, makan akan muncul hasil berikut:

![image.png](img/17.png)

# Konfigurasi GIT

Sebelum mengguanakan git sebaiknya melakukan 2 konfigurasi username dan email, dengan menggunakan perintah berikut ini :


```
$ git config --global user.name "username"
$ git config --global user.email emailkamu@domain.tld
```



Pastikan username dan email untuk memasukkan username dan email yang sama dengan github yang digunakan.dan gunakan perintah dibawah ini untuk melihat configurasinya.

# Mengelola Repositori
Personal access token
Mulai 13 Agustus 2021, penggunakan token merupakan hal wajib ubtuk semua akses ke github yang memerlukan otentikasi. Sehingga perlu membuat personal access token. dapat melihat pada link berikut : https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

## Mengelola repositori di akun sendiri

### Membuat Repository

Langkah pertama yang dilakukkan adalah membuat repositori baru klik tanda + dibagian pojok kanan atas, lalu pilih New repository.

![q](img/c.png)

isikan nama repositori, deskripsi (opsional), dan lisensi (bila diperlukan), dan repositori dapat dibuat public maupun private.

![org](img/eq.png)

klik tombol Create repository

Clone Repository
Clone repositori adalah cara ubtuk menduplikasi ropositori kita yang berada digithub ke komputer lokal. caranya dengan menggunakan perintah berikut ini $ git clone https://alamatrepo.git.

![h](img/y.png)

Setelah melakukan clone di komputer lokal kita dapat melakukan perubahan maupun penambahan yang nantinya dapat dipush ke github.


Mengubah - Push tanpa branching dan merging
perubahan terjadi karena :

Ada file atau direktori yang dihapus
Isi File berubah, atau file diedit
Ada File atau direktori baru

![h](img/a.png)

Ketika menabahkan file README.md dan memasukan text otomatis telah terjadi perubahan kita perlu untuk melakukan perintah $ git add -A untuk memasukan file mana saja yang akan dicommit, setelah itu kita perlu melakukan commit dengan perintah ``$ git commit -m`` "pesan" barulah melakukan push dengan perintah $ git push origin branch.

Mengubah isi dengan branching dan merging
Dengan cara ini ketika akan melakukan perubahan, perubajhan itu dilakukan di komuter lokal dengan membuat branch yang nantinya akan digunakan untuk menampung perubahan - perubahan. Dan nantinya branch itu akan di merge dengan branch utama biasanya bernama master atau main.

![h](img/b.png)




# Sinkronisasi
Bila kita melakukkan perubahan di komputer lain kita perlu melakukkan sinkronisasi pada komputer lainnya. Dengan perintah berikut :
```
$ git pull
```
Membatalkan Perubahan


# Mengelola repositori di organisasi

Repositori dapat kita buat diakun kita maupun berada di organisasi. Organisasi dapat kita buat sendiri juga bila dimasukkan menjadi anggota organisasi. Perbedaan pada saat membuat diakun sendiri adalah pada bagian Owner, Owner dari repositori yang kita buat adalah organisasi.

![org](img/organisasi.png)
