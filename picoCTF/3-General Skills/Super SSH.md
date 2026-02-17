## Super SSH
## Descripción
Using a Secure Shell (SSH) is going to be pretty important.Can you `ssh` as `ctf-player` to `titan.picoctf.net` at port `57249` to get the flag?You'll also need the password `1db87a14`. If asked, accept the fingerprint with `yes`.If your device doesn't have a shell, you can use: [https://webshell.picoctf.org](https://webshell.picoctf.org/)If you're not sure what a shell is, check out our Primer: [https://primer.picoctf.com/#_the_shell](https://primer.picoctf.com/#_the_shell)
## Solución
```
Sarkcs20-picoctf@webshell:~$ ssh ctf-player@ titan.picoctf.net -p 57249
ssh: Could not resolve hostname : Name or service not known
Sarkcs20-picoctf@webshell:~$ ssh ctf-player@titan.picoctf.net -p 57249
The authenticity of host '[titan.picoctf.net]:57249 ([3.139.174.234]:57249)' can't be established.
ED25519 key fingerprint is SHA256:4S9EbTSSRZm32I+cdM5TyzthpQryv5kudRP9PIKT7XQ.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[titan.picoctf.net]:57249' (ED25519) to the list of known hosts.
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_45a48857}
Connection to titan.picoctf.net closed.
Sarkcs20-picoctf@webshell:~$ 
```
## Notas
## Referencias