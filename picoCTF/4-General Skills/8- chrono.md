##  chrono
## Descripción
How to automate tasks to run at intervals on linux servers?

Additional details will be available after launching your challenge instance.
## Solución
```
picoplayer@challenge:~$ ls -la /
total 0
drwxr-xr-x   1 root   root     51 Feb 21 02:45 .
drwxr-xr-x   1 root   root     51 Feb 21 02:45 ..
-rwxr-xr-x   1 root   root      0 Feb 21 02:45 .dockerenv
lrwxrwxrwx   1 root   root      7 Mar  8  2023 bin -> usr/bin
drwxr-xr-x   2 root   root      6 Apr 15  2020 boot
d---------   1 root   root     27 Aug  4  2023 challenge
drwxr-xr-x   5 root   root    340 Feb 21 02:45 dev
drwxr-xr-x   1 root   root     66 Feb 21 02:45 etc
drwxr-xr-x   1 root   root     24 Aug  4  2023 home
lrwxrwxrwx   1 root   root      7 Mar  8  2023 lib -> usr/lib
lrwxrwxrwx   1 root   root      9 Mar  8  2023 lib32 -> usr/lib32
lrwxrwxrwx   1 root   root      9 Mar  8  2023 lib64 -> usr/lib64
lrwxrwxrwx   1 root   root     10 Mar  8  2023 libx32 -> usr/libx32
drwxr-xr-x   2 root   root      6 Mar  8  2023 media
drwxr-xr-x   2 root   root      6 Mar  8  2023 mnt
drwxr-xr-x   2 root   root      6 Mar  8  2023 opt
dr-xr-xr-x 275 nobody nogroup   0 Feb 21 02:45 proc
drwx------   2 root   root     37 Mar  8  2023 root
drwxr-xr-x   1 root   root     66 Feb 21 02:53 run
lrwxrwxrwx   1 root   root      8 Mar  8  2023 sbin -> usr/sbin
drwxr-xr-x   2 root   root      6 Mar  8  2023 srv
dr-xr-xr-x  13 nobody nogroup   0 Feb 21 02:45 sys
drwxrwxrwt   1 root   root      6 Aug  4  2023 tmp
drwxr-xr-x   1 root   root     18 Mar  8  2023 usr
drwxr-xr-x   1 root   root     17 Mar  8  2023 var
picoplayer@challenge:~$ ls -la /challenge
ls: cannot open directory '/challenge': Permission denied
picoplayer@challenge:~$ cat /etc/crontab
# picoCTF{Sch3DUL7NG_T45K3_L1NUX_1d781160}
picoplayer@challenge:~$ Connection to saturn.picoctf.net closed by remote host.
Connection to saturn.picoctf.net closed.
Sarkcs20-picoctf@webshell:~$ 
```
## Notas
tuve que buscar el problema en linea pero tenian soluciones que no se me permetian por permisos entonces busque con las ias dando la solucion.
## Referencias