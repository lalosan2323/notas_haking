## DESCRIPTION

Run the Python script `code.py` in the same directory as `codebook.txt`.

- [Download code.py](https://artifacts.picoctf.net/c/2/code.py)
- [Download codebook.txt](https://artifacts.picoctf.net/c/2/codebook.txt)

## HINT
On the webshell, use `ls` to see if both files are in the directory you are in

## SOLUTION


````

Solamente ejecutando el code.py
EduardoSanchez-picoctf@webshell:~$ python code.py
 -> picoCTF{c0d3b00k_455157_7d102d7a}

Quise ver como funcionaba el progrma ay así funciona: 

Le hice un nano al .py, y observé que la contraseña se encuantra en el archivo codebook.txt. Utilizando las posiciones de una cadena. 

password = codebook[4] + codebook[14] + codebook[13] + codebook[14] +\
               codebook[23]+ codebook[25] + codebook[16] + codebook[0]  +\
               codebook[25]
Cadena: azbycxdwevfugthsirjqkplomn

Contraseña: chthonian

```