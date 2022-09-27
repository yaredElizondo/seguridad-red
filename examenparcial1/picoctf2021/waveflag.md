# Wave a flag

## Descripcion
Can you invoke help flags for a tool or binary? This program has extraordinarily helpful information...

## Datos acceso
chmod
file

## Solucion
```shell
(base) yared@yared-stark:~/notas-examen-seguridadredes/picoctf-2021$ ./warm
bash: ./warm: Permiso denegado
(base) yared@yared-stark:~/notas-examen-seguridadredes/picoctf-2021$ chmod +x warm
(base) yared@yared-stark:~/notas-examen-seguridadredes/picoctf-2021$ ./warm
Hello user! Pass me a -h to learn what I can do!
(base) yared@yared-stark:~/notas-examen-seguridadredes/picoctf-2021$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_755f3544}
(base) yared@yared-stark:~/notas-examen-seguridadredes/picoctf-2021$ 

```

## Referencias

Uso del chmod para dar permisos
Uso del ./ para ejecutar un programa
