
## DESCRIPTION

How to automate tasks to run at intervals on linux servers?

Additional details will be available after launching your challenge instance.

## SOLUTION

````

Nos conectamos al servidor. 
EduardoSanchez-picoctf@webshell:~$ ssh picoplayer@saturn.picoctf.net -p 51553

Con el comando cat a esta dirección /etc/crontab, ya que este es el archivo que realiza un seguimineto a las tareas que se ejecutan en el servidor de linux. 
picoplayer@challenge:~$ cat /etc/crontab

flag -> picoCTF{Sch3DUL7NG_T45K3_L1NUX_1d781160}
```






