## DESCRIPTION
Find the flag being held on this server to get ahead of the competition [http://mercury.picoctf.net:45028/](http://mercury.picoctf.net:45028/)

## HINT

- Maybe you have more than 2 choices
- Check out tools like Burpsuite to modify your requests and look at the responses
## SOLUTION

````

Se usa CURL con la opción -I, que sirve para hacer una petición HTTP HEAD al servidor y obtener solo los encabezados de la respuesta, sin cambiar el contenido de la página. 

EduardoSanchez-picoctf@webshell:~$ curl -I http://mercury.picoctf.net:45028/index.php
HTTP/1.1 200 OK
-> flag: 

Content-type: text/html; charset=UTF-8
picoCTF{r3j3ct_th3_du4l1ty_775f2530}

```