## Operation Orchid
## Descripción
Download this disk image and find the flag. Note: if you are using the webshell, download and extract the disk image into /tmp not your home directory.
## Solución
seguimos los pasos a continuacion despues de descomprimirlo "gzip" : 
-mmls disk.flag.img
-fls -o 411648 disk.flag.img
-icat -i raw -o 411648 disk.flag.img 1875
-icat -o 411648  disk.flag.img 1782
-icat -o 411648 disk.flag.img 1782 > flag.txt.enc
-openssl aes256 -salt -d -in flag.txt.enc -out flag.txt -k unbreakablepassword1234567 (desencriptamos la bandera)
-cat flag.txt

picoCTF{h4un71ng_p457_1d02081e}

## Notas
## Referencias