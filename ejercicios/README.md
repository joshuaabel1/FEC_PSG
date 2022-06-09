# Ejercicios 💪🐍

## Ejercicio 1

Crear un entorno virtual de Python en cualquier versión e instalar dos librerías:
Una la instalaremos mediante pip: `pip install matplotlib`
Otra la instalaremos mediante un archivo llamado requirements.txt en la raíz de la carpeta. Dentro, van a poner: `pandas==1.4.2`. Luego, en consola, tipean: `pip install -r requirements.txt`
Chequeen que, dentro del entorno, hayan podido instalar estas dos librerías


## Ejercicio 2

Crear un archivo main.py que guarde las siguientes variables:
- first_name
- last_name
- age
- country
- hobby

Pedir estas variables mediante consola, usando la función input. Ejemplo de uso:
```py
first_name = input('Ingrese su nombre: ')
```

Cuidado! Esta función input por defecto guarda todo en formato string. Para la edad deberíamos guardalo como tipo int (entero). Averiguar como cambia de tipo en Python!


## Ejercicio 3

En el mismo archivo main.py del ejercicio 2, vamos a guardar en una lista los datos de dos personas. Las variables que declaramos antes vamos a guardarlas en un diccionario. El flujo de como encarara el ejercicio (por ahora), sería de la siguiente forma:

- Pido datos y guardo en diccionario usuario1
- Pido otra vez datos y guardo en diccionario usuario2
- Guardar usuario1 y usuario2 en una lista usuarios


## Ejercicio 4

Estamos participando de una encuesta telefónica y nos piden nuestros datos para poder realizar cierto análisis de datos. El operador ingresa los datos recolectados, las cuales tienen las siguientes temáticas: identidad (`full_name`), cantidad de autos (`cars`) y monotributista (`is_contributor`). Vemos que la carga de datos tiene una falla y viene de la siguiente forma:

```py
data = {
    "full_name": "Javo",
    "cars": 1,
    "is_contributor": True
    "sarasa": "123312312amlsdalsld" # NO VA
    "children": 0, # NO VA
}
```


A nosotros solamente nos interesa los datos anteriormente mencionados, por lo que necesitamos hacer lo siguiente:

- Utilizar la variable data (inicialmente viene con las keys `sarasa` y `children`) y almacenar los datos de la encuesta.
- Crear una nueva variable `data_parsed` con los datos de interés de la encuesta.
- Limpiar la variable `data` y mostrar `data_parsed` en consola.


## Ejercicio 5

El que realiza la encuesta, no coordinó con los otros censistas y encuestaron a algunas personas por segunda vez. Es entonces que necesitamos tomar alguna estrategia para limpiar datos.
Para que no vuelva a suceder lo mismo, en una variable almacenamos, por cada encuesta, solamente el valor del nombre (`full_name`). Esto quiere decir que tendremos una serie de nombres que tomaremos de referencia para filtrar datos repetidos (disclaimer: esto no lo hagan en un proyecto real, es solamente para facilitar el ejercicio).

En resumen, la estrategia consta de:

- Por cada encuesta realizada, a demás de hacer todo lo del ejercicio 4, también guardaremos en una lista el nombre de cada encuestado. El nombre de la lista puede llamarse `list_names`.
- Necesitamos saber cuantos encuestados hay en total e imprimirlo en consola.


## Ejercicio 6

Se ingresa por consola día y mes. Crear un script que pueda decirnos si es navidad! 🎅🎄.

Para esto, van a tener que usar una librería llamada datetime. Pueden usar lo siguiente para obtener día y mes actual:

```py
from datetime import datetime as dt

actual = dt.now()
actual_day = actual.day # Día
actual_month = actual.month # Mes
```

## Ejercicio 7

En un país, por la crisis económica, se optó por el racionamiento de alimentos. Los criterios son los siguientes:

- Los días lunes solo se pueden presentar a comprar los DNI terminados en 0 y 1
- Los días martes solo se pueden presentar a comprar los DNI terminados en 2 y 3
- Los días miércoles solo se pueden presentar a comprar los DNI terminados en 4 y 5
- Los días jueves solo se pueden presentar a comprar los DNI terminados en 6 y 7
- Los días viernes solo se pueden presentar a comprar los DNI terminados en 8 y 9
- Los fines de semana, el acceso es ilimitado

Imprimir si la persona con el DNI ingresado en el sistema puede ingresar o no al establecimiento. Pueden usar el script del ejercicio 6, queda por averiguar como conseguir el nombre del día con la librería datetime!


## Ejercicio 8

A partir de una lista desordenada de números enteros, se pide (USAR BUCLE FOR):

- Separar en dos listas: una para números pares y otra para números impares
- En la lista de pares, ordenar de menor a mayor
- En la lista de impares, ordenar de mayor a menor

Ejemplo:

```py
numbers = [6, 2, 1, 4, 9, 33, 11, 24]

# Ouput
# Pares: [2, 4, 6, 24]
# Impares: [33, 11, 9, 1]
```

Usar las siguientes listas:
```py
[32, 21, 26, 80, 76, 46, 75, 58, 38, 51, 47]
[62, 60, 44, 22, 57, 21, 13, 39, 47, 74, 87, 69, 4, 1, 83, 42, 12, 12, 64]
[34, 65, 61, 81, 49, 94, 96, 54, 74, 42, 82, 0, 98, 59, 62, 94, 83, 60, 54, 10, 36, 81, 92, 3, 76]
[]
```

## Ejercicio 9

Dejamos de ser programadores y ahora seremos repositores en un supermercado. Nos pasan una lista de productos que faltan en las góndolas y nosotros como buenos repositores, iremos a llenar las góndolas.

```py
productos_faltantes = [
    {
        'name': 'Arroz',
        'checked': False
    },
    {
        'name': 'Cereal',
        'checked': False
    },
    {
        'name': 'Bondiola',
        'checked': False
    },
    {
        'name': 'Café',
        'checked': False
    },
    {
        'name': 'Yerba',
        'checked': False
    }
]
```

Lamentablemente, no tenemos todos los productos de la lista en el almacen. Durante la mañana solamente podemos completar parte de las góndolas y luego por la tarde traerán los productos que faltan para llenar las góndolas.

Con esto dicho, volveremos a nuestro rol de programadores y vamos a crear un script (usando while y for) para cambiar el estado (`checked`) de cada producto en nuesta lista de diccionarios.

Tip: usar el método input para indicar al script cuando llenamos la góndola de un producto y usar break para cortar el while (o sea, siempre va a iterar hasta que todos los productos estén con `checked = True`)


## Ejercicio 10

Teniendo el ejercicio 3 hecho, queremos adaptarlo para poder utilizar funciones. La idea es ingresar N cantidad de usuarios en una lista. Para esto, se pide primero ingresar un valor N, la cual representará las veces que se ingresa un usuario nuevo.
Al final de la iteración, se deberán imprimir el nombre (`first_name`) de cada usuario.


## Ejercicio 11

Crear una función que convierta un número ingresado (entero y positivo) al sistema binario ([acá tienen una explicación de como hacerlo matemáticamente](https://www.cuemath.com/numbers/decimal-to-binary/)). Pueden devolver el resultado como string para facilitar el resultado de la conversión.

Plus: Hacer lo mismo pero para sistema octal y hexadecimal!
