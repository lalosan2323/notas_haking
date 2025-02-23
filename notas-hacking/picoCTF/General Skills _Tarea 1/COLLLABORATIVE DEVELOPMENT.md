
## DESCRIPTION

My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/69/challenge.zip)

## SOLUTION


````

-- Con git branch vemos las ramas del trabajo. 

	EduardoSanchez-picoctf@webshell:~/drop-in$ git branch 
	* feature/part-1
	  feature/part-2
	  feature/part-3
-- Con git checkout nos movemos entre las rammas de nuestros proyectos.

-- Nos movemos a la primera rama del proyecto y ejecutamos el programa flag, nos muestra la primera parte de la flag. 
	EduardoSanchez-picoctf@webshell:~/drop-in$ python flag.py 
	Printing the flag...
	picoCTF{t3@mw0rk_ -> parte de la flag

-- Nos movemos a la segunda rama y ejecutamos el programa
	EduardoSanchez-picoctf@webshell:~/drop-in$ git checkout feature/part-2
	Switched to branch 'feature/part-2'
	EduardoSanchez-picoctf@webshell:~/drop-in$ python flag.py 
	Printing the flag...
	m@k3s_th3_dr3@m_ - > parte de la flag
--  Nos movemos a la segunda tercera y ejecutamos el programa
	EduardoSanchez-picoctf@webshell:~/drop-in$ python flag.py 
	Printing the flag...
	w0rk_e4b79efb} -> parte de la flag

-- flag completa -> picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_e4b79efb}
	




```


