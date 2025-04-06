
## Description


This is a really weird text file [TXT](https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt)? Can you find the flag?

## Hint 

How do operating systems know what kind of file it is? (It's not just the ending!
## Solution

File format es la manera en que los datos están organizados y almacenados dentro de un archivo, es el idioma específico que usan las computadoras para entender el contenido de ese archivo.


```

mv es el comando de mover o renombrar en sistemas linux, no cambia el conetino del archivo, ,solo el nombre/extension.

mv flag.txt flag.png


y luego volvemos abrir el archivo 

open flag.png



```

flag- > picoCTF{now_you_know_about_extensions}
