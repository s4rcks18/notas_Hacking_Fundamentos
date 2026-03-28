## Disk, disk, sleuth!
## Descripción
Use `srch_strings` from the sleuthkit and some terminal-fu to find a flag in this disk image.
## Solución
seguimos esos pasos para poder obtener la bandera 
gzip -d dds1-alpine.flag.img.gz
file dds1-alpine.flag.img
sudo apt install -y sleuthkit
srch_strings dds1-alpine.flag.img | grep pico

picoCTF{f0r3ns1c4t0r_n30phyt3_5e56e786}
## Notas
el sleuthkit es para analisis forence
## Referencias