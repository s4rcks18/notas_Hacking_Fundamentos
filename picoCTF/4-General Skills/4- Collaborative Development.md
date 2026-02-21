## ### Collaborative Development
## Descripción
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:
## Solución
```
Sarkcs20-picoctf@webshell:~/drop-in$ git branch -a
Sarkcs20-picoctf@webshell:~/drop-in$ git checkout feature/part-1
Switched to branch 'feature/part-1'
Sarkcs20-picoctf@webshell:~/drop-in$ cat flag.py
print("Printing the flag...")
print("picoCTF{t3@mw0rk_", end='')Sarkcs20-picoctf@webshell:~/drop-in$ git checkout feature/part-2
Switched to branch 'feature/part-2'
Sarkcs20-picoctf@webshell:~/drop-in$ cat flag.py
print("Printing the flag...")

print("m@k3s_th3_dr3@m_", end='')Sarkcs20-picoctf@webshell:~/drop-in$ git checkout feature/part-3
Switched to branch 'feature/part-3'
Sarkcs20-picoctf@webshell:~/drop-in$ cat flag.py
print("Printing the flag...")

print("w0rk_7ffa0077}")
```

	picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_7ffa0077}
## Notas
menciona algo de unir mediante el git config pero no entendi entonces lo tome asi
## Referencias