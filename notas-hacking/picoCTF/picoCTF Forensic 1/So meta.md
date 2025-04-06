
## Description

Find the flag in this [picture](https://jupiter.challenges.picoctf.org/static/89b371a46702a31aa9931a2a2b12f8bf/pico_img.png).

## Hint

What does meta mean in the context of files?


## Solution

Los metadatos son información que describe las características de un archivo, documento, imagen, sin ser parte del contenido principal.

ExifTool es una herramienta para ller, escribir , editar metadatos de un archivo, especialmente imágenes.

```

Le aplicamos un exiftool al archivo pico_img.img

flag-> picoCTF{s0_m3ta_eb36bf44}
```

