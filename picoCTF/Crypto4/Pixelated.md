## Pixelated
## Descripción
I have these 2 images, can you make a flag out of them?

[scrambled1.png](https://challenge-files.picoctf.net/c_wily_courier/fd911d04c960ddc4effdf884e8cc954b91e1936eb4c1bdee81a39f7b16a5e465/scrambled1.png) [scrambled2.png](https://challenge-files.picoctf.net/c_wily_courier/fd911d04c960ddc4effdf884e8cc954b91e1936eb4c1bdee81a39f7b16a5e465/scrambled2.png)
## Solución
utilize el segundo metodo a solucionar que es el de python con el codigo siguiente, despues de abrirlo tomo el texto y solamente le doy el formato de bandera:
```
from PIL import Image import numpy as np imagen1 = np.asarray( Image.open('scrambled1.png') ) imagen2 = np.asarray( Image.open('scrambled2.png') ) data = imagen1 + imagen2 nueva = Image.fromarray(data) nueva.save("out.png", "PNG")
```
picoCTF{8cdf93c3}
## Notas
## Referencias