
## DESCRIPTION

Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames: [Addadshashanammu.zip](https://mercury.picoctf.net/static/a350754a299cb58988d6d47aed5be3ba/Addadshashanammu.zip)

---
## SOLUTION

````
Con el uso de la tecla TAB es muy util para estar navegando entre carpetas y no estar ingresando una por una.

EduardoSanchez-picoctf@webshell:~$ cd Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/

EduardoSanchez-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkal
a/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ file fang-of-haynekhtnamet 
fang-of-haynekhtnamet: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=47e898db922f38cb54ab4a08fb4e3def5a1cb6a1, not stripped
EduardoSanchez-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkal
a/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ ./fang-of-haynekhtnamet 
*ZAP!*

falg -> picoCTF{l3v3l_up!_t4k3_4_r35t!_a00cae70}

```