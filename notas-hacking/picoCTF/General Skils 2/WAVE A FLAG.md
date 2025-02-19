
## DESCRIPTION
Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/f95b1ee9f29d631d99073e34703a2826/warm) has extraordinarily helpful information...

## SOLUTION

````
LE DOY PERMISOS A EL ARCHVIO PARA PODER EJECUTARLO, LE PASAMOS EL -H PARA MOSTRAR LA AYUDA DEL PROGRAMA.

EduardoSanchez-picoctf@webshell:~$ chmod +x warm
EduardoSanchez-picoctf@webshell:~$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: 
flag -> picoCTF{b1scu1ts_4nd_gr4vy_f0668f62}
```