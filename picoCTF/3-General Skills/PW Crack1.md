## PW Crack1
## Descripción
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/10/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/10/level1.flag.txt.enc) in the same directory too.
## Solución
en esta solucion se podria ver la contraseña por lo que solo se toma y cuando te la pida la mandas dandote la bandera: picoCTF{545h_r1ng1ng_56891419}
```
flag_enc = open('level1.flag.txt.enc', 'rb').read()



def level_1_pw_check():
    user_pw = input("Please enter correct password for flag: ")
    if( user_pw == "691d"):
        print("Welcome back... your flag, user:")
        decryption = str_xor(flag_enc.decode(), user_pw)
        print(decryption)
        return
    print("That password is incorrect")



level_1_pw_check()
Sarkcs20-picoctf@webshell:~$ 
```
## Notas
## Referencias