## Cookies
## Descripción
Who doesn't love cookies? Try to figure out the best one.

Additional details will be available after launching your challenge instance.
## Solución
aqui se soluciona de varias maneras pero tome la primera que aparece en el video 
```
for i in {0..20}; do curl -s http://wily-courier.picoctf.net:62549/check -H "Cookie: name=$i"; done | grep picoCTF
```

picoCTF{3v3ry1_l0v3s_c00k135_a4dadb49}
## Notas
## Referencias