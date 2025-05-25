
## Description

In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/3cfeb09681369c26e3f19d886bc1e5d9/values)

## Hint

1. Bits are expensive, I used only a little bit over 100 to save money


## Solution

Observamos el contenido del archivo values: 

```
┌──(lalosan㉿lalosan)-[~/crypto3/mpsq]
└─$ cat values 
Decrypt my super sick RSA:
c: 8533139361076999596208540806559574687666062896040360148742851107661304651861689
n: 769457290801263793712740792519696786147248001937382943813345728685422050738403253
e: 65537    
```

Utilizando la herramienta FactorDB, se factoriza n para sacar p y q

```
──(lalosan㉿lalosan)-[~/crypto3/mpsq]
└─$ python       
Python 3.13.2 (main, Feb  5 2025, 01:23:35) [GCC 14.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> p = 1617549722683965197900599011412144490161
>>> q = 475693130177488446807040098678772442581573

```

Pegamos los demás valores, y verificamos que la factorización este bien. 

```
>>> n = 769457290801263793712740792519696786147248001937382943813345728685422050738403253
>>> c = 8533139361076999596208540806559574687666062896040360148742851107661304651861689
>>> p * q == n
True

```

Aplicamos las otras fórmulas de RSA y desciframos la flag
```
>> tn = (p - 1) * (q - 1)
>>> d = pow(e, -1, tn)
>>> m = pow(c, d, n)
>>> m
13016382529449106065927291425342535437996222135352905256639629442503647501498237
>>> bytes.fromhex(hex(m)[2:])
b'picoCTF{sma11_N_n0_g0od_45369387}'
>>> 

```

flag -> picoCTF{sma11_N_n0_g0od_45369387}