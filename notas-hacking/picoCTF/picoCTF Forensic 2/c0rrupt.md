## Description

We found this [file](https://jupiter.challenges.picoctf.org/static/ab30fcb7d47364b4190a7d3d40edb551/mystery). Recover the flag.

## Hint
Try fixing the file_header

## Solution

1. Descargamos el archivo.
2. Observamos que el archivo esta dañado.
3. Es un archivo png, por los chunks
4. Los primeros bytes de la cabecera no están bien.
5. ![[Pasted image 20250415174401.png]]
6. Después los chunks los modifuamos también.
7. ![[Pasted image 20250415174659.png]]
```
┌──(eduarsan㉿vbox)-[~/retox]
└─$ file mystery                                                                  
mystery: PNG image data, 1642 x 1095, 8-bit/color RGB, non-interlaced

Checamos el archivo, pero todavia existen errore, en el formato del editor que impide que editor integrado pueda abrir.

```

8. Instalamos pngcheck
9. Modificamos el chunk phYs
10. ![[Pasted image 20250415175157.png]]
11. Se modifica el chunk IDAT
12. Se checa la integridad de los errores, para posteriormente abrirla. 
13. flag-> picoCTF{c0rrupt10n_1847995}