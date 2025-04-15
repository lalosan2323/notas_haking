## DESCRIPTION

The web project was rushed and no security assessment was done. Can you read the /etc/passwd file?

Additional details will be available after launching your challenge instance.

## hint 

XML external entity Injection

## Solution

XXE es una vulnerabilidad de seguridad que ocurre cuando una aplicación que procesa entradas XML no maneja correctamente las entidades externas definidas dentro del documento XML



```
Utilzando la herramienta burpsuit, utilizando una inyección XXE, nos dimos cuenta que le servidor es vulnerable.

<!ENTITY ent SYSTEM "file:///etc/passwd">
Esta línea declara una entidad llamada ent que hace referencia al archivo local /etc/passwd (un archivo típico en sistemas Linux que contiene información sobre los usuarios del sistema).


Esto nos dará como resultado que el servidor procesará el XML y **devolverá como parte de la respuesta el contenido de /etc/passwd
```
![[Pasted image 20250415154830.png]]


![[Pasted image 20250415154844.png]]