# PW crack 1

## Descripcion
Can you crack the password to get the flag?
Download the password checker here and you'll need the encrypted flag in the same directory too.

## Datos de entrada

level1.py
level1.flag.txt.enc

## Solucion
```shell
(base) yared@yared-stark:~/Descargas$ python level1.py 
Please enter correct password for flag: 
That password is incorrect
(base) yared@yared-stark:~/Descargas$ cat level1.py 
### THIS FUNCTION WILL NOT HELP YOU FIND THE FLAG --LT ########################
def str_xor(secret, key):
    #extend key to secret length
    new_key = key
    i = 0
    while len(new_key) < len(secret):
        new_key = new_key + key[i]
        i = (i + 1) % len(key)        
    return "".join([chr(ord(secret_c) ^ ord(new_key_c)) for (secret_c,new_key_c) in zip(secret,new_key)])
###############################################################################


flag_enc = open('level1.flag.txt.enc', 'rb').read()



def level_1_pw_check():
    user_pw = input("Please enter correct password for flag: ")
    if( user_pw == "8713"):
        print("Welcome back... your flag, user:")
        decryption = str_xor(flag_enc.decode(), user_pw)
        print(decryption)
        return
    print("That password is incorrect")



level_1_pw_check()
(base) yared@yared-stark:~/Descargas$ ptyhon level1.py level1.flag.txt.enc 
ptyhon: orden no encontrada
(base) yared@yared-stark:~/Descargas$ python level1.py level1.flag.txt.enc 
Please enter correct password for flag: 8713
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_1b2fd683}
(base) yared@yared-stark:~/Descargas$ 
```

## Referencias
