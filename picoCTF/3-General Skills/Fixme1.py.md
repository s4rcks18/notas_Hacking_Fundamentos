## Fixme1.py
## Descripción
Fix the syntax error in this Python script to print the flag.
## Solución
```
Sarkcs20-picoctf@webshell:~$ python fixme1.py
  File "/home/Sarkcs20-picoctf/fixme1.py", line 20
    print('That is correct! Here\'s your flag: ' + flag)
IndentationError: unexpected indent
Sarkcs20-picoctf@webshell:~$ nano fixme1.py
Sarkcs20-picoctf@webshell:~$ python fixme1.py
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_182342f7}
Sarkcs20-picoctf@webshell:~$ 
```
## Notas
## Referencias