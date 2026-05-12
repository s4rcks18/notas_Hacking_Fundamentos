## asm3
## Descripción
What does asm3(0xb75a8f13,0xe1860bd7,0xc8e62f81) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://challenge-files.picoctf.net/c_fickle_tempest/a8d942aa65a7a2dbe79352e0db95f90237024106f4efd380bda7ad339151b383/test.S)
## Solución
### . Ejecución Paso a Paso

- **`<+7>: xor eax, eax`**
    
    - `eax` se limpia por completo: `0x00000000`.
        
- **`<+9>: mov ah, BYTE PTR [ebp+0x9]`**
    
    - El byte en `0x9` es **`0x8f`**.
        
    - `eax` ahora es: `0x00008f00`.
        
- **`<+12>: shl ax, 0x10`**
    
    - Esta es una instrucción "trampa". `ax` es un registro de 16 bits. Desplazar un registro de 16 bits hacia la izquierda 16 veces (`0x10`) vacía el registro por completo.
        
    - `ax` ahora es: **`0x0000`**.
        
- **`<+16>: sub al, BYTE PTR [ebp+0xf]`**
    
    - El byte en `0xf` es **`0xe1`**.
        
    - Operación: `0x00 - 0xe1`.
        
    - En aritmética de 8 bits (unsigned): `0x1f` (esto es como hacer `256 - 225`).
        
    - `ax` ahora es: `0x001f`.
        
- **`<+19>: add ah, BYTE PTR [ebp+0xd]`**
    
    - El byte en `0xd` es **`0x0b`**.
        
    - Sumamos `0x0b` a `ah` (que era `0x00`).
        
    - `ax` ahora es: **`0x0b1f`**.
        
- **`<+22>: xor ax, WORD PTR [ebp+0x12]`**
    
    - Aquí debemos extraer el "Word" (2 bytes) que empieza en la posición `0x12`.
        
    - Tus entradas están alineadas de 4 en 4 bytes. La tercera entrada empieza en `0x10`: `[10: 81], [11: 2f], [12: e6], [13: c8]`.
        
    - Por lo tanto, el Word en `0x12` es **`0xc8e6`**.
        
    - Operación XOR: `0x0b1f XOR 0xc8e6`.
0xc3f9
## Notas
por supuesto revise y vi los videos que nos proporciono el profesor para la solucion del problema.
## Referencias