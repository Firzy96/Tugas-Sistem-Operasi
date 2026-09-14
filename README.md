Tugas-Sistem-Operasi
NAMA:M.Firzy Alfurqon  
NIM:09011382530149  

1. Mencari dan Menghapus File Log Lama
  `firzy@ubuntu:~$ find /var/log \`
  `> -type f \`
  `> -name "*.log" \`
  `> -mtime +30 \`
  `> -delete`
2. Melihat 10 Proses Konsumsi RAM Tertinggi
`firzy@ubuntu:~$ ps aux \`
`> --sort=-%mem | \`
`> head -n 11`
3. Melihat 10 Proses Konsumsi CPU Tertinggi
`firzy@ubuntu:~$ ps aux \`
`> --sort=-%cpu | \`
`> head -n 11`
4. Membuat Arsip Terenkripsi AES-256
`firzy@ubuntu:~$ tar -czvf - /home/firzy/data | \`
`> openssl enc \`
`> -e \`
`> -aes256 \`
`> -out backup.tar.gz.enc`
5. Membuka Arsip Terenkripsi
`firzy@ubuntu:~$ openssl enc \`
`> -d \`
`> -aes256 \`
`> -in backup.tar.gz.enc | \`
`> tar -xzvf -`
6. Sinkronisasi Folder dengan Progress
`firzy@ubuntu:~$ rsync -avz \`
`> --progress \`
`> --exclude='.git' \`
`> /folder/asal/ \`
`> /folder/tujuan/`
7. Mencari Teks dalam Log secara Rekursif
`firzy@ubuntu:~$ grep \`
`> --color=auto \`
`> -rnw \`
`> -e 'ERROR' \`
`> /var/log/`
8. Melihat Penggunaan Disk Terbesar
`firzy@ubuntu:~$ du -h \`
`> --max-depth=1 \`
`> /var | \`
`> sort -hr`
9. Menampilkan Port yang Aktif dan Listen
`firzy@ubuntu:~$ sudo ss \`
`> -tulnp | \`
`> grep LISTEN`
10. Mengubah Akses Folder Saja secara Rekursif
`firzy@ubuntu:~$ find /path/tujuan \`
`> -type d \`
`> -exec chmod 755 {} +`
11. Mengubah Akses File Saja secara Rekursif
`firzy@ubuntu:~$ find /path/tujuan \`
`> -type f \`
`> -exec chmod 644 {} +`
12. Memonitor Log Sistem secara Real-Time
`firzy@ubuntu:~$ tail \`
`> -f \`
`> -n 50 \`
`> /var/log/syslog`
13. Mengunduh File Besar di Background
`firzy@ubuntu:~$ wget \`
`> -b \`
`> -q \`
`> -c \`
`> [http://example.com/file.iso](http://example.com/file.iso)`
14. Membunuh Proses Berdasarkan Nama
`firzy@ubuntu:~$ ps aux | \`
`> grep 'nginx' | \`
`> awk '{print $2}' | \`
`> xargs sudo kill -9`
15. Menghitung Jumlah Baris Kode/Teks
`firzy@ubuntu:~$ find . \`
`> -name "*.py" | \`
`> xargs wc -l`
16. Membuat File Kosong Berukuran 1GB
`firzy@ubuntu:~$ dd \`
`> if=/dev/zero \`
`> of=test.img \`
`> bs=1M \`
`> count=1024`
17. Cek Koneksi Port Jaringan
`firzy@ubuntu:~$ nc \`
`> -zv \`
`> -w 3 \`
`> 192.168.1.1 \`
`> 80`
18. Mencari File Berdasarkan Ukuran
`firzy@ubuntu:~$ find / \`
`> -type f \`
`> -size +100M \`
`> -exec ls -lh {} +`
19. Mengubah Kepemilikan Rekursif
`firzy@ubuntu:~$ sudo chown \`
`> -R \`
`> firzy:firzy \`
`> /var/www/html`
20. Menggabungkan Beberapa File Teks
`firzy@ubuntu:~$ cat \`
`> file1.txt \`
`> file2.txt | \`
`> sort | \`
`> uniq > gabungan.txt`
21. Melihat Koneksi Jaringan Aktif
`firzy@ubuntu:~$ netstat \`
`> -antp | \`
`> grep ESTABLISHED`
22. Monitor Lalu Lintas Jaringan
`firzy@ubuntu:~$ sudo tcpdump \`
`> -i eth0 \`
`> -n \`
`> port 80`
23. Mencari dan Mengganti Teks dalam File
`firzy@ubuntu:~$ sed \`
`> -i \`
`> 's/lama/baru/g' \`
`> /path/ke/file.txt`
24. Membuat User Baru dengan Home Directory
`firzy@ubuntu:~$ sudo useradd \`
`> -m \`
`> -s /bin/bash \`
`> userbaru`
25. Mengunci Akun Pengguna
`firzy@ubuntu:~$ sudo usermod \`
`> -L \`
`> userbaru`
26. Melihat Tabel Routing Jaringan
`firzy@ubuntu:~$ ip route \`
`> show \`
`> dev eth0`
27. Backup Database MySQL/MariaDB
`firzy@ubuntu:~$ mysqldump \`
`> -u root \`
`> -p \`
`> nama_db | \`
`> gzip > db_backup.sql.gz`
28. Restore Database MySQL/MariaDB
`firzy@ubuntu:~$ gunzip < \`
`> db_backup.sql.gz | \`
`> mysql -u root -p nama_db`
29. Melihat Informasi Perangkat Hardware
`firzy@ubuntu:~$ sudo lshw \`
`> -short \`
`> -class disk`
30. Cek Suhu dan Status Perangkat
`firzy@ubuntu:~$ sensors | \`
`> grep \`
`> 'Core 0'`
31. Menghapus Package dan Konfigurasinya
`firzy@ubuntu:~$ sudo apt purge \`
`> -y \`
`> nama_paket`
32. Melihat Riwayat Perintah Terakhir
`firzy@ubuntu:~$ history | \`
`> tail -n 20 | \`
`> awk '{print $2}'`
33. Uji Kecepatan Akses Disk (Read)
`firzy@ubuntu:~$ sudo hdparm \`
`> -Tt \`
`> /dev/sda`
34. Mengubah Priority Proses (Nice)
`firzy@ubuntu:~$ sudo renice \`
`> -n -10 \`
`> -p 1234`
35. Membuat Cronjob Otomatis
`firzy@ubuntu:~$ (crontab -l ; echo \`
`> "0 2 * * * /path/script.sh") | \`
`> crontab -`
36. Mengubah Format Gambar secara Massal
`firzy@ubuntu:~$ mogrify \`
`> -format png \`
`> *.jpg`
37. Melihat Informasi SSL Certificate
`firzy@ubuntu:~$ openssl x509 \`
`> -in cert.crt \`
`> -text \`
`> -noout`
38. Melihat Jalur Paket Jaringan (Traceroute)
`firzy@ubuntu:~$ traceroute \`
`> -m 15 \`
`> google.com`
39. Membuat SSH Tunneling/Port Forwarding
`firzy@ubuntu:~$ ssh \`
`> -L 8080:localhost:80 \`
`> user@remote_server`
40. Kirim File via SSH (SCP)
`firzy@ubuntu:~$ scp \`
`> -P 22 \`
`> /path/file.txt \`
`> user@remote:/path/tujuan/`
41. Cek Status Service Systemd
`firzy@ubuntu:~$ systemctl status \`
`> nginx.service \`
`> --no-pager`
42. Melihat Log Service Tertentu
`firzy@ubuntu:~$ sudo journalctl \`
`> -u nginx \`
`> -n 100 \`
`> --no-pager`
43. Mencari Package Aplikasi yang Terinstall
`firzy@ubuntu:~$ dpkg-query \`
`> -l | \`
`> grep -i 'docker'`
44. Mengosongkan RAM Cache
`firzy@ubuntu:~$ sudo sync; echo 3 | \`
`> sudo tee \`
`> /proc/sys/vm/drop_caches`
45. Format Partisi Disk ke ext4
`firzy@ubuntu:~$ sudo mkfs.ext4 \`
`> -L "DataDrive" \`
`> /dev/sdb1`
46. Mount Perangkat Disk
`firzy@ubuntu:~$ sudo mount \`
`> -o ro \`
`> /dev/sdb1 \`
`> /mnt/media`
47. Memeriksa Integritas File Hash MD5
`firzy@ubuntu:~$ find . \`
`> -type f \`
`> -exec md5sum {} + > hashes.md5`
48. Verifikasi File Hash MD5
`firzy@ubuntu:~$ md5sum \`
`> -c \`
`> hashes.md5`
49. Membatasi Penggunaan CPU pada Proses
`firzy@ubuntu:~$ cpulimit \`
`> -l 50 \`
`> -p 1234`
50. Melihat Daftar UUID Partisi Disk
`firzy@ubuntu:~$ sudo blkid | \`
`> awk -F: '{print $1, $3}'`
