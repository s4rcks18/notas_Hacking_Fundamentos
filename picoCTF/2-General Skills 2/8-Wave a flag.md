## ### Wave a flag
## Descripción
Can you invoke help flags for a tool or binary? This program has extraordinarily helpful information...
## Solución

```
Sarkcs20-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_wily_courier/fc72a950cbaa130f81486c2df35deced17604b2c08c6a5aa99d18168036d3107/warm

Sarkcs20-picoctf@webshell:~$ chmod +x warm
Sarkcs20-picoctf@webshell:~$ ./warm
Hello user! Pass me a -h to learn what I can do!
Sarkcs20-picoctf@webshell:~$ -h
-bash: -h: command not found
Sarkcs20-picoctf@webshell:~$ ./warm -h
```

picoCTF{b1scu1ts_4nd_gr4vy_ac5832c}
## Notas
## Referencias