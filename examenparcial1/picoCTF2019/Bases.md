# Bases


# Descripcion
What does this `bDNhcm5fdGgzX3IwcDM1` mean? I think it has something to do with bases.

## Datos acceso
data =  "bDNhcm5fdGgzX3IwcDM1" 

## Solucion
```shell
┌──(kali㉿kali)-[~/descargas-archivos-ctf]
└─$ echo "bDNhcm5fdGgzX3IwcDM1" | base64 -d  
l3arn_th3_r0p35                                                                   
```

## Referencias
uso del echo y de base64 linux
https://linuxhint.com/bash_base64_encode_decode/
