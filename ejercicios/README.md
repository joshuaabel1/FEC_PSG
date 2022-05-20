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

En el mismo archivo main.py del ejercicio 3, vamos a guardar en una lista los datos de dos personas. Las variables que declaramos antes vamos a guardarlas en un diccionario. El flujo de como encarara el ejercicio (por ahora), sería de la siguiente forma:

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