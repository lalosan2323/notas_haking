## DESCRIPTION

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/17/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/17/level3.hash.bin) in the same directory too.There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

## HINT
To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`

## SOLUTION

````
1. lA PRIMERA SOLUCIÓN ES METER CADA CONSTRASEÑA QUE SE ENCUNATRA EN EL LEVEL3.PY, HASTA QUE SALGA LA BUENA. 
2. ES METER LOS HASHES QUE SE ENCUENTRA EN EL BINARIO, LE HACEMOS UN CRACKHASHES EN LA PAGINA CRACKSTATION.  


EduardoSanchez-picoctf@webshell:~$ python level3.py
Please enter correct password for flag: 87ab
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_cd6ed2eb}


```