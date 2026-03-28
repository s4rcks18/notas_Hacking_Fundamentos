## Sleuthkit Apprentice
## Descripción
Download this disk image and find the flag. Note: if you are using the webshell, download and extract the disk image into /tmp not your home directory.

Download compressed disk image
## Solución
despues de descomprimirlo
-mmls disk.flag.img
-fls -o 2048 disk.flag.img
-fls -o 360448 -r disk.flag.img
-icat -o 360448 -r disk.flag.img 2371
picoCTF{by73_5urf3r_adac6cb4}
## Notas
## Referencias