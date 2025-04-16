
## Description

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). Recover the flag that was pilfered from the network.

## Solution

1. Se va utilizar la herramienta scapy (paquete para el análisis, manipulación, y creación de paquetes de red)  , que nos a ayudar a automatizar la extracción de la bandera. 
2. ![[Pasted image 20250415205007.png]]
El código recorre cada paquete, y si el destino es el puerto 22, y el puerto es mayor a 5000, **0**, toma la diferencia entre el puerto de origen y 5000, la convierte en un carácter usando chr y la añade a una cadena.
3. flag-> picoCTF{p1LLf3r3d_data_v1a_st3g0}
