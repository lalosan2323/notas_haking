
## Description

We have several pages hidden. Can you find the one with the flag?The website is running [here](http://saturn.picoctf.net:57145/).

## Hint
folders folders folders

## Solution

Inspeccionamos el html.
Nos vamos a la direccion de la pagína donde se encuentra la carpeta secrets.
```
http://saturn.picoctf.net:57145/secret/


Analizamos el html de esa parte y nos dirigimos a la siguiente dirección.
http://saturn.picoctf.net:52855/secret/hidden/

Analizamos el html de esa parte y nos dirigimos a la siguiente dirección.
http://saturn.picoctf.net:52855/secret/hidden/superhidden/

No nos aparece nada a la vista de la página, inspeccionamos el código fuente. 


<h1>Finally. You found me. But can you see me</h1>|
<h3 class="flag">picoCTF{succ3ss_@h3n1c@10n_51b260fe}</h3>

flag- > picoCTF{succ3ss_@h3n1c@10n_51b260fe}
```

