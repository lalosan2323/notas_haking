
## Description

Can you get the flag?

Additional details will be available after launching your challenge instance.

Go to this [website](http://saturn.picoctf.net:52908/) and see what you can discover.

## Hint
How is the password checked on this website?

## Solution



Nos logueamos, e inspeccionamos el html. Observamos que hay un archivo secure.js que nos muestra el siguiente código: 
```
  
function checkPassword(username, password)
{
  if( username === 'admin' && password === 'strongPassword098765' )
  {
    return true;
  }
  else
  {
    return false;
  }
}
```

Nos volvemos a loguear. 

flag-> picoCTF{j5_15_7r4n5p4r3n7_b0c2c9cb}

