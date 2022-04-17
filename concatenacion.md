## Concatenar :

<pre>La concatenación se puede definir como la integración de dos cadenas en un objeto,
podemos sumar 2 strings con el operador (+).
Tambien podemos formatear una string 
</pre>

``` python
cadena1 = "Hola" 
cadena2 = "mundo" 
nombre = "Juan" 
print(cadena1 , cadena2)
print(cadena1 + cadena2) 
```
``` bash
Hola mundo 
Holamundo 
```
## Formatear string :

<pre>Para formatear una cadena en python hay varias formas pero solo veremos la mas nueva

</pre>
``` python
print(f"{nombre} dice {cadena1} {cadena2}") 
```
``` terminal
Juan dice Hola mundo

```