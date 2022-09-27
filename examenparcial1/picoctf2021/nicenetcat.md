# Nice Net Cat...

## Descripcion
There is a nice program that you can talk to by using this command in a shell: 
$ nc mercury.picoctf.net 43239, but it doesn't speak English...


## Datos de entrada

nc mercury.picoctf.net 43239

## Solucion 

codigo en python funcion

def convert():
nums = [112, 105, 99, 111, 67, 84, 70, 123, 103, 48, 48, 100, 95, 107, 49, 116, 116, 121, 33, 95, 110, 49, 99, 51, 95, 107, 49, 116, 116, 121, 33, 95, 55, 99, 48, 56, 50, 49, 102, 53, 125, 10]
flag = ""
for number in nums:
    flag += chr(number)
print(flag)

convert()

## Referencias
