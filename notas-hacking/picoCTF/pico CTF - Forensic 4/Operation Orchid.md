
## Description

Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

## Hint

1. none
## Solution

- Se utiliza `mmls` sirve para ver el esquema de las particiones dentro de una imagen de disco
- Se utiliza esta partición en 411648
- - **`icat`** extrae un archivo de una imagen (`disk.flag.img`).
- `-o 411648`: indica que el sistema de archivos (FS) inicia en el sector **411648**.
- `> flag.txt.enc`: se guarda como archivo local
- Se descubre  un archivo cifrado.
- Se prueba  cifrar/descifrar con `openssl` usando una contraseña.
- Con un `cat` vemos el contenido de flag.txt


```

┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ mmls disk.flag.img 
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000206847   0000204800   Linux (0x83)
003:  000:001   0000206848   0000411647   0000204800   Linux Swap / Solaris x86 (0x82)
004:  000:002   0000411648   0000819199   0000407552   Linux (0x83)
                                                                                                              
┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ icat  disk.flag.img -o 411648 1782 > flag.txt.enc
                                                                                                              
┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ icat disk.flag.img -o 411648 1782 > flag.txt.enc 
                        
┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ ls
disk.flag.img  flag.txt.enc

┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ icat disk.flag.img -o 411648 1875               
touch flag.txt
nano flag.txt 
apk get nano
apk --help
apk add nano
nano flag.txt 
openssl
openssl aes256 -salt -in flag.txt -out flag.txt.enc -k unbreakablepassword1234567
shred -u flag.txt
ls -al
halt

┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ openssl aes256 -salt -d -in disk.flag.enc -out flag.txt -k unbreakablepassword1234567
Can't open "disk.flag.enc" for reading, No such file or directory
4017A5B8A77F0000:error:80000002:system library:BIO_new_file:No such file or directory:../crypto/bio/bss_file.c:67:calling fopen(disk.flag.enc, rb)
4017A5B8A77F0000:error:10000080:BIO routines:BIO_new_file:no such file:../crypto/bio/bss_file.c:75:

┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ ls
disk.flag.img  flag.txt.enc

┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ ls
disk.flag.img  flag.txt  flag.txt.enc

┌──(lalosan㉿lalosan)-[~/for4/opor]
└─$ cat flag.txt       
picoCTF{h4un71ng_p457_5113beab}   
```


flag -> picoCTF{h4un71ng_p457_5113beab}   