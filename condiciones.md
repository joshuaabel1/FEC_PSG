
## Control de flujo :

<pre>Un programa o script de Python es un conjunto de instrucciones analizadas y ejecutadas por el intérprete de arriba hacia abajo y de izquierda a derecha. Cuando todas las instrucciones se han ejecutado, el programa termina. No obstante, contamos con herramientas para alterar el flujo natural del programa: hacer que se saltee una porción de código según se cumpla tal o cual condición, repetir un conjunto de instrucciones, etc.</pre>

## Conciciones :

<pre> Las condiciones son las palabras reservadas con las cuales le decimos a 
Python que deseamos que se muestre, la palabra "if" es con la que indicaremos
que si se cumple la condicion ejecutaremos el siguiente codigo .
</pre>

``` python
edad = 30

if edad >= 18: 
    print("Eres un adulto.") 
```
``` bash
Eres un adulto.
```

<pre> Si la variable definida cumple con la condicion impuesta, ejecutaremos el siguiente codigo.
Como se ver dejamos dejamos unos espacios esto se llama indentacion es parte de las reglas de python .
</pre>

<pre> Para ejecutar un bloque de codigo en caso de que no se cumpla la condición,
usamos la palabra reservada "else" .
</pre>

``` python
if edad >= 18:
    print("Eres un adulto.")
    
else:
    print("Aún no eres un adulto.")
```

<pre> Por último, podemos especificar otras condiciones en caso que la primera no se cumpla vía elif. </pre>

``` python
if edad >= 18 and edad < 65:
    print("Eres un adulto.")
elif edad >= 65:
    print("Eres un adulto mayor.")
else:
    print("Aún no eres un adulto.")
```