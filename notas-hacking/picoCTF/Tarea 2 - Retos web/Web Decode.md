
## Description

Do you know how to use the web inspector?

Additional details will be available after launching your challenge instance.

## Hint

Use the web inspector on other files included by the web page.


## Solution

Inspeccionamos el index.html, pero no encuentro nada
En el ABOUT.HTML esta el siguiente mensaje:

```
<h1>
Try inspecting the page!! You might find it there|
</h1>


Y observamos un mensaje posiblemente cifrado

<section class="about" notify_true="cGljb0NURnt3ZWJfc3VjYzNzc2Z1bGx5X2QzYzBkZWRfMDdiOTFjNzl9">



Utilizamos cyberchef para descubrir la flag: 
picoCTF{web_succ3ssfully_d3c0ded_07b91c79}
```