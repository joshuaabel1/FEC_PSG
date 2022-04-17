## Bucles :

<pre> Los bucles osn otra herramiente usada para alterar el flujo de nuestro
programa podes repetir una porcion de codigo las veces que querramos .
Python incluye únicamente dos tipos de bucle: while y for .</pre>

## Bucle while :

<pre>La palabra reservada while ejecuta una porción de código una y otra vez hasta que la condición especificada sea falsa; o, dicho de otro modo, ejecuta una porción de código mientras que la condición sea verdadera.
</pre>
``` python
a = 1

while a < 10:

    print("¡Hola, mundo!")

    a = a + 1
```

## Bucle for :

<pre>El bucle for ejecuta el bloque de código indentado (en este caso la llamada a print()) tantas veces como elementos haya en la colección indicada a la derecha del operador in. Pero, cada vez que ese código es ejecutado, la variable lenguaje tendrá un valor diferente: en la primera ejecución será igual a "Python"; en la segunda, a "C"; y así hasta alcanzar el final de la lista
</pre>

``` bash python 

lenguajes = ["Python", "C", "C++", "Java"]

for lenguaje in lenguajes:

    print(lenguaje)
```