Tugas-Sistem-Operasi
NAMA:M.Firzy Alfurqon  
NIM:09011382530149  

Berikut adalah 50 perintah terminal Ubuntu untuk username `firzy`:

1. Melihat Direktori Saat Ini
firzy@ubuntu:~$ pwd
/home/firzy
2. Melihat Daftar File dan Folder
firzy@ubuntu:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
3. Melihat Daftar File Tersembunyi
firzy@ubuntu:~$ ls -a
.    .bash_history  .bashrc  .profile  Documents  Pictures
..   .bash_logout   .cache   Desktop   Downloads  Videos
4. Melihat Detail File dan Hak Akses
firzy@ubuntu:~$ ls -l
drwxr-xr-x 2 firzy firzy 4096 Sep 15 10:00 Desktop
drwxr-xr-x 2 firzy firzy 4096 Sep 15 10:00 Documents
-rw-r--r-- 1 firzy firzy  150 Sep 15 10:05 contoh.txt
5. Pindah ke Direktori Tertentu
firzy@ubuntu:~$ cd /var/log
firzy@ubuntu:/var/log$
6. Pindah ke Direktori Home
firzy@ubuntu:/var/log$ cd ~
firzy@ubuntu:~$
7. Naik Satu Level Direktori
firzy@ubuntu:~$ cd ..
firzy@ubuntu:/home$
8. Membuat Folder Baru
firzy@ubuntu:~$ mkdir proyek_baru
firzy@ubuntu:~$
9. Membuat File Kosong
firzy@ubuntu:~$ touch catatan.txt
firzy@ubuntu:~$
10. Melihat Isi File
firzy@ubuntu:~$ cat catatan.txt
Halo, ini adalah isi dari file catatan.txt
11. Membaca File per Halaman
firzy@ubuntu:~$ less catatan.txt
Halo, ini adalah isi dari file catatan.txt
(END)
12. Melihat 10 Baris Pertama File
firzy@ubuntu:~$ head log.txt
Baris 1
Baris 2
Baris 3
Baris 4
Baris 5
Baris 6
Baris 7
Baris 8
Baris 9
Baris 10
13. Melihat 10 Baris Terakhir File
firzy@ubuntu:~$ tail log.txt
Baris 91
Baris 92
Baris 93
Baris 94
Baris 95
Baris 96
Baris 97
Baris 98
Baris 99
Baris 100
14. Menyalin File
firzy@ubuntu:~$ cp catatan.txt catatan_backup.txt
firzy@ubuntu:~$
15. Menyalin Folder
firzy@ubuntu:~$ cp -r proyek_baru proyek_backup
firzy@ubuntu:~$
16. Memindahkan atau Mengubah Nama File
firzy@ubuntu:~$ mv catatan.txt dokumen.txt
firzy@ubuntu:~$
17. Menghapus File
firzy@ubuntu:~$ rm catatan_backup.txt
firzy@ubuntu:~$
18. Menghapus Folder dan Isinya
firzy@ubuntu:~$ rm -rf proyek_backup
firzy@ubuntu:~$
19. Menghapus Folder Kosong
firzy@ubuntu:~$ rmdir proyek_baru
firzy@ubuntu:~$
20. Mencari File Berdasarkan Nama
firzy@ubuntu:~$ find . -name "dokumen.txt"
./dokumen.txt
21. Mencari Teks dalam File
firzy@ubuntu:~$ grep "Halo" dokumen.txt
Halo, ini adalah isi dari file catatan.txt
22. Mengubah Hak Akses File
firzy@ubuntu:~$ chmod 755 dokumen.txt
firzy@ubuntu:~$
23. Mengubah Pemilik File
firzy@ubuntu:~$ sudo chown firzy:firzy dokumen.txt
[sudo] password for firzy:
firzy@ubuntu:~$
24. Mengedit File dengan Nano
firzy@ubuntu:~$ nano dokumen.txt
(Membuka tampilan text editor Nano di terminal)
25. Mengubah Akses Menjadi Superuser (Root)
firzy@ubuntu:~$ sudo su
root@ubuntu:/home/firzy#
26. Memperbarui Daftar Paket Aplikasi
firzy@ubuntu:~$ sudo apt update
Hit:1 [http://archive.ubuntu.com/ubuntu](http://archive.ubuntu.com/ubuntu) noble InRelease
Get:2 [http://archive.ubuntu.com/ubuntu](http://archive.ubuntu.com/ubuntu) noble-updates InRelease [126 kB]
Fetched 126 kB in 1s (150 kB/s)
Reading package lists... Done
27. Mengupgrade Paket Aplikasi
firzy@ubuntu:~$ sudo apt upgrade
Reading package lists... Done
Building dependency tree... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
28. Menginstall Aplikasi Baru
firzy@ubuntu:~$ sudo apt install curl
Reading package lists... Done
curl is already the newest version (8.5.0-2ubuntu10).
0 upgraded, 0 newly installed, 0 to remove.
29. Menghapus Aplikasi
firzy@ubuntu:~$ sudo apt remove curl
Reading package lists... Done
The following packages will be REMOVED:
curl
0 upgraded, 0 newly installed, 1 to remove.
30. Clean Up Paket Tidak Terpakai
firzy@ubuntu:~$ sudo apt autoremove
Reading package lists... Done
0 upgraded, 0 newly installed, 0 to remove.
31. Melihat Daftar Proses Berjalan
firzy@ubuntu:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.1  21356  9812 ?        Ss   09:00   0:01 /sbin/init
firzy       1234  0.0  0.2  10540  4120 pts/0    Ss   09:05   0:00 -bash
firzy       2345  0.0  0.1  11200  3200 pts/0    R+   10:15   0:00 ps aux
32. Melihat Monitoring Sistem Real-time
firzy@ubuntu:~$ top
top - 10:15:30 up 1:15, 1 user, load average: 0.08, 0.03, 0.01
Tasks: 105 total, 1 running, 104 sleeping
%Cpu(s):  1.5 us,  0.5 sy,  0.0 ni, 98.0 id
MiB Mem :   3950.0 total,   2100.0 free,    850.0 used
33. Menghentikan Proses Berdasarkan PID
firzy@ubuntu:~$ kill 1234
firzy@ubuntu:~$
34. Menghentikan Proses Berdasarkan Nama
firzy@ubuntu:~$ pkill firefox
firzy@ubuntu:~$
35. Melihat Penggunaan Memori (RAM)
firzy@ubuntu:~$ free -h
total        used        free      shared  buff/cache   available
Mem:           3.8Gi       850Mi       2.0Gi        12Mi       1.0Gi       2.8Gi
Swap:          2.0Gi          0B       2.0Gi
36. Melihat Penggunaan Ruang Disk
firzy@ubuntu:~$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        20G  8.5G   11G  45% /
tmpfs           1.9G     0  1.9G   0% /dev/shm
37. Melihat Ukuran Folder/File
firzy@ubuntu:~$ du -sh Documents
12M     Documents
38. Melihat Informasi Pengguna Saat Ini
firzy@ubuntu:~$ whoami
firzy
39. Melihat Detail Sistem OS
firzy@ubuntu:~$ uname -a
Linux ubuntu 6.8.0-40-generic #40-Ubuntu SMP PREEMPT_DYNAMIC x86_64 x86_64 x86_64 GNU/Linux
40. Melihat Alamat IP Sistem
firzy@ubuntu:~$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default
inet 127.0.0.1/8 scope host lo
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default
inet 192.168.1.15/24 brd 192.168.1.255 scope global eth0
41. Uji Koneksi Jaringan
firzy@ubuntu:~$ ping google.com
PING google.com (142.250.190.46) 56(84) bytes of data.
64 bytes from cg-in-f46.1e100.net (142.250.190.46): icmp_seq=1 ttl=115 time=14.2 ms
64 bytes from cg-in-f46.1e100.net (142.250.190.46): icmp_seq=2 ttl=115 time=13.8 ms
^C
--- google.com ping statistics ---
2 packets transmitted, 2 received, 0% packet loss, time 1001ms
42. Mengunduh File dari Internet
firzy@ubuntu:~$ wget [http://example.com/file.zip](http://example.com/file.zip)
--2026-09-15 10:20:00--  [http://example.com/file.zip](http://example.com/file.zip)
Connecting to example.com:80... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1024 (1.0K) [application/zip]
Saving to: ‘file.zip’

file.zip            100%[===================>]   1.00K  --.-KB/s    in 0s

2026-09-15 10:20:00 (15.2 MB/s) - ‘file.zip’ saved [1024/1024]

43. Mengubah Kata Sandi Pengguna
firzy@ubuntu:~$ passwd
Changing password for firzy.
Current password:
New password:
Retype new password:
passwd: password updated successfully
44. Melihat Riwayat Perintah
firzy@ubuntu:~$ history
1  ls
2  pwd
3  mkdir proyek_baru
4  touch catatan.txt
5  history
45. Membuat File Arsip Tar.gz
firzy@ubuntu:~$ tar -czvf arsip.tar.gz Documents
Documents/
Documents/laporan.pdf
Documents/data.xlsx
46. Mengekstrak File Tar.gz
firzy@ubuntu:~$ tar -xzvf arsip.tar.gz
Documents/
Documents/laporan.pdf
Documents/data.xlsx
47. Mengosongkan Tampilan Terminal
firzy@ubuntu:~$ clear
(Layar terminal dibersihkan secara otomatis)
48. Melihat Manual Penggunaan Perintah
firzy@ubuntu:~$ man ls
LS(1)                           User Commands                           LS(1)

NAME
ls - list directory contents

SYNOPSIS
ls [OPTION]... [FILE]...
Manual page ls(1) line 1 (press h for help or q to quit)

49. Mulai Ulang Sistem (Restart)
firzy@ubuntu:~$ sudo reboot
[sudo] password for firzy:
Shutdown scheduled for Tue 2026-09-15 10:25:00 WIB, use 'shutdown -c' to cancel.
50. Mematikan Sistem (Shutdown)
firzy@ubuntu:~$ sudo shutdown -h now
[sudo] password for firzy:
System is going down for power-off NOW!
