# Lest Warm Up


# Descripcion
If I told you a word started with 0x70 in hexadecimal, what would it start with in ASCII?

## Datos acceso
uso de python para convertir de hex - ascii

## Solucion
```shell
>>> hex_string = "0x70"[2:]
>>> bytes_object = bytes.fromhex(hex_string)
>>> ascii_string = bytes_object. decode("ASCII")
>>> print(ascii_string)
p
>>> 

picoCTF{p}
```

## Referencias

python nivel bits para conversiones