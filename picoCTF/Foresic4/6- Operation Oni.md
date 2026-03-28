## Operation Oni
## Descripción
Download this disk image, find the key and log into the remote machine. Note: if you are using the webshell, download and extract the disk image into /tmp not your home directory.

Additional details will be available after launching your challenge instance.

## Solución
se supone que seguimos lo siguientes comandos que hemos utilizado, descomprimir la imagen, buscar la llave despues utilizarla para poder conectarnos en el puerto y aparte de darle permisos a la llave.
mmls disk.img 
fls -o 206848 disk.img
fls -o 206848 disk.img 470
fls -o 206848 disk.img 3916
icat -o 206848 disk.img 2345 > id_rsa
chmod 600 id_rsa
ssh -i id_rsa -p 64715 ctf-player@saturn.picoctf.net
ls 
cat flag.txt

picoCTF{k3y_5l3u7h_af277f77}

## Notas
## Referencias