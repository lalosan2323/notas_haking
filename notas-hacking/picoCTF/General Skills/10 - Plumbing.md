## DESCRIPTION
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 7480`.

## SOLUTION
```
Nos conectamos a un servidor remoto a través del puerto 7480 usando un netcat.
Filtramos la salida del servidor y que me muestre solo las lineas que contiene la palbara 'pico'

comando -> nc jupiter.challenges.picoctf.org 7480 | grep "pico"

flag -> picoCTF{digital_plumb3r_06e9d954}
```
