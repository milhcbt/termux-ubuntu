# Cara Menginstall Ubuntu di Termux

Pada Repository ini berisi sebuah script untuk menginstal `chroot` di termux.
[chroot](https://en.wikipedia.org/wiki/Chroot) adalah sebuah aplikasi di unix variannya (termasuk linux dan termux) 
untuk mensimulasikan akses ke root di mana akses ke root sebenarnya tidak memungkinkan, contoh di android akses 
ke root (rooting) bisa mengakibatkan hilangnya garansi device (tablet/smartphone), sehingga kita perlu menggunakan 
chroot ini untuk bisa menginstall ubuntu.

Jalankan perintah ini di terminal termux

```
pkg update
pkg install wget proot
```

Selanjutnya buat folder yang akan kita jadikan root untuk ubuntu yang akan diinstall dgn perintah sbb

```
mkdir -p ~/jails/ubuntu
cd ~/jails/ubuntu
wget https://raw.githubusercontent.com/Neo-Oli/termux-ubuntu/master/ubuntu.sh
bash ubuntu.sh
```

Setelah selesai menjalankan `./start-ubuntu.sh` untuk masuk mode ubuntu.
