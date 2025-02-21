## DESCRPTION

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/13/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) in the same directory too.

## HINT

Does that encoding look familiar?

## SOLUTION

````
- Descargamos los dos archivos tanto el .py como .enc donde se enceuantra la flag encriptada.

- Con nano vemos el archivo .py, y vemos que la password esta en hexadecimal y la tenemos que pasar a decimal para obtener la flag. Utilizamos cyberchef.
	if( user_pw == chr(0x64) = d + 
	chr(0x65) = e + chr(0x37) = 7 + chr(0x36) = 6 ):
- obtenemos la flag
	EduardoSanchez-picoctf@webshell:~$ nano level2.py
	EduardoSanchez-picoctf@webshell:~$ python level2.py
	Please enter correct password for flag: de76
	Welcome back... your flag, user:
	picoCTF{tr45h_51ng1ng_489dea9a}
	EduardoSanchez-picoctf@webshell:~$ 



```
