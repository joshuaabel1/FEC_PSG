## Tipos de variables :

    Python tiene cuatro tipos primitivos: enteros, flotantes, booleanos y cadenas o Strings. Los tipos de variables enteros en Python (int) se utilizan para representar datos numéricos, específicamente números enteros. Estos pueden ser tanto positivos como negativos.

### String :
 <pre> Las variables que almacenan texto se denominan strings (str). Tienen que estar entre comillas sencillas(‘) o dobles ("), o si el texto ocupa varias líneas, entre triples comillas dobles (""" """)) . </pre>
``` python
cadena = "Esto es una string" 
print(type(cadena)) 
```
```bash
<class 'str'> 
```

### Int :

<pre> Los números enteros son aquellos que no tienen decimales, tanto positivos como negativos (además del cero). En Python se pueden representar mediante el tipo int (de integer, entero) o el tipo long (largo). La única diferencia es que el tipo long permite almacenarnúmeros más grandes. Es aconsejable no utilizar el tipo long a menos que sea necesario, para no malgastar memoria.
</pre>
``` python
numero_entero = 3 
print(type(numero_entero)) 
```
``` bash
<class 'int'> 
```

### Float :

<pre> Los números reales son los que tienen decimales. En Python se expresan mediante el tipo float. </pre>
``` python
numero_real = 3.2 
print(type(numero_entero)) 
```
``` bash
<class 'float'> 
```


### Complex :

<pre> Los números complejos se componen de una parte real y una parte imaginaria. En Python, la parte imaginaria se puede expresar simplemente agregando una j o una J después del número.
Se puede crear un número complejo fácilmente: asignando directamente la parte real e imaginaria a una variable. El siguiente código de ejemplo demuestra cómo puede crear un número complejo en Python:
</pre>
``` python
numero_complejo = 8 + 5j 
print(type(a)) 
``` bash
<class 'complex'> 
```

### List :

<pre> La lista en Python son variables que almacenan arrays, internamente cada posición puede ser un tipo de datos distinto.
</pre>
``` python
lista = [5, "numero", "clavos"] 
print(type(lista)) 
```
```bash
<class 'list'> 
```

### Tuple :

<pre> Las tuplas son objetos de tipo secuencia, específicamente es un tipo de dato lista inmutable. Esta no puede modificarse de ningún modo después de su creación.

</pre>

``` python
tupla = (5, "numero", "clavos") 

print(type(lista)) 
```
``` bash
<class 'tuple'> 
```

### Range :

<pre> El tipo range() con un único argumento se escribe range(n) y crea una lista inmutable de n números enteros consecutivos que empieza en 0 y acaba en n - 1.
Para ver los valores del range(), es necesario convertirlo a lista mediante la función list(). 
El tipo range con tres argumentos se escribe range(m, n, p) y crea una lista inmutable de enteros que empieza en m y acaba justo antes de superar o igualar a n, aumentando los valores de p en p. Si p es negativo, los valores van disminuyendo de p en p.</pre>
``` python
rango = range() 
print(type(range)) 
```
``` bash
<class 'range'> 
```
### Dict :

<pre> Los diccionarios en Python, al igual que las listas y las tuplas, nos permiten almacenar diferentes tipos de datos: Strings, enteros, flotantes, booleanos, tuplas, listas e inclusive otros diccionarios.
Los diccionario son mutables, es decir, es posible modificar su longitud, podemos agregar o quitar elementos de él; de igual forma todos los valores almacenados en el diccionario pueden ser modificados.
A diferencias de las listas y de las tuplas los diccionarios no se rigen por la regla de los índices, no, nada de eso, en este caso todos los valores que se almacenen en el diccionario no corresponderá a un índice, si no a una llave.
</pre>

``` python
diccionario = {"total": 55} 
print(type(diccionario)) 
```
```bash
<class 'dict'> 
```
### Set :

<pre> Un conjunto es una colección no ordenada de objetos únicos. Python provee este tipo de datos «por defecto» al igual que otras colecciones más convencionales como las listas, tuplas y diccionarios.
Los conjuntos son ampliamente utilizados en lógica y matemática, y desde el lenguaje podemos sacar provecho de sus propiedades para crear código más eficiente y legible en menos tiempo.</pre>
``` python
set = {1, 2, 3, 4} 
print(type(set))
```
``` bash
<class 'set'> 
```

### Bool :

<pre> El tipo booleano sólo puede tener dos valores: True (verdadero) y False (falso). Estos valores son especialmente importantes para las expresiones condicionales y los bucles, como verá más adelante.

</pre>

``` python
afirmacion = True 
print(type(afirmacion)) 
```
``` bash
<class 'bool'> 
```