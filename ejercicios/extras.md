# Ejercicios de refuerzo 💪🏼

A pedido de varios, vamos a dar más ejercicios para practicar. Vamos a dividir en 3 niveles:

- `Fácil`: Ideal para los que recién empiezan o quieren repasar lo básico. No implica mucho desarrollo en cada ejercicio.
- `Intermedio`: Acá va a requerir un poco más de investigación, sin mucha ayuda de parte nuestra en las consignas.
- `Javo`: Por qué el nombre? Según dicen que yo (Javo) hago ejercicios difíciles, así que vamos a nombrar este nivel como "Javo". Va a requerir un adicional de esfuerzo y elaborar mayor cantidad de scripts (acá ya no van a ser solo uno o dos archivos Python). Con qué se pueden encontrar? Uso de librerías, consumo y elaboración de APIs, uso de bases de datos (relacionales y no relacionales), etc.

A continuación, encontrar los ejercicios enumerados. Recomendamos crear distintas carpetas, aunque tal vez alguno requiera hacerlo por separado en un entorno aislado (la mayoría de los de nivel "Javo"). Éxitos!

## 😀Fácil

### Ejercicio 1
Escribir una función a la que se le pase una cadena <nombre> y muestre por pantalla el saludo ¡hola <nombre>!.

### Ejercicio 2
Realizar lo mismo del ejercicio 1, pero dentro de una función, agregando en otra línea de la terminal la cantidad de caracteres que tiene el nombre.

Ejemplo de salida:
> ¡hola Joshua!

> Tu nombre tiene 6 letras!

### Ejercicio 3
La pizzería Bella Napoli ofrece pizzas vegetarianas y no vegetarianas a sus clientes. Los ingredientes para cada tipo de pizza aparecen a continuación.

- Ingredientes vegetarianos: Pimiento y tofu.
- Ingredientes no vegetarianos: Peperoni, Jamón y Salmón

Escribir un programa que pregunte al usuario si quiere una pizza vegetariana o no, y en función de su respuesta le muestre un menú con los ingredientes disponibles para que elija. Solo se puede eligir un ingrediente además de la mozzarella y el tomate que están en todas la pizzas. Al final se debe mostrar por pantalla si la pizza elegida es vegetariana o no y todos los ingredientes que lleva.

### Ejercicio 4
Escribir un programa que pida al usuario su peso (en kg) y estatura (en metros), calcule el índice de masa corporal y lo almacene en una variable, y muestre por pantalla la frase "Tu índice de masa corporal es <imc>", donde <imc> es el índice de masa corporal calculado redondeado con dos decimales

### Ejercicio 5
Escribir un programa que pregunte los nombres y apellidos del usuario en la consola y después muestre por pantalla el nombre completo del usuario tres veces:

- Una con todas las letras minúsculas
- Otra con todas las letras mayúsculas
- Y otra solo con la primera letra del nombre y de los apellidos en mayúscula.

El usuario puede introducir su nombre combinando mayúsculas y minúsculas como quiera.

### Ejercicio 6
Realizar una calculadora básica (suma, resta, producto y división), implementado solamente condicionales if..elif...else.

Ejemplo del resultado:
> Ingrese un número: 5

> Ingrese otro número: 2

> Elegir operación (S/R/P/D): R

> El resultado es 3

# Ejercicio 7
Dado el siguiente listado de libros

```py
libros = [
    'Don Quijote de la Mancha',
    'Historia de dos ciudades',
    'El Señor de los Anillos',
    'El principito',
    'El hobbit',
    'Sueño en el pabellón rojo',
    'Las aventuras de Alicia en el país de las maravillas',
    'Triple representatividad,',
    'Y no quedó ninguno (Diez negritos)',
    'El león, la bruja y el armario'
]
```
Desarrolla un programa el cual cumpla con los siguiente requerimientos.

- El programa listará en consola todos los elementos de la lista.
- El usuario podrá seleccionar (mediante un número) un libro en especifico.
- En caso el usuario ingrese un número mayor a la cantidad de libros en el listado, el programa deberá mostrar en consola el siguiente mensaje:
- Indice no disponible

Ejemplo:

```
1º- Don Quijote de la Mancha
2º- Historia de dos ciudades
3º- El Señor de los Anillos
4º- El principito
5º- El hobbit
6º- Sueño en el pabellón rojo
7º- Las aventuras de Alicia en el país de las maravillas
8º- Triple representatividad,
9º- Y no quedó ninguno (Diez negritos)
10º- El león, la bruja y el armario

Selecciona un libro: 10
El león, la bruja y el armario
```
Ayuda: En Python más vale pedir perdón que pedir permiso.

Deseado:

- Sería estupendo que la enumeración que el usuario visualizará en consola comenzará desde 1 y no desde 0.
- Si tienes tiempo y así lo deseas, sería un muy buena idea validar que el usuario solo pueda introducir números.

# Ejercicio 8
Dada la siguiente clase

```py
class Animal():

    def comer(self):
        print('El animal come.')

    def dormir(self):
        print('El animal duerme.')
```

Define dos nuevas clases (Perro, Gato) que hereden de la clase Animal. Las clases hijas debe ser capaces de sobre escribir los métodos de la clase padre (Animal)

- La clase Perro deberá imprimir en consola: el Perro Come y el Perro Duerme para los métodos comer y dormir respectivamente.
- La clase Gato deberá imprimir en consola: el Gato Come y el Gato Duerme para los métodos comer y dormir respectivamente.

Ejemplo:

```
>>> gato.comer()
El Gato come.

>>> perro.dormir()
El Perro duerme.
```

### Ejercicio 9
Dado un diccionario de usuarios con sus respectivas edades. Ejemplo:

```py
usuarios = [
    {'username':  'Eduardo', 'age': 27 },
    {'username':  'Fernando', 'age': 25 },
    {'username':  'Loki', 'age': 30 },
    {'username':  'Duke', 'age': 19}
]
```

Desarrolla un programa en Python que muestre en consola el nombre de todos los usuarios con una edad mayor a 25.

Salida: 

```
Eduardo
Loki
```

## 🤨 Intermedio

### Ejercicio 1
En una determinada empresa, sus empleados son evaluados al final de cada año. Los puntos que pueden obtener en la evaluación comienzan en 0.0 y pueden ir aumentando, traduciéndose en mejores beneficios. Los puntos que pueden conseguir los empleados pueden ser 0.0, 0.4, 0.6 o más, pero no valores intermedios entre las cifras mencionadas. A continuación se muestra una tabla con los niveles correspondientes a cada puntuación. La cantidad de dinero conseguida en cada nivel es de 2.400€ multiplicada por la puntuación del nivel.

| Nivel        |   Puntuación |
|--------------|--------------|
| Inaceptable  |   0.0        |
| Aceptable    |   0.4        |
| Meritorio    |   0.6 o más  |

Escribir un programa que lea la puntuación del usuario e indique su nivel de rendimiento, así como la cantidad de dinero que recibirá el usuario

### Ejercicio 2
A partir del siguiente listado de usuarios. Desarrolla un programa el cual nos permita crear un archivo .json.

El programa debe cumplir con los siguiente requerimientos.

- El programa debe ser capaz de generar el archivo users.json.
- El archivo debe poseer los 200 usuarios del listado en un formato json.
- Cada objeto json debe encontrarse identado por 4 espacios.

Ejemplo:
```json
[
    {
        "age": "73",
        "country": "United States",
        "email": "jerome.thomas@example.com",
        "gender": "male",
        "id": "0",
        "name": "Mr Jerome Thomas"
    },
    {
        "age": "70",
        "country": "United Kingdom",
        "email": "gary.berry@example.com",
        "gender": "male",
        "id": "1",
        "name": "Mr Gary Berry"
    },
...
]
```

Ayuda: vas a tener que usar la librería `json`! Es posible sin, pero va a ser más complicado.

### Ejercicio 3
Desarrolla una función que nos permita conocer todas las llaves duplicadas dentro de 2 diccionarios.

La función deberá cumplir con los siguientes aspectos.

- La función deberá tener por nombre common_keys.
- La función deberá recibir, de forma obligatoria, dos diccionarios como argumentos.
- La función deberá retornará una tupla con todas las llaves duplicadas dentro de los diccionarios ingresados.

Ejemplo:

```
>>> a = {'a': 10, 'b':20, 'c':30}
>>> b = {'a': 10, 'c': 30, 'd': 40}

>>> common_keys(a, b)
('a', 'c')
```

## 🤯 Javo

Pronto 😛