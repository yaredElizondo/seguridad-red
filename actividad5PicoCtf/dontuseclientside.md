# Dont use client side

Can you break into this super secure portal? 
https://jupiter.challenges.picoctf.org/problem/17682/ (link) or 
http://jupiter.challenges.picoctf.org:17682

## Datos de acceso
https://jupiter.challenges.picoctf.org/problem/17682/

## Solucion
bandera = picoCTF{no_clients_plz_b706c5}

Checamos la logica del split en html

```shell
<script type="text/javascript">
  function verify() {
    checkpass = document.getElementById("pass").value;
    split = 4;
    if (checkpass.substring(0, split) == 'pico') {
      if (checkpass.substring(split*6, split*7) == '706c') {
        if (checkpass.substring(split, split*2) == 'CTF{') {
         if (checkpass.substring(split*4, split*5) == 'ts_p') {
          if (checkpass.substring(split*3, split*4) == 'lien') {
            if (checkpass.substring(split*5, split*6) == 'lz_b') {
              if (checkpass.substring(split*2, split*3) == 'no_c') {
                if (checkpass.substring(split*7, split*8) == '5}') {
                  alert("Password Verified")
                  }
                }
              }
      
            }
          }
        }
      }
    }
    else {
      alert("Incorrect password");
    }
    
  }
</script>

```

## Referencias

youtube: https://www.youtube.com/watch?v=19Hkmb1Guzk&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=4
