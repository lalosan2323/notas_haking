

## Description

Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

## Solution



```

┌──(lalosan㉿lalosan)-[~/for4/sa]
└─$ mmls disk.flag.img 
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000206847   0000204800   Linux (0x83)
003:  000:001   0000206848   0000360447   0000153600   Linux Swap / Solaris x86 (0x82)
004:  000:002   0000360448   0000614399   0000253952   Linux (0x83)

```

Fls se utiliza para **listar los nombres de los archivos y directorios** de un sistema de archivos. Es una de las primeras herramientas que un analista forense suele ejecutar en una imagen de disco o un dispositivo.


"Icat" se utiliza para mostrar el contenido de un archivo desde una imagen de disco o un sistema de archivos basándose en su número de inode.



![[Pasted image 20250508125013.png]]
