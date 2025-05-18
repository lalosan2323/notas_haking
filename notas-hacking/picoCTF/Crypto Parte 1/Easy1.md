
## Description

The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We've given you the encrypted flag, key, and a table to help `UFJKXQZQUNB` with the key of `SOLVECRYPTO`. Can you use this [table](https://jupiter.challenges.picoctf.org/static/1fd21547c154c678d2dab145c29f1d79/table.txt) to solve it?.

## Hint 

1. Submit your answer in our flag format. For example, if your answer was 'hello', you would submit 'picoCTF{HELLO}' as the flag.
2. Please use all caps for the message.

## Solution

El cifrado de Vigenere es un cifrado de sustitución parafilético, lo que significa que usa múltiples alfabetos de cigfrado, a diferencia del César que solo usa uno .

- Se tiene un mensaje claro, se tiene una palabra de clave, cada letra del mensaje se desplaza una cierta cantidad, según la letra correspondiente de la clave. 

Se utiliza el mensaje `UFJKXQZQUNB` y `SOLVECRYPTO`:

Utilizando un decodificador `vigenere` :

el siguiente mensaje decodificado -> `CRYPTOISFUN`

flag-> picoCTF{CRYPTOISFUN}