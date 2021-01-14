Autologin
Autologin WMS, WIFI ID, dll with OpenWRT

Instalasi
Merk Router bebas

Router sudah terinstall OS OpenWRT

Sambungkan dengan Internet, akan ada update dan download library

Copy file autologin ke ROOT, (biasanya saya pakai WinSCP)

Gunakan PUTTY dan lakukan remote SSH Router anda

Jalankan perintah pada PUTTY dan tunggu sampai proses selesai :

sh autologin

Untuk buka GUI ketik pada browser anda:

http://IP-ROUTER-ANDA/cgi-bin/register

contoh = http://192.168.1.1/cgi-bin/register

Isi Kolom dalam GUI, sesuaikan dengan kondisi URL Landing Page anda dan kode Voucher anda.

Klik SUBMIT

Sambungkan Router anda ke jaringan Wifi ID, WMS Venue atau Wico 2.0 anda

Restart

Selesai

Pemecahan masalah
A. Jika setelah proses Instalasi dan tidak mau tersambung dengan jaringan

Periksa jaringan anda

Periksa apakah Jenis Voucher, Produk dan Type jaringan anda sudah sesuai (WMS Venue, WIFI ID atau WICO)

Periksa di Gui apakah sudah benar data yang anda masukkan

Periksa penulisan Username dan Password Voucher anda

Periksa INTERFACE yang terkoneksi apakah sudah betul

Jika sudah benar semua, SSH Router anda dengan PUTTY lalu jalankan perintah :

sh auto_login

Lihat proses yg berjalan dan bandingkan Informasi yg ada dengan GUI yg sudah anda input.

B. Jika masih belum tersambung, kemungkinan pemblokiran MAC ADDRESS Router oleh ISP Anda.

Isi Kolom NEW MAC pada tampilan GUI dengan MAC ADDRESS

Format penulisan : xx:xx:xx:xx:xx:xx
atau tulis "random" ==> huruf kecil semua dan tanpa tanda petik
Klik SUBMIT

Tunggu 1 menit atau lakukan SSH Router anda dengan PUTTY lalu jalankan perintah :

sh auto_login

4. Lihat hasil
