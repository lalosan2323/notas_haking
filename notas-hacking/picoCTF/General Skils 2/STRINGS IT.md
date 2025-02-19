## DESCRIPTION

Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings) without running it?

## SOLUTION

````

Descargo el archivo 
wget https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings


Es un archivo de 64 bits ejecutable

Se utiliza el comando strings que extrae y muestra las cadenas de texto en un archivo bianrio, y con el comando grep se filtra las lisnes que contengan la palabra pico. 

EduardoSanchez-picoctf@webshell:~$ strings strings | grep pico
flag -> picoCTF{5tRIng5_1T_7f766a23}

```