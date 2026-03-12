## WhitePages
## Descripción
I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://challenge-files.picoctf.net/c_fickle_tempest/bdd421d396847b0b8c86a2bc0c86331a18e2f9191b961b162f7c6379a4ca94be/whitepages.txt) is all blank!
## Solución
utilizando un codigo para poder abrir el archivo y realizar los intercambios correspindientes para que de la bandera.
```
def convertSpacesToBinary():
    with open('whitepages.txt', 'rb') as f:
        result = f.read()
    result = result.replace(b'\xe2\x80\x83', b'0')  # Unicode EM SPACE -> 0
    result = result.replace(b'\x20', b'1')  # ASCII Space -> 1
    result = result.decode()
    return result

def convertFromBinaryToASCII(binaryValues):
    binary_int = int(binaryValues, 2)
    byte_number = (binary_int.bit_length() + 7) // 8
    binary_array = binary_int.to_bytes(byte_number, "big")
    ascii_text = binary_array.decode('ascii')
    print(ascii_text)

convertFromBinaryToASCII(convertSpacesToBinary())
```

picoCTF{not_all_spaces_are_created_equal_aa90f80c1cebc20be3564d2f96a9726c}
## Notas
codigo de internet
## Referencias