
## DESCRIPTION
There is a website running at `https://jupiter.challenges.picoctf.org/problem/50009/` ([link](https://jupiter.challenges.picoctf.org/problem/50009/)) or http://jupiter.challenges.picoctf.org:50009. Do you think you can log us in? Try to see if you can login!
## HINT

There doesn't seem to be many ways to interact with this. I wonder if the users are kept in a database?

Try to think about how the website verifies your login.

## SOLUTION

Una inyección SQL  es un tipo de ataque en el que un atacante manipula las consultas SQL de una aplicación para acceder, modificar o eliminar datos no autorizados en la base de datos.

![[Pasted image 20250402182704.png]]

En el inspector cambiamos el valor a 1, y volvemos hacer log y observamos como es la sentencia sql para verificar al usuario. 

````

En la parte de username usamos una inyección sql básica -> ' or 1==1;
````

![[Pasted image 20250402183350.png]]



