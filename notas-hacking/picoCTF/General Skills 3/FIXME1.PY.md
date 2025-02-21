
## DESCRIPTION
Fix the syntax error in this Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/26/fixme1.py)

## HINT
Indentation is very meaningful in Python

## SOLUTION


````
- Descargamos el archivo 
EduardoSanchez-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/26/fixme1.py

- utilizamos nano para ver el archivo y modificarlo. Ctrl + x para guardar los cambios. El error era que un print estaba mañ identado.
flag = str_xor(flag_enc, 'enkidu')
print('That is correct! Here\'s your flag: ' + flag) -> corregido

- ejecutamos el programa y nos muestra la flag
EduardoSanchez-picoctf@webshell:~$ nano fixme1.py
EduardoSanchez-picoctf@webshell:~$ python fixme1.py
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_09ee727a}
EduardoSanchez-picoctf@webshell:~$ 

```