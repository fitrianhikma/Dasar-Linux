# Dasar-Linux
$ man apt | akan menampilkan manual penggunaan dari program apt.

$ ls /var/lib | digunakan untuk melihat apa saja yang ada pada folder lib.

$ cd /home/ | untuk menjadikan folder home sebagai direktori pada saat itu.

$ cp /home/test.php /var/www/html | akan memindahkan file test.php ke folder html. Sedangkan jika menyalin folder harus menggunakan opsi “-r”.

$ cp /home/test.php /var/www/html | digunakan untuk memindahkan file test.php ke folder html.

$ rm <file> | untuk menghapus file
  
$ find -name niagahoster.txt

$ history | grep apt

$ cat niagahoster1.txt niagahoster2.txt | lihat isi file

$ echo “Teks” >> niagahoster.txt |. Perintah tersebut akan menuliskan “Teks” ke dalam file “niagahoster.txt”, jika file tersebut belum ada maka otomatis akan dibuat.

$ grep -i source niagahoster.txt | maka akan memunculkan baris yang mengandung kata “source” pada “niagahoster.txt”.

$ chmod 644 niagahoster.txt | untuk mengganti hak akses

$ chown niaga:niaga niagahoster.txt |. Kata “niaga” di depan merujuk pada user sedangkan “niaga” di belakang merujuk pada nama group.

$ su <nama user> | atau menjadikan user pada saat itu menjadi super user.
  
$ sudo passwd | mengganti password user pada saat itu, sedangkan
$ sudo passwd niagahoster | digunakan untuk mengganti password user “niagahoster”.

$ sudo kill -9 373 | 373 adalah PID dari proses yang sedang berjalan.
  
$ sudo fdisk -l | Menampilkan list partisi pada perangkat, biasanya menggunakan opsi “-l”

$ sudo mount /dev/sda2 /mnt |. Perintah ini akan membuat isi partisi /dev/sda2 bisa diakses melalui /mnt.

$ umount /mnt | digunakan untuk memutuskan perintah mount pada folder /mnt

# Penting
$ ls -lh | lihat list file

$ netstat -plnt | lihat koneksi, port

# SSH
$ ssh <namauser>@<ip>
$ ssh -p 2222 fitria@103.110.43.68 | ssh port 2222 namauser@ip

# SCP
$ scp <file> <user>@<ip>:<folder tujuan> | Menyalin file dari host lain yang terhubung dalam satu jaringan
$ scp -P 2223 coba@localhost:/home/coba/vicon.baru.key | salin ke port 2223 user@lokasi

# Notes
who untuk menampilkan user

ps untuk menampilkan snapshot

mkdir namafolder

kill untuk menghentikan program

ifconfig untuk melihat ip
Melihat IP yang sedang terkoneksi dan network device apa saja yang tersedia.

date untuk menampilkan tanggal
Menampilkan tanggal hari ini.

nano merubah teks editor
Perintah digunakan sebagai text editor yang tidak perlu membuka jendela baru. Hampir sama dengan Vi namun lebih praktis.

top melihat proses secara urut
Melihat semua proses yang sedang berjalan, diurutkan dari proses yang paling besar. Fungsinya hampir sama seperti system monitor.

clear membersihkan terminal
Membersihkan jendela terminal. Jadi isi jendela terminal akan kosong, namun jika di scroll keatas maka perintah yang sebelumnya dijalankan masih bisa terlihat.

dpkg -i <namapackage>.deb instalasi paket
Berguna untuk melakukan instalasi paket dengan ekstensi “.deb”. Terkadang bisa juga menggunakan program “gdebi”, tetapi harus install.

uname melihat versi kernel
Menampilkan versi kernel yang dipakai, tanggal instalasi, dan jenis arsitektur sistem operasi.
