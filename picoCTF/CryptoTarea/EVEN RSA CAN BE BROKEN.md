## EVEN RSA CAN BE BROKEN
## Descripción
This service provides you an encrypted flag. Can you decrypt it with just N & e?
## Solución
```
# Valores que me pasaste
n = 26392904775820372075658038956570074109240496783261977166125322013210809750367877413977041404722942412786944763352010915956858311394576440354404856493465358
e = 65537
c = 14871642438770396829383921057755488750200564673689701102083102287090966020218300290200546536380377283748275750590880680887576803487188805049531332007954331

# N es par, por lo tanto p=2
p = 2
q = n // p

# Calculamos Phi
phi = (p - 1) * (q - 1)

# Calculamos d (Inverso modular)
# pow(base, exponente, modulo) -> si el exponente es -1, calcula el inverso
d = pow(e, -1, phi)

# Desciframos el mensaje m = c^d mod n
m = pow(c, d, n)

# Convertimos el número resultante a texto
try:
    # Convertimos a hex y luego a bytes
    hex_string = hex(m)[2:]
    # Si el hex es impar, le agregamos un 0 al inicio
    if len(hex_string) % 2 != 0:
        hex_string = '0' + hex_string
    
    flag = bytes.fromhex(hex_string).decode('ascii')
    print(f"\nTu bandera es: {flag}")
except Exception as e:
    print(f"Error al convertir a texto: {e}")
    print(f"Valor numérico de m: {m}")
```
picoCTF{tw0_1$_pr!m375129bb1}
## Notas
codigo dado por IA para poder sacar la bandera.
## Referencias