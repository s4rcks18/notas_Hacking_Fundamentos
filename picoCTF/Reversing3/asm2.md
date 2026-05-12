## asm2
## Descripción
What does asm2(0x8,0x2e) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://challenge-files.picoctf.net/c_fickle_tempest/e52eb78a50fe37d5d90fa3200de17edb7b6e51a3e01c583cec0ed94d9e9bc306/test.S)
## Solución
de igual manera que el asm1:
 ### 1. Configuración Inicial (Variables Locales)

El código reserva espacio en el stack y asigna valores a variables locales:

- `[ebp-0x4]` recibe el valor de `[ebp+0xc]`, así que **`var1 = 0x2e`**.
    
- `[ebp-0x8]` recibe el valor de `[ebp+0x8]`, así que **`var2 = 0x8`**.
    

### 2. El Bucle (Loop)

El código salta directamente a la comparación en `<+35>`:

- **Condición:** ¿Es `var2` (`[ebp-0x8]`) menor o igual (`jle`) a **`0xe6da`**?
    
- **Si es cierto:**
    
    1. Suma **1** a `var1`: `var1 = var1 + 0x1`
        
    2. Suma **0xed** (237 en decimal) a `var2`: `var2 = var2 + 0xed`
        
    3. Vuelve a comparar.
        

### 3. Cálculo de la Bandera

Necesitamos saber cuántas veces se ejecuta el bucle para que `var2` supere `0xe6da`.

1. **¿Cuántas iteraciones?**
    
    - `var2` empieza en `0x8`.
        
    - Debe llegar a ser mayor que `0xe6da` (59100 en decimal).
        
    - En cada vuelta aumenta `0xed` (237 en decimal).
        
    - Cálculo: $(0xe6da - 0x8) / 0xed$
        
    - En decimal: $(59098 - 8) / 237 = 59090 / 237 \approx 249.32$
        
    - Esto significa que el bucle se ejecutará **250 veces** (la vuelta 250 es la que finalmente hace que sea mayor).
        
2. **Valor final de `eax` (la bandera):**
    
    - `eax` devuelve el valor de `var1` (`[ebp-0x4]`).
        
    - `var1` empezó en `0x2e`.
        
    - Se le sumó `1` por cada una de las **250** iteraciones.
        
    - $0x2e + 250$ (decimal)
        
    - $250$ en hexadecimal es **`0xfa`**.
        
    - Suma final: `0x2e + 0xfa`
esa es la manera que llego a esa conclusion la ia.
0x128
## Notas
## Referencias