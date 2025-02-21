
## DESCRIPTION
Find the flag in the Python script![Download Python script](https://artifacts.picoctf.net/c/35/serpentine.py)

## HINT
Try running the script and see what happens

## SOLUTION

````

Este programa al momento de ejecutarlo, nos trolea ya que al presionar b no imprime la flag. Tuve que modificar el .py con el comando nano, en la condición cuando es == 'b', mande a llamar el método print_flag()


flag-> picoCTF{7h3_r04d_l355_7r4v3l3d_ae0b80bd}
```