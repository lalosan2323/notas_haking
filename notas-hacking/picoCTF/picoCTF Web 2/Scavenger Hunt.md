## DESCRIPTION
There is some interesting information hidden around this site [http://mercury.picoctf.net:55079/](http://mercury.picoctf.net:55079/). Can you find it

## HINT

You should have enough hints to find the files, don't run a brute forcer.

## SOLUTION

Nos metemos al html, en un comentario aparece la primera parte de la flag. 

![[Pasted image 20250326224911.png]]

En el archivo mycss.css se encuantra la otra parte de la flag : h4ts_4_l0

En el archivo myjs.js no se encuentra la otra parte, pero si nos deja la siguiente pista: 
![[Pasted image 20250326225231.png]]

Nos vamos al archvio robots.txt. http://mercury.picoctf.net:55079/robots.txt

Se encuentra una parte de la flag, y otra pista para la última parte. 
![[Pasted image 20250326225424.png]]
Nos vamos al archivo .htaccess http://mercury.picoctf.net:55079/.htaccess

![[Pasted image 20250326225615.png]]

En el contexto de las mac, existe un archivo .DS_Store, el cual almacena información de la configuración una carpeta, como la posición de los íconos, aquello que tenga que ver con lo visual.  
http://mercury.picoctf.net:55079/.DS_Store
![[Pasted image 20250326225941.png]]

flag -> picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_74cceb07}