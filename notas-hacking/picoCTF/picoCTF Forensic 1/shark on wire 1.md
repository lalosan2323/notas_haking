
## Description

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/483e50268fe7e015c49caf51a69063d0/capture.pcap). Recover the flag.

## Hint

Try using a tool like Wireshark, What are streams?
## Solution

PCAP, es un archivo que contiente los datos de red intercepatados, como si estuvieras "espiando" lo que pasa por una red. Es útil después para ver dispositivos se comunicaron, qué datos se enviaron y cómo lo hicieron.

```

Wireshark en linux es una herramiento de análisis de protocolos de red, permite ver todo el tráfico que pasa por tu red en tiempo real.


Abrimos con wireshark el archivo capture.pcap

Seleccinamos cualquier paquete, y seguimos su stream. Buscamos en las distintas secuancias hasta que aparezca la flag.

flag -> picoCTF{StaT31355_636f6e6e}


```

