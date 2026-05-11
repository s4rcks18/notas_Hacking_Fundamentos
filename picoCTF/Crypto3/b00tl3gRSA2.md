## b00tl3gRSA2
## Descripción
In RSA d is a lot bigger than e, why don't we use d to encrypt instead of e?

## Solución
usando el codigo compartido e inicial el launcher acomodando los datos nos da la bandera :
```
c = ... n = ... e = ... e = 65537 m = pow(c,e,n) print(m) flag = bytes.fromhex(hex(m)[2:]).decode() print(flag) 
```
picoCTF{bad_1d3a5_3801255}
## Notas
## Referencias