# EchoCTF


Algunas cosas que se pudieron aprender de este CTF.


## pii-scammer / 10.0.41.17

![image](https://user-images.githubusercontent.com/63270579/213623630-800000af-fddf-4d88-8dbf-715288ef2a62.png)

Nos damos cuenta que guarda una cookie le hacemos el URL decode y vemos que tiene el user que le ingresamos.


```
{"fullname":"masa","user_id":65}
```

Entonces procedemos a poner el user admin y el id 0 porque en Linux el id de usuario root es 0. Actualizamos la pagina y nos da una flag. Ahora nos dice que revisemos el /admin.php ya que en las headers vemos que esta hecho con PHP 7.x

Modificamos la cookie a admin y nos da el siguiente portal:


![image](https://user-images.githubusercontent.com/63270579/213624700-85e6dc9f-455b-4611-84c6-02ca08f05283.png)

Para borrar toda la base de datos nos damos cuenta que podria ser por SQLi

![image](https://user-images.githubusercontent.com/63270579/213628703-6ea8a349-1835-492e-a4f7-c05419d03c9d.png)


# Challenges

Algunas cosas que se pudieron aprender(nuevas)

## echoCTF Tutorial 101 (ID#1)

El puerto 60213 si te conectas con nc te regresa una consola de python como cuanod pones python3 en la shell.

```
nc 10.100.10.1 6213

#para leer un archivo hacemos.

print (open("flag.txt", "r").read())

# ya sabes para python 3 quita los corchetes.

```



































