Tugas-Sistem-Operasi
NAMA:M.Firzy Alfurqon  
NIM:09011382530149  

Berikut adalah 50 perintah terminal Ubuntu untuk username `firzy`:

1. Melihat Direktori Saat Ini
firzy@ubuntu:~$ pwd
2. Melihat Daftar File dan Folder
firzy@ubuntu:~$ ls
3. Melihat Daftar File Tersembunyi
firzy@ubuntu:~$ ls -a
4. Melihat Detail File dan Hak Akses
firzy@ubuntu:~$ ls -l
5. Pindah ke Direktori Tertentu
firzy@ubuntu:~$ cd /path/ke/direktori
6. Pindah ke Direktori Home
firzy@ubuntu:~$ cd ~
7. Naik Satu Level Direktori
firzy@ubuntu:~$ cd ..
8. Membuat Folder Baru
firzy@ubuntu:~$ mkdir nama_folder
9. Membuat File Kosong
firzy@ubuntu:~$ touch nama_file.txt
10. Melihat Isi File
firzy@ubuntu:~$ cat nama_file.txt
11. Membaca File per Halaman
firzy@ubuntu:~$ less nama_file.txt
12. Melihat 10 Baris Pertama File
firzy@ubuntu:~$ head nama_file.txt
13. Melihat 10 Baris Terakhir File
firzy@ubuntu:~$ tail nama_file.txt
14. Menyalin File
firzy@ubuntu:~$ cp file_asal.txt file_tujuan.txt
15. Menyalin Folder
firzy@ubuntu:~$ cp -r folder_asal folder_tujuan
16. Memindahkan atau Mengubah Nama File
firzy@ubuntu:~$ mv nama_lama.txt nama_baru.txt
17. Menghapus File
firzy@ubuntu:~$ rm nama_file.txt
18. Menghapus Folder dan Isinya
firzy@ubuntu:~$ rm -rf nama_folder
19. Menghapus Folder Kosong
firzy@ubuntu:~$ rmdir nama_folder
20. Mencari File Berdasarkan Nama
firzy@ubuntu:~$ find . -name "nama_file.txt"
21. Mencari Teks dalam File
firzy@ubuntu:~$ grep "kata" nama_file.txt
22. Mengubah Hak Akses File
firzy@ubuntu:~$ chmod 755 nama_file.txt
23. Mengubah Pemilik File
firzy@ubuntu:~$ sudo chown firzy:firzy nama_file.txt
24. Mengedit File dengan Nano
firzy@ubuntu:~$ nano nama_file.txt
25. Mengubah Akses Menjadi Superuser (Root)
firzy@ubuntu:~$ sudo su
26. Memperbarui Daftar Paket Aplikasi
firzy@ubuntu:~$ sudo apt update
27. Mengupgrade Paket Aplikasi
firzy@ubuntu:~$ sudo apt upgrade
28. Menginstall Aplikasi Baru
firzy@ubuntu:~$ sudo apt install nama_aplikasi
29. Menghapus Aplikasi
firzy@ubuntu:~$ sudo apt remove nama_aplikasi
30. Clean Up Paket Tidak Terpakai
firzy@ubuntu:~$ sudo apt autoremove
31. Melihat Daftar Proses Berjalan
firzy@ubuntu:~$ ps aux
32. Melihat Monitoring Sistem Real-time
firzy@ubuntu:~$ top
33. Menghentikan Proses Berdasarkan PID
firzy@ubuntu:~$ kill 1234
34. Menghentikan Proses Berdasarkan Nama
firzy@ubuntu:~$ pkill nama_proses
35. Melihat Penggunaan Memori (RAM)
firzy@ubuntu:~$ free -h
36. Melihat Penggunaan Ruang Disk
firzy@ubuntu:~$ df -h
37. Melihat Ukuran Folder/File
firzy@ubuntu:~$ du -sh nama_folder
38. Melihat Informasi Pengguna Saat Ini
firzy@ubuntu:~$ whoami
39. Melihat Detail Sistem OS
firzy@ubuntu:~$ uname -a
40. Melihat Alamat IP Sistem
firzy@ubuntu:~$ ip a
41. Uji Koneksi Jaringan
firzy@ubuntu:~$ ping google.com
42. Mengunduh File dari Internet
firzy@ubuntu:~$ wget [http://example.com/file.zip](http://example.com/file.zip)
43. Mengubah Kata Sandi Pengguna
firzy@ubuntu:~$ passwd
44. Melihat Riwayat Perintah
firzy@ubuntu:~$ history
45. Membuat File Arsip Tar.gz
firzy@ubuntu:~$ tar -czvf arsip.tar.gz nama_folder
46. Mengekstrak File Tar.gz
firzy@ubuntu:~$ tar -xzvf arsip.tar.gz
47. Mengosongkan Tampilan Terminal
firzy@ubuntu:~$ clear
48. Melihat Manual Penggunaan Perintah
firzy@ubuntu:~$ man nama_perintah
49. Mulai Ulang Sistem (Restart)
firzy@ubuntu:~$ sudo reboot
50. Mematikan Sistem (Shutdown)
firzy@ubuntu:~$ sudo shutdown -h now
