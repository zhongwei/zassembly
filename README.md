# ZOS
Learning Operating System Development

## qemu

```shell
sudo apt install build-essential zlib1g-dev pkg-config libglib2.0-dev binutils-dev libboost-all-dev autoconf libtool libssl-dev libpixman-1-dev libpython-dev python-pip python-capstone virtualenv
wget https://download.qemu.org/qemu-4.2.0.tar.xz
tar xvJf qemu-4.2.0.tar.xz
cd qemu-4.2.0
./configure
make
sudo make install
```

## VNC

- [RealVNC](https://www.realvnc.com) GTK UI
- [Teamviewr](https://www.teamviewer.com) QT UI

## Bootloader

```shell
sudo apt install qemu nasm -y
nasm -f bin boot.asm -o boot.bin
# curses ui
qemu-system-x86_64 boot.bin --nographic and/or --curses
# VNC Server
qemu-system-x86_64 boot.bin
```
