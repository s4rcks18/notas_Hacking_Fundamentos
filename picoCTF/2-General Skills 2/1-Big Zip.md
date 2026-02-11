## ### Big Zip
## Descripción
Unzip this archive and find the flag.
## Solución
En la terminal de pico se consigue el zip despues se descomprime y se le realiza un grep pero para todos los subdirectorios y directorios
```
Sarkcs20-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/505/big-zip-files.zip
Sarkcs20-picoctf@webshell:~$ unzip big-zip-files.zip
Sarkcs20-picoctf@webshell:~$ grep -r "pico"
```

picoCTF{gr3p_15_m4g1c_ef8790dc}
## Notas
Un grep se puede realizar para directorios, archivos y subdirectorios.
## Referencias