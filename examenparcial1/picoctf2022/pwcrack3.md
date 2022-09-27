# PW crack 3

## Descripcion
Can you crack the password to get the flag?
Download the password checker here and you'll need the encrypted flag and the hash in the same directory too.
There are 7 potential passwords with 1 being correct. You can find these by examining the password 
checker script.

## Datos de entrada

level3.py 
"" "".hash
"" "".enc

## Solucion

modificamos la funcion para hacer un ciclo for y solo pruebe las combinaciones
de las contras

def level_3_pw_check(user_pw):
  6     #user_pw = input("Please enter correct password for flag: ")
  5     user_pw_hash = hash_pw(user_pw)
  4     #print(correct_pw_hash)
  3     #print(str(flag_enc.decode(),user_pw))
  2     if( user_pw_hash == correct_pw_hash ):
  1         print("Welcome back... your flag, user:")
33          decryption = str_xor(flag_enc.decode(), user_pw)
  1         print(decryption)
  2         return
  3     print("That password is incorrect")
  4 
  5 
  6 
  7 #level_3_pw_check()
  8 
  9 # The strings below are 7 possibilities for the correct password. 
 10 #   (Only 1 is correct)
 11 pos_pw_list = ["8799", "d3ab", "1ea2", "acaf", "2295", "a9de", "6f3d"]
 12 
 13 for i in pos_pw_list:
 14     level_3_pw_check(i)


```shell

(base) yared@yared-stark:~/Descargas$ python level3.py 
That password is incorrect
That password is incorrect
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_6f98a49f}
That password is incorrect
That password is incorrect
That password is incorrect
That password is incorrect
```

## Referencias

