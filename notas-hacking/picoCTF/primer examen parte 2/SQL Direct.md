
## Description

Connect to this PostgreSQL server and find the flag!

Additional details will be available after launching your challenge instance.

## Solution


```

┌──(lalosan㉿lalosan)-[~]
└─$ psql -h saturn.picoctf.net -p 61398 -U postgres pico
Contraseña para usuario postgres: 
psql (17.4 (Debian 17.4-1), servidor 15.2 (Debian 15.2-1.pgdg110+1))
Digite «help» para obtener ayuda.

pico=# \d
        Listado de relaciones
 Esquema | Nombre | Tipo  |  Dueño   
---------+--------+-------+----------
 public  | flags  | tabla | postgres
(1 fila)



--------------
  1 | Luke      | Skywalker | picoCTF{L3arN_S0m3_5qL_t0d4Y_31fd14c0}
  2 | Leia      | Organa    | Alderaan
  3 | Han       | Solo      | Corellia
(3 filas)


```