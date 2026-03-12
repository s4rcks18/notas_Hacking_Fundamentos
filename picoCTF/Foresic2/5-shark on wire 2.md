## shark on wire 2
## Descripción


## Solución
utilizamos un scrip que permitia abrir la captura de los udp para encontrar la bandera

```
from scapy.all import *

flag = ''

packets = rdpcap ('capture(1).pcap')
for p in packets:
   if UDP in p and p[UDP].dport == 22:
      if p[UDP].sport > 5000:
         flag += chr(p[UDP].sport - 5000)
print(flag)
```

picoCTF{p1LLf3r3d_data_v1a_st3g0}
## Notas
## Referencias