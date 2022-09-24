# Where are the robots

## Descripcion

Can you find the robots? https://jupiter.challenges.picoctf.org/problem/56830/ (link) or 
http://jupiter.challenges.picoctf.org:56830

## Datos acceso

https://jupiter.challenges.picoctf.org/problem/56830/
http://jupiter.challenges.picoctf.org:56830

## Solucion

1.- agregamos la ruta el archivo robots.txt
view-source:https://jupiter.challenges.picoctf.org/problem/56830/robots.txt

```shell

User-agent: *
Disallow: /1bb4c.html
```

2.- despues copeamos el .html a la liga
view-source:https://jupiter.challenges.picoctf.org/problem/56830/1bb4c.html

y obtenemos la flag

```shell
      <div class="content">
	<p>Guess you found the robots<br />
	  <flag>picoCTF{ca1cu1at1ng_Mach1n3s_1bb4c}</flag></p>
      </div>
```

## Referencias

Video de youtube: https://www.youtube.com/watch?v=LRgg3Kcnbuw&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=2
