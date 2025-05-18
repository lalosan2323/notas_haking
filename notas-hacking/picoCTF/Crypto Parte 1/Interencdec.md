
## Description

Can you get the real meaning from this file.Download the file [here](https://artifacts.picoctf.net/c_titan/2/enc_flag).

## Hint

1. Engaging in various decoding processes is of utmost importance

## Solution

Toma el contenido de `enc_flag` y lo decodifica a base 64. 

```
┌──(lalosan㉿lalosan)-[~/crypto1/interencdec]
└─$ base64 -d enc_flag  
b'd3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrXzc4MjUwaG1qfQ=='
```


Ingresamos la siguiente cadena a cyber chef
`d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrXzc4MjUwaG1qfQ==`


Y nos regresa la siguiente cadena
`gwpjvJAM{jhlzhy_k3jy9wa3k_78250hmj}`

La ingresamos a un decodificador de cifrado césar: 

A la vuelta 19 nos muestra:


flag-> picoCTF{caesar_d3cr9pt3d_78250afc}