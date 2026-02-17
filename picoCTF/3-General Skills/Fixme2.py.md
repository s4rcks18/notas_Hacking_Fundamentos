## Fixme2.py
## Descripción
Fix the syntax error in the Python script to print the flag.
## Solución
```
Sarkcs20-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/6/fixme2.py -q
Sarkcs20-picoctf@webshell:~$ python fixme2.py
  File "/home/Sarkcs20-picoctf/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
Sarkcs20-picoctf@webshell:~$ nano fixme2.py
Sarkcs20-picoctf@webshell:~$ python fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_f6a5aefc}
```
## Notas
## Referencias