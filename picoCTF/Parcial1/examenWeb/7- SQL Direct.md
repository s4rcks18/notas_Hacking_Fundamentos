##  SQL Direct
## Descripción
Connect to this PostgreSQL server and find the flag!

Additional details will be available after launching your challenge instance.
## Solución
al conectarnos dentro del servidor con el shell de pico, usando \dt para ver las tablas encontramos la tabla flags donde al revisarla con 
```
SELECT * FROM flags;
```
obtemenos la bandera
picoCTF{L3arN_S0m3_5qL_t0d4Y_21c94904}
## Notas
## Referencias