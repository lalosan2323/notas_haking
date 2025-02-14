## DESCRIPTION

There is a nice program that you can talk to by using this command in a shell: `$ nc mercury.picoctf.net 35652`, but it doesn't speak English...

## HINT

You can practice reading and writing ASCII with this picoGym problem: [Let's Warm Up](https://play.picoctf.org/practice/challenge/22)

# SOLUTION

````
nc mercury.picoctf.net 35652` nos conectamos. Nos arroja la siguiente salida: Nos pide encontrar los carácteres, ya que se encuantra en ASCII de modo de practica.  
112 -> p
105 -> i
99 -> c
111 -> o
67 -> C
84 -> T
70 -> F
123 -> {
103 -> g
48 -> 0
48 -> 0
100 -> d
95 -> -
107 -> k
49 -> 1
116 -> t
116 -> t
121 -> y
33 ->!
95 -> -
110 -> n
49 -> 1
99 -> c
51 -> 3
95 -> -
107 -> k
49 -> 1
116 -> t
116 -> t
121 -> y
33 -> !
95 -> -
57 -> 9
98-> b
51-> 3
98-> b
55-> 7
51-> 3
57-> 9
50-> 2
125-> }
10-> Es un salto de linea
```

FLAG -> picoCTF{g00d_k1tty!_n1c3_k1tty!_9b3b7392}