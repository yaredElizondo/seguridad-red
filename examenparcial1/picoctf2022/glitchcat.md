# Glitch Cat

## Descripcion
Our flag printing service has started glitching!
$ nc saturn.picoctf.net 65353

## Datos de entrada
nc saturn.picoctf.net 65353

## Solucion
```shell

(base) yared@yared-stark:~/Descargas$  nc saturn.picoctf.net 65353
'picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}'
(base) yared@yared-stark:~/Descargas$ python
Python 3.8.8 (default, Apr 13 2021, 19:58:26) 
[GCC 7.3.0] :: Anaconda, Inc. on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print('picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}'
... )
picoCTF{gl17ch_m3_n07_9c42a45d}
>>> exit()
(base) yared@yared-stark:~/Descargas$ 

```

## Referencias
