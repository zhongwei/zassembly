# ZOS
Learning Operating System Development

## Bootloader

```shell
sudo apt install qemu nasm -y
nasm -f bin boot.asm -o boot.bin
qemu-system-x86_64 boot.bin
```
