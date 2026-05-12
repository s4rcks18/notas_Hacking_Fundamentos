## asm1
## Descripción
What does asm1(0xe26) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://challenge-files.picoctf.net/c_fickle_tempest/c7ce5cfbb522cd448de7adcb1dc42106af4f859002381aa47d85b45cc66aa3f2/test.S)

## Solución
se hace un analisis de como funciona el asm para saber cual es el resultado, al darle la entrada otorgada dentro del reto, sin embargo dando codigo a la ia y pasarle el valor da la bandera:
Paso a paso, así se mueve el procesador con tu valor:

1. **`<+7> cmp 0xe26, 0x75b`**: Compara si tu valor es mayor a `0x75b`.
    
    - **Resultado**: Sí es mayor ($3622 > 1883$). Salta a `<+41>`.
        
2. **`<+41> cmp 0xe26, 0xe26`**: Compara tu valor con `0xe26`.
    
    - **Resultado**: ¡Son iguales! Por lo tanto, **no** salta en la instrucción `jne` (jump if not equal) y continúa a la línea siguiente.
        
3. **`<+50> mov eax, 0xe26`**: Mueve tu valor al registro de retorno.
    
4. **`<+53> sub eax, 0x13`**: A tu valor le resta `0x13` (19 en decimal).
    
5. **`<+56> jmp 0x11ed`**: Salta al final de la función para retornar el resultado.
   este es el orden que siguio segun mi caso.
0xe13
## Notas
## Referencias