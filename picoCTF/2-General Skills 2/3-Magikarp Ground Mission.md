## Magikarp Ground Mission
## Descripción
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin.

Additional details will be available after launching your challenge instance.
## Solución
se conecto hacia el puerto que se indico pero tambien por ssh despues se realizazo lo siguiente.

```
Sarkcs20-picoctf@webshell:~$  ssh ctf-player@wily-courier.picoctf.net -p 52956

ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ cat 1of3.flag.txt
picoCTF{xxsh_
ctf-player@pico-chall$ cat instructions-to-2of3.txt
Next, go to the root of all things, more succinctly `/`
ctf-player@pico-chall$ cat instructions-to-2of3.txt
Next, go to the root of all things, more succinctly `/`
ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ dior
-bash: dior: command not found
ctf-player@pico-chall$ dir
2of3.flag.txt  challenge  home                      lib64  opt   run   sys  var
bin            dev        instructions-to-3of3.txt  media  proc  sbin  tmp
boot           etc        lib                       mnt    root  srv   usr
ctf-player@pico-chall$ cat instructions-to-3of3.txt
Lastly, ctf-player, go home... more succinctly `~`
ctf-player@pico-chall$ cd ~
ctf-player@pico-chall$ dir
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cat 3of3.flag.txt
0b24fc4f}ctf-player@pico-chall$ 
ctf-player@pico-chall$ cd ..
ctf-player@pico-chall$ dir
ctf-player
ctf-player@pico-chall$ cd ..
ctf-player@pico-chall$ dir
2of3.flag.txt  challenge  home                      lib64  opt   run   sys  var
bin            dev        instructions-to-3of3.txt  media  proc  sbin  tmp
boot           etc        lib                       mnt    root  srv   usr
ctf-player@pico-chall$ cat 2of3.flag.txt
0ut_0f_//4t3r_
```
	picoCTF{xxsh_0ut_0f_//4t3r_0b24fc4f}
## Notas
Buscando en internet e inteligencias para saber como hacer la sintaxis para poder realizar la conexion ssh pero como se nos estaba pidiendo siendo :
ssh ctf-player@wily-courier.picoctf.net -p 52956
## Referencias
ia gemini.