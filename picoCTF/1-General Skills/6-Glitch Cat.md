## Glitch Cat
## Descripción

Our flag printing service has started glitching!

Additional details will be available after launching your challenge instance.
## Solución
En en problema, nos dan un tipo de launcher donde muestra un comando para linux, se implementa en la terminal de la pagina.
comando realizado:
nc saturn.picoctf.net 51473

texto de resultado:
'picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}'

después se implementa en la pagina de CyberChef para poder combertir el caracter de hexa a asci obteniendo la bandera a entregar: 
picoCTF{gl17ch_m3_n07_bda68f75}
## Notas
 Cyber Chef es una pagina que me permite decodificar en diferentes formatos 
## Referencias
https://gchq.github.io/CyberChef/