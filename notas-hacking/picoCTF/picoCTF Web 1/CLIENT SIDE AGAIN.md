
## DESCRIPTION

Can you break into this super secure portal? `https://jupiter.challenges.picoctf.org/problem/56816/` ([link](https://jupiter.challenges.picoctf.org/problem/56816/)) or http://jupiter.challenges.picoctf.org:56816

## HINT

What is obfuscation?

## SOLUTION

Utilizo un la página jsnice.org y pongo tota la variable 0x5a46 que es una variable que se encuntra muy confusa. Esa página me da el siguiente variable un poco más visible. 

var _0x5a46 = ["37115}", "_again_3", "this", "Password Verified", "Incorrect password", "getElementById", "value", "substring", "picoCTF{", "not_this"];

![[Pasted image 20250321212757.png]]
Nos vamos a consola y formamos la bandera, tomamos las partes que coinciden más con la flag. 