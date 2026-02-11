## ### Static ain't always noise
## Descripción
Can you look at the data in this binary? The bash script might help!
## Solución
se trato de darle el presmiso a el sh para poder ejecutarlo después simplemente se muestra el texto para encontrar la solucion

```

Sarkcs20-picoctf@webshell:~$ ./ltdis.sh static
-bash: ./ltdis.sh: Permission denied
Sarkcs20-picoctf@webshell:~$ chmod +x ltdis.sh
Sarkcs20-picoctf@webshell:~$ 
Sarkcs20-picoctf@webshell:~$ ./ltdis.sh static
```
 picoCTF{d15a5m_t34s3r_20335e41}
## Notas
tuve que investigar lo de darle permiso al scrip
## Referencias