## Operadores aritméticos :
<pre> Estos son los operadores que permiten realizar diferentes operaciones aritméticas .
</pre>

``` python
x = 7

y = 2
```
``` python
print(x + y)  # Suma dos operandos .
```
``` bash
9
```
``` pytohn
print(x - y)  # Resta al operando de la izquierda el valor del operando de la derecha. Utilizado sobre un único operando, le cambia el signo .
```
``` bash
5
```
``` python
print(x * y)  # Producto/Multiplicación de dos operandos .
```
``` bash
14
```
``` python
print(x / y)  # Divide el operando de la izquierda por el de la derecha (el resultado siempre es un float) .
```
``` bash
3.5
```
``` python
print(x % y)  # Operador módulo. Obtiene el resto de dividir el operando de la izquierda por el de la derecha .
```
``` bash
1
```
``` python
print(x // y)  # Obtiene el cociente entero de dividir el operando de la izquierda por el de la derecha .
```
``` bash
3
```
``` python
print(x ** y)  # Potencia. El resultado es el operando de la izquierda elevado a la potencia del operando de la derecha .
```
``` bash
49
```

## Operadores de comparación :

<pre> Los operadores de comparación se utilizan, como su nombre indica, para comparar dos o más valores. El resultado de estos operadores siempre es True o False . 
</pre>
``` python
( " > " ) # Mayor que. True si el operando de la izquierda es estrictamente mayor que el de la derecha; False en caso contrario .

(" >= ") # Mayor o igual que. True si el operando de la izquierda es mayor o igual que el de la derecha; False en caso contrario .

(" < ") # Menor que. True si el operando de la izquierda es estrictamente menor que el de la derecha; False en caso contrario .

(" <= ") # Menor o igual que. True si el operando de la izquierda es menor o igual que el de la derecha; False en caso contrario .

(" == ") # Igual. True si el operando de la izquierda es igual que el de la derecha; False en caso contrario .

(" != ") # Distinto. True si los operandos son distintos; False en caso contrario .

```

## Operadores de pertenencia :

<pre> Los operadores de pertenencia se utilizan para comprobar si un valor o variable se encuentran en una secuencia (list, tuple, dict, set o str). </pre>

``` python
in # Devuelve True si el valor se encuentra en una secuencia; False en caso contrario .

not in # Devuelve True si el valor no se encuentra en una secuencia; False en caso contrario .
```
## Operadores de identidad :

<pre>Por último, los operadores de identidad se utilizan para comprobar si dos variables son, o no, el mismo objeto .
</pre>
``` python
is # Devuelve True si ambos operandos hacen referencia al mismo objeto; False en caso contrario 

is not # Devuelve True si ambos operandos no hacen referencia al mismo objeto; False en caso contrario .

```