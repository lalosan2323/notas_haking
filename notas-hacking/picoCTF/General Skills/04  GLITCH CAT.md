## DESCRIPTION
Our flag printing service has started glitching!

Additional details will be available after launching your challenge instance.

## HINT
ASCII is one of the most common encodings used in programming

# SOLUTION

````
Aplicamos un net cat -> nc saturn.picoctf.net 56691

Nos muestra una parte de la bandera, pero la otra se intenta concatenar las otros carácteres, pero estos estan en código ASCII.

'picoCTF{gl17ch_m3_n07_' + 
chr(0x61) = a
+ chr(0x34) = 4
+ chr(0x33) = 3
+ chr(0x39)= 9 
+ chr(0x32) = 2
+ chr(0x64) = d
+ chr(0x32) = 2
+ chr(0x65) = e
+ '}'

flag -> picoCTF{gl17ch_m3_n07_a4392d2e}
```