
## Description

We found this [file](https://mercury.picoctf.net/static/d0129ad98ba9258ab59e7700a1b18c14/tunn3l_v1s10n). Recover the flag.

## Solution

Los **magic bytes** (o **números mágicos**) son una **secuencia específica de bytes al principio de un archivo** que sirve para identificar su **tipo o formato**. Son una especie de "firma" del archivo.

en el upset 0x00000000, identificamos los que faltan. 

En el 0A, donde se encuentra algo mal, debe ir la dirección de inicio de los datos. 
Una vez que se termina el encabezado, en el upset 40 se termina el archivo entonces también 0x28. 

En el 0E, también se encuentra mal, debe ir el tamaño del encabezado. 
En el BM- windows el tamaño debe ser de 40 bytes, en hexadecimal 0x28. 


En el upset 16, se observa el tamaño de la imagen, hay que ponerlo más grande para que se vea mejor. 


FLAG-> picoCTF{qu1t3_a_v13w_2020}

