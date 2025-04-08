
## Description

The flag is somewhere on this web application not necessarily on the website. Find it.Check [this](http://saturn.picoctf.net:60571/) out.

## Solution

```

Nos vamos al archivo robots.txt. Me muestra lo siguiente:
ZmxhZzEudHh0;anMvbXlmaW
anMvbXlmaWxlLnR4dA==
svssshjweuiwl;oiho.bsvdaslejg


- Vamos a decodificar, (ZmxhZzEudHh0). Utilizando cyberchef el mensaje esta en base64, nos dice el file1.txt. Lo buscamos pero no hay ningun archivo con ese nombre.
- Vamos a decodificar, (ZmxhZzEudHh0). Utilizando cyberchef el mensaje esta en base64, nos dice qye vayamos a la ruta js/myfile.txt para ver si se encuentra la flag.
- flag -> picoCTF{Who_D03sN7_L1k5_90B0T5_22ce1f22}

```

