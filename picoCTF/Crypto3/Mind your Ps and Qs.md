## Mind your Ps and Qs
## Descripción
In RSA, a small e value can be problematic, but what about N? Can you decrypt this?

[values](https://challenge-files.picoctf.net/c_wily_courier/f5f0388785f1835df56b6c50fcbe25d88004d2c3184fe7191b852514bf04941a/values)
## Solución
revisando el video de la clase se puede solucionar pero quise probar si la IA geminis para comporbar si lo soluciona y me dio la bandera claro tambien me dio un codigo :
```
from Crypto.Util.number import inverse, long_to_bytes

# Valores iniciales proporcionados en el reto
c = 15341890103764929939105506004034128738090325640037083301857608662849501626260517
n = 948406957756830799684818171639547165784816468744946013083947881743680617123566349
e = 65537

# Factores primos obtenidos (Ps y Qs)
p = 1891771437429478964908181306574287207137
q = 501332739776173570344039681219489434626477

# Calcular phi(n) y obtener la clave privada d
phi = (p - 1) * (q - 1)
d = inverse(e, phi)

# Desencriptar el mensaje matemáticamente (m = c^d mod n)
m = pow(c, d, n)

# Convertir el número desencriptado resultante a texto ASCII
flag = long_to_bytes(m)
print(flag.decode('utf-8'))
```
picoCTF{sma11_N_n0_g0od_1dc7ae91}

## Notas
## Referencias