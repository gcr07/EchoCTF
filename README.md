# EchoCTF


Algunas cosas que se pudieron aprender de este CTF.


## pii-scammer / 10.0.41.17

![image](https://user-images.githubusercontent.com/63270579/213623630-800000af-fddf-4d88-8dbf-715288ef2a62.png)

Nos damos cuenta que guarda una cookie le hacemos el URL decode y vemos que tiene el user que le ingresamos.


```
{"fullname":"masa","user_id":65}
```

Entonces procedemos a poner el user admin y el id 0 porque en Linux el id de usuario root es 0.







































