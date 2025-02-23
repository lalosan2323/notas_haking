
## DESCRIPTION
I accidentally wrote the flag down. Good thing I deleted it!You download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/76/challenge.zip)

## SOLUTION

````
-- Con el uso del comando git reflog vemos los commits perdidos o los cambios que se hicieron con la rama referenciada. 
	EduardoSanchez-picoctf@webshell:~/drop-in$ git reflog
	e720dc2 (HEAD) HEAD@{2}: commit (initial): create flag
-- Con el uso del comando nos movemos al commit donde se hizo la creación de la bandera. Y hacemos un cat para ver el contenido del message.txt
	EduardoSanchez-picoctf@webshell:~/drop-in$ git checkout e720dc2       
	Note: switching to 'e720dc2'.
	EduardoSanchez-picoctf@webshell:~/drop-in$ cat message.txt
	picoCTF{s@n1t1z3_7246792d}
	
	


```

