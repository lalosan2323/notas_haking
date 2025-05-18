

## Description

Decrypt this [message](https://jupiter.challenges.picoctf.org/static/7d707a443e95054dc4cf30b1d9522ef0/ciphertext).

## Hint

caesar cipher [tutorial](https://learncryptography.com/classical-encryption/caesar-cipher)


## Solution

Le aplicamos un cat al archivo, y nos muestra la bandera pero esta esta encriptada. 

```
┌──(lalosan㉿lalosan)-[~/crypto1/caesar]
└─$ cat ciphertext 
picoCTF{gvswwmrkxlivyfmgsrhnrisegl}                                                     
```

Metemos la siguiente cadena a un decodificador de cifrado de cesar: 
`vswwmrkxlivyfmgsrhnrisegl`

flag-> picoCTF{crossingtherubicondjneoach}