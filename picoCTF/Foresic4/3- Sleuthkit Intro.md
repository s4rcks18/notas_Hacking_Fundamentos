## Sleuthkit Intro
## Descripción
Download the disk image and use mmls on it to find the size of the Linux partition. Connect to the remote checker service to check your answer and get the flag. Note: if you are using the webshell, download and extract the disk image into /tmp not your home directory. Download disk image

Additional details will be available after launching your challenge instance.
## Solución
gzip -d disk.img.gz
file disk.img
mmls disk.img -- aqui nos da el tamaño en linux que necesita la bandera y al conectarnos al servidor nos pregunta ese valor.

nc saturn.picoctf.net 52273

picoCTF{mm15_f7w!}
## Notas
## Referencias