Don't power users get tired of making spelling mistakes in the shell? Not anymore! Enter Special, the Spell Checked Interface for Affecting Linux. Now, every word is properly spelled and capitalized... automatically and behind-the-scenes! Be the first to test Special in beta, and feel free to tell us all about how Special streamlines every development process that you face. When your co-workers see your amazing shell interface, just tell them: That's Special (TM)Start your instance to see connection details.

Additional details will be available after launching your challenge instance.

## SOLUTION

````

-- Esto es un entrono especial, ya que tiene algunas restricciones algo diferentes para mi.

Special$ hello
Hello 
sh: 1: Hello: not found

-- Este comando no funciona. 
Special$ $(ls)        
$(ls) 
sh: 1: blargh: not found
blargh.

-- Este comando se puede ejecutar, tiene una sintaxis parecida como uns estructura para evaluar aritmética. Ahi nos muestra la carpeta blargh.  
Special$ ((ls))
((ls)) 
blargh

-- Aqui hacemos una redicrreción en la entrada desde el archivo. 
Special$ ((cat)) < blargh/flag.txt
((cat)) < blargh/flag.txt 
picoCTF{5p311ch3ck_15_7h3_w0r57_f906e25a}
```

