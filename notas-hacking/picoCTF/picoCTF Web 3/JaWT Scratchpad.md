## DESCRIPTION
Check the admin scratchpad! `https://jupiter.challenges.picoctf.org/problem/58210/` or http://jupiter.challenges.picoctf.org:58210
## HINT
What is that cookie?

Have you heard of JWT?

## SOLUTION

los JWT son una forma eficiente y segura de transmitir información entre partes, especialmente en aplicaciones web y API.

Nos vamos al link antes mencionado.

![[Pasted image 20250402164714.png]]
Entro a la aplicación con mi  nombre, ya que con  admin no se puede por que es especial. 



![[Pasted image 20250402171450.png]]
pegamos la cookie generada en un archivo hash. Vamos a intentar crackearla con  un ataque de diccionario.

````

john hash -w-/usr/share/wordlists/rockyou.txt

Se aplica un john the ripper al archivo hash. Se obsera que se usa la palabra ilovepico.




Me voy JWT.IO.

En la parte de playload cambio el user -> admin.
Y en verify signature -> ilovepico


cokie modificada -> eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VyIjoiYWRtaW4ifQ.gtqDl4jVDvNbEe_JYEZTN19Vx6X9NNZtRVbKPBkhO-s


picoCTF{jawt_was_just_what_you_thought_44c752f5}
````
