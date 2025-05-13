
## Description

Every file gets a flag.The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/259/flag.png).

## Hint

none

## Solution

Aplicamos un `strings` a `flag.png`: 

De todo lo que nos muestra existe algo interesante: 

```
7`_QB\\
##ib{
RP0x3
--e^
I|L_
[u]mC
secret/UT
pVgE#
secret/flag.png  <---------
```


Se utiliza la herramienta `binwalk`, es una herramienta forense que analiza archivos binarios en busca de firmas que correspondan a archivos embebidos o estructuras conocidas: como imágenes, archivos comprimidos, ejecutables. 

```
┌──(lalosan㉿lalosan)-[~/forensic3/hideme]
└─$ binwalk -e flag.png                   

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
41            0x29            Zlib compressed data, compressed
39739         0x9B3B          Zip archive data, at least v1.0 to extract, name: secret/
39804         0x9B7C          Zip archive data, at least v2.0 to extract, compressed size: 2869, uncompressed size: 3024, name: secret/flag.png

WARNING: One or more files failed to extract: either no utility was found or it's unimplemented

                                                        
┌──(lalosan㉿lalosan)-[~/forensic3/hideme]
└─$ ls
flag.png  _flag.png.extracted
                                                        
┌──(lalosan㉿lalosan)-[~/forensic3/hideme]
└─$ cd _flag.png.extracted/secret
                                                        
┌──(lalosan㉿lalosan)-[~/forensic3/hideme/_flag.png.extracted/secret]
└─$ open flag.png 
```

flag-> picoCTF{Hiddinng_An_imag3_within_@n_ima9e_cda72af0}