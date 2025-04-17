Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/ende.py) using [this password](https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/pw.txt) to get [the flag](https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/flag.txt.en)?

## Hint

1. Get the Python script accessible in your shell by entering the following command in the Terminal prompt: `$ wget https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/ende.py`
2. $ man python

## Solution

Copiamos los archivos con wget a nuestro directorio de trabajo, al analizar el código python vemos que acepta las opcioens de -d y -e. Lo que queremos es decodificar la flag, por lo que hacer lo siguiente:`

```
┌──(lalosan㉿lalosan)-[~/exam1p1/python_wrahgling]
└─$ nano pw.txt                
┌──(lalosan㉿lalosan)-[~/exam1p1/python_wrahgling]
└─$ python ende.py -d flag.txt.en
Please enter the password:192ee2db192ee2db192ee2db192ee2db
picoCTF{4p0110_1n_7h3_h0us3_192ee2db}
```

Nos pide una contraseña por lo que pegamos lo que hay dentro del archivo pw.txt y vemos la flag