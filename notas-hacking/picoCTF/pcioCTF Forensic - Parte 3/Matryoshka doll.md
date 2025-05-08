
## Description

Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: [this](https://mercury.picoctf.net/static/f6cc2560a70b1ea811c151accba5390f/dolls.jpg)


## Solution

Se utiliza unzip para que ir descomprimiendo las imágenes. Nos crea una carpeta base_images, y dentro de esa carpeta hay otra imagen, y así sucesivamente hasta encontrar la flag. 


```
(lalosan㉿lalosan)-[~/par1/matro]
└─$ binwalk dolls.jpg      

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             PNG image, 594 x 1104, 8-bit/color RGBA, non-interlaced
3226          0xC9A           TIFF image data, big-endian, offset of first image directory: 8
272492        0x4286C         Zip archive data, at least v2.0 to extract, compressed size: 378955, uncompressed size: 383936, name: base_images/2_c.jpg
651613        0x9F15D         End of Zip archive, footer length: 22

                                                       
┌──(lalosan㉿lalosan)-[~/par1/matro]
└─$ ls
dolls.jpg
                                                       
┌──(lalosan㉿lalosan)-[~/par1/matro]
└─$ unzip dolls.jpg         
Archive:  dolls.jpg
warning [dolls.jpg]:  272492 extra bytes at beginning or within zipfile
  (attempting to process anyway)
  inflating: base_images/2_c.jpg     
                                                       
┌──(lalosan㉿lalosan)-[~/par1/matro]
└─$ cd base_images 
                                                       
┌──(lalosan㉿lalosan)-[~/par1/matro/base_images]
└─$ ls
2_c.jpg

┌──(lalosan㉿lalosan)-[~/…/matro/base_images/base_images/base_images]
└─$ cat flag.txt       
picoCTF{ac0072c423ee13bfc0b166af72e25b61}                                                  
```