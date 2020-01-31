# ZOS
Learning Operating System Development

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
