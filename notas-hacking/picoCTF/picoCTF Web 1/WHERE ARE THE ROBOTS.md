
## DESCRIPTION

Can you find the robots? `https://jupiter.challenges.picoctf.org/problem/60915/` ([link](https://jupiter.challenges.picoctf.org/problem/60915/)) or http://jupiter.challenges.picoctf.org:60915


## SOLUTION

````

Nos vamos al archivo robots.txt en la página: 
	https://jupiter.challenges.picoctf.org/problem/60915/robots.txt
Nos muestra esto: 
	User-agent: *
	Disallow: /8028f.html

Lo que vemos en el archivo nos vamos a esa parte del directorio a ver que sale: 
	https://jupiter.challenges.picoctf.org/problem/60915//8028f.html
FLAG -> picoCTF{ca1cu1at1ng_Mach1n3s_8028f}
```