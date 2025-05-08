
## Description

I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/52da699e0f203321c7c90ab56ea912d8/Forensics%20is%20fun.pptm)

## Hint

1. None

## Solution

### Para qué se usa un archivo `.pptm`?

- Para **automatizar tareas** dentro de la presentación.
    
- Ejecutar **código personalizado** al abrir o interactuar con la presentación.
    
- Usado frecuentemente en entornos corporativos o educativos para presentaciones interactivas o dinámicas.


Abrimos el archivo, pero no tiene nada. Las macros están deshabilitados.

Desempaquetamos el archivo. 

La bandera se encuentra en hidden.

```
┌──(lalosan㉿lalosan)-[~/par1]
└─$ cat ppt/slideMasters/hidden
Z m x h Z z o g c G l j b 0 N U R n t E M W R f d V 9 r b j B 3 X 3 B w d H N f c l 9 6 M X A 1 f Q                                                                                             
┌──(lalosan㉿lalosan)-[~/par1]
└─$ cat ppt/slideMasters/hidden | tr -d ' ' | base64 -d
flag: picoCTF{D1d_u_kn0w_ppts_r_z1p5}  
```

Con el comando cat se muestra el contenido del archivo hidden, elimina todos los espacios del contenido usando tr (translate/delete characters). Decodifica la salida como si fuera una cadena codificada en base 64. 

flag-> picoCTF{D1d_u_kn0w_ppts_r_z1p5} 


