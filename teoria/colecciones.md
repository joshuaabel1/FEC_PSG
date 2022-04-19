## Colecciones :

<pre>Una colección nos permite agrupar varios objetos bajo un mismo nombre. Por ejemplo, si necesitamos almacenar en nuestro programa los nombres de los alumnos de un curso de programación, será más conveniente ubicarlos a todos dentro de una misma colección de nombre alumnos, en lugar de crear los objetos alumno1, alumno2, etc.

En Python existen tres colecciones básicas, a saber: las listas, las tuplas y los diccionarios .
</pre>

## Listas :

<pre>Una lista es un conjunto ordenado de objetos. Por objetos entendemos cualquiera de los tipos de dato ya mencionados, incluso otras listas.

Para crear una lista, especificamos sus elementos entre corchetes y separados por comas.
</pre>
``` python
lenguajes = ["Python", "Java", "C", "C++"]
``` 

## Tuplas :

<pre>Las tuplas, al igual que las listas, son colecciones ordenadas. No obstante, a diferencia de éstas, son inmutables. Es decir, una vez asignados los elementos, no pueden ser alterados. En términos funcionales, podría decirse que las tuplas son un subconjunto de las listas, por cuanto soportan las operaciones con índices para acceder a sus elementos, pero no así las de asignación.
</pre>
``` python
lenguajes = ("Python", "Java", "C", "C++")
```

## Diccionarios :

<pre>Los diccionarios, a diferencia de las listas y las tuplas, son colecciones no ordenadas de objetos. Además, sus elementos tienen una particularidad: siempre conforman un par clave-valor. Es decir, cuando añadimos un valor a un diccionario, se le asigna una clave única con la que luego se podrá acceder a él (pues la posición ya no es un determinante).
Para crear un diccionario, indicamos los pares clave-valor separados por comas y estos, a su vez, separados por dos puntos.
</pre>

``` python
d = {"Python": 1991, "C": 1972, "Java": 1996} 
```