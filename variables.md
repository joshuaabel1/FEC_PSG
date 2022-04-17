

## Variables :

    Es un nombre que se refiere a un objeto que reside en la memoria. 
    El objeto puede ser de alguno de los tipos vistos (número o cadena de texto), 
    o alguno de los otros tipos existentes en Python.

    Cada variable debe tener un nombre único llamado identificador. 
    Eso es muy de ayuda pensar las variables como contenedores que 
    contienen data el cual puede ser cambiado después a través de 
    técnicas de programación.

``` python 
saludo = "Hola Mundo" # cadenas de caracteres 
print(saludo) 
 ```
 ``` bash
hola mundo
```



## Alcance de las variables :

    Las variables en Python son locales por defecto. Esto quiere decir que las variables definidas y utilizadas en el bloque de código de una función, sólo tienen existencia dentro de la misma, y no interfieren con otras variables del resto del código.

    A su vez, las variables existentes fuera de una función, no son visibles dentro de la misma.

    En caso de que sea conveniente o necesario, una variable local puede convertirse en una variable global declarándola explícitamente, como tal con la sentencia global.


## asignar múltiples valores a a múltiples variables

    A continuación, se creará múltiples variables (entero, coma flotante, cadenas de caracteres) asignando múltiples valores:
    
``` python
a, b, c = 5, 3.2, "Hola" 

print(a) 
print(b) 
print(c)
```
``` bash
5 
3.2
'Hola'
```
## Reglas y convención de nombres :

    Algunas reglas y convenciones de nombres para las variables y constantes:

   * Nunca use símbolos especiales como !, @, #, $, %, etc.

   * El primer carácter no puede ser un número o dígito.

   * Las constantes son colocadas dentro de módulos Python y significa que no puede ser cambiado.

   * Los nombres de constante y variable debería tener la combinación de letras en minúsculas (de a a la z) o MAYÚSCULAS (de la A a la Z) o dígitos (del 0 al 9) o un underscore (_). Por ejemplo:

        - snake_case
        - MACRO_CASE
        - camelCase
        - CapWords
        - Los nombres que comienzan con guión bajo (simple _ o doble __) se reservan para -  variables con significado especial

   *  No pueden usarse como identificadores, las palabras reservadas .

##   Sentencia global :

    No tenemos que declarar explícitamente las variables antes de usarlas, por lo tanto, para diferenciar entre una variable local y una global, necesitamos especificar que la variable a la que estamos accediendo es la variable global o no. Podemos especificar una variable como global en Python usando la palabra clave

 ``` python
global saludo 
 ```
    
    ahora esta misma variable, podra usarse para todo el bloque de codigo .