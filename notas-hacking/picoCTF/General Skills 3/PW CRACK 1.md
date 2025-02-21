## DESCRIPTION

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/10/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/10/level1.flag.txt.enc) in the same directory too.

## HINT

To view the file in the webshell, do: `$ nano level1.py`

## SOLUTION

````

- Descargamos los dos archivos tanto el .py como .enc donde se enceuantra la flag encriptada.


- con nano vemos el level1.py, y nos damos cuenta que la password es:
 user_pw = input("Please enter correct password for flag: ")
    if( user_pw == "691d"):
- entoces con eso ejecutamos el .py y metemos la constraseña.
	EduardoSanchez-picoctf@webshell:~$ nano level1.py
	EduardoSanchez-picoctf@webshell:~$ python level1.py 
	Please enter correct password for flag: 691d
	Welcome back... your flag, user:
	picoCTF{545h_r1ng1ng_56891419}
```




