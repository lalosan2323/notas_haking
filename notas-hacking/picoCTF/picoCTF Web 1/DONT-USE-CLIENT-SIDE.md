## DESCRIPTION
Can you break into this super secure portal? `https://jupiter.challenges.picoctf.org/problem/37821/` ([link](https://jupiter.challenges.picoctf.org/problem/37821/)) or http://jupiter.challenges.picoctf.org:37821

Se inspecciona el código : 

![[Pasted image 20250321213026.png]]

el código verifica si la contraseña ingresada en un campo con id pass coincide con la clave específica, el valor de split es 4, lo que significa que cada segmento tiene cuatro caracteres. Ordenando los segmentos según su posición en la cadena la flag es -> picoCTF{no_clients_plz_1a3c89}