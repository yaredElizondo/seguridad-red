# Plumbing

## Descripcion
Sometimes you need to handle process data outside of a file. 
Can you find a way to keep the output from this program 
and search for the flag? 
Connect to jupiter.challenges.picoctf.org 4427.

## Datos acceso

host -> jupiter.challenges.picoctf.org
port -> 4427


## Solucion
```shell
┌──(kali㉿kali)-[~]
└─$ nc jupiter.challenges.picoctf.org 4427 | grep picoCTF
picoCTF{digital_plumb3r_5ea1fbd7}


```

## Referencias

uso del grep 
uso del nc para acceder al host

