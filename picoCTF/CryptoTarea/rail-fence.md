## rail-fence
## Descripción
A type of transposition cipher is the rail fence cipher, which is described [here](https://en.wikipedia.org/wiki/Rail_fence_cipher). Here is one such cipher encrypted using the rail fence with 4 rails. Can you decrypt it?

Download the message [here](https://artifacts.picoctf.net/c/188/message.txt).

Put the decoded message in the picoCTF flag format, `picoCTF{decoded_message}`.
## Solución
- Usa un decodificador de **Rail Fence Cipher**.
    
- Si no tienes la clave (número de rieles), prueba del 2 al 6. Con 4 rieles suele ser el estándar en estos retos.
    
- Busca el patrón que empiece con "p", "i", "c", "o".
picoCTF{WH3R3_D035_7H3_F3NC3_8361N_4ND_3ND_4A76B997}
## Notas
## Referencias