## Permissions
## Descripción
Can you read files in the root file?The system admin has provisioned an account for you on the main server:`ssh  picoplayer@saturn.picoctf.net -p 61798`Password: `UYiOazkqY2`Can you login and read the root file?
## Solución
aplique el comando despues de conectarme al puerto usando sudo -l
despues el comando sudo vi /root para poder tener ina interfas donde manejar la raiz 
entrando en el flag.txt dando la bandera
## Notas
investigue en internet el problema, después investigue que es el comando vi para dando entender que es para tener una interfaz visual para manjar en la terminal, aplicandole el sudo dando permisos.
## Referencias