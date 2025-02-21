
## DESCRIPTION

Fix the syntax error in the Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/4/fixme2.py)

## HINT

Are equality and assignment the same symbol?

## SOLUTION

````

- descargamos el archivo .py
EduardoSanchez-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/4/fixme2.py

- el archivo fixme2.py tenia un error en la linea 22, la sintaxis en un if, al momento de hacer la comparación es con dos "=". 
# Check that flag is not empty
if flag == "": - > corregido
  print('String XOR encountered a problem, quitting.')
else:
  print('That is correct! Here\'s your flag: ' + flag)


- obtenemos la flag
EduardoSanchez-picoctf@webshell:~$ python fixme2.py
  File "/home/EduardoSanchez-picoctf/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
EduardoSanchez-picoctf@webshell:~$ nano fixme2.py
EduardoSanchez-picoctf@webshell:~$ python fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_e8814d03}


```