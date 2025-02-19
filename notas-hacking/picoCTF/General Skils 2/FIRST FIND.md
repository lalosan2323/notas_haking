## DESCRIPTION

Unzip this archive and find the file named 'uber-secret.txt'

- [Download zip file](https://artifacts.picoctf.net/c/501/files.zip)

## SOLUTION

````

- descargamos el .zip
wget https://artifacts.picoctf.net/c/501/files.zip

- descomprimimos
EduardoSanchez-picoctf@webshell:~$ unzip files.zip
Archive:  files.zip'

- con el grep de forma recusrsiva, se busca dentro de todos los archivos y subdirectortios la cadena picoCTF en el archivo descomprimido
grep -r "picoCTF" files

flag -> picoCTF{f1nd_15_f457_ab443fd1}


```