## DESCRIPTION

Unzip this archive and find the flag.

- [Download zip file](https://artifacts.picoctf.net/c/503/big-zip-files.zip)

## HINT

Can grep be instructed to look at every file in a directory and its subdirectories?

## SOLUTION

`
````
Primeramente descargamos el archivo

- wget https://artifacts.picoctf.net/c/503/big-zip-files.zip)

descomprimimos el .zip con unzip

- unzip big-zip-files.zip

con el grep de forma recusrsiva, se busca dentro de todos los archivos y subdirectortios la cadena picoCTF en el archivo descomprimido

- grep -r "picoCTF" big-zip-files

flag -> picoCTF{gr3p_15_m4g1c_ef8790dc}

```