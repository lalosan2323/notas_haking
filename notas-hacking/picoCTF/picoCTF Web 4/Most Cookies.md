
## Description

Alright, enough of using my own encryption. Flask session cookies should be plenty secure! [server.py](https://mercury.picoctf.net/static/26760321c25c9659050a37a707247690/server.py) [http://mercury.picoctf.net:52134/](http://mercury.picoctf.net:52134/)

## Hint
How secure is a flask cookie?

## Solution

![[Pasted image 20250414204650.png]]
1. Vamos a tomar el valor de las cookies para crear un diccionario.
2. Acomodamos todos los valores en un archivo cookies.txt
3. Para poder instalar la herramienta python.flask-unsign se necesita un ambiente virtual.
4. Utilizamos flask en la cookie con ayudan del diccionario que creamos.
![[Pasted image 20250415151355.png]]
![[Pasted image 20250415151555.png]]
