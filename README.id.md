# Cara Menginstall Ubuntu di Termux

A script to install Ubuntu chroot in Termux
Pada Repository ini berisi sebuah script untuk menginstal `chroot` di termux.
[chroot](https://en.wikipedia.org/wiki/Chroot) adalah sebuah aplikasi di unix variannya (termasuk linux dan termux) 
untuk mensimulasikan akses ke root di mana akses ke root sebenarnya tidak memungkinkan, contoh di android akses 
ke root (rooting) bisa mengakibatkan hilangnya garansi device (tablet/smartphone), sehingga kita perlu menggunakan 
chroot ini untuk bisa menginstall ubuntu.

You need to install wget and proot in Termux before using this script.


```
pkg install wget proot
```

The script will make its files in the current directory. So if you want your Ubuntu-filesystem at a particular location switch to that folder first and then call the script with it's relative path. Example:
```
mkdir -p ~/jails/ubuntu
cd ~/jails/ubuntu
wget https://raw.githubusercontent.com/Neo-Oli/termux-ubuntu/master/ubuntu.sh
bash ubuntu.sh
```

After running it you can run "start-ubuntu.sh" to switch into your ubuntu
