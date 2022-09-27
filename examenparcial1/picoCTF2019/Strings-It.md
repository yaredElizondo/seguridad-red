# Strings It


# Descripcion
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings) without running it?

## Datos acceso
archivo strings

## Solucion
```shell
┌──(kali㉿kali)-[~/descargas-archivos-ctf]
└─$ strings -f strings | grep picoCTF             
strings: picoCTF{5tRIng5_1T_7f766a23}

```

## Referencias

comandos basicos de uso de string y grep, y comandos en terminal de linux