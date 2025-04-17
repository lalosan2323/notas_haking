
## Description

Welcome to the challenge! In this challenge, you will explore a web application and find an endpoint that exposes a file containing a hidden flag.The application is a simple blog website where you can read articles about various topics, including an article about API Documentation. Your goal is to explore the application and find the endpoint that generates files holding the server’s memory, where a secret flag is hidden.The website is running [picoCTF News](http://verbal-sleep.picoctf.net:55393/).

## Hint
1. Explore backend development with us
2. The head was dumped

## Solution

Buscamos el endpoint correcto que esta en el enlace de API Documentation en uno de los post. Se lo agregas a la ur [http://verbal-sleep.picoctf.net:58519/heapdum](http://verbal-sleep.picoctf.net:58519/heapdum) y descarga un archivo de una snaphost le haces un cat


```
┌──(lalosan㉿lalosan)-[~]
└─$ cat heapdump-1744853678574.heapsnapshot  | grep picoCTF{
picoCTF{Pat!3nt_15_Th3_K3y_305d5b9a}

``