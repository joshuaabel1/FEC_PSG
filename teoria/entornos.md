### 📚 Recursos:
- [Entornos virtuales de Python explicados con ejemplos](https://www.freecodecamp.org/espanol/news/entornos-virtuales-de-python-explicados-con-ejemplos/)

- [Entornos Virtuales con Python (Módulo virtualenv) ✅ | Curso Python 3 🐍 # 63](https://www.youtube.com/watch?v=TNtrAvNNxTY)

- [Pipenv: Flujo de trabajo en Python para humanos.](https://pipenv-es.readthedocs.io/es/latest/)

# 📦 Entornos virtuales

A los entornos virtuales lo podemos pensar como directorios aislados, estos crean una version de Python independiente de la que usamos en nuestro sistema operativo . Libre de las dependencias usadas en el mismo. 

## ¿Por qué existen?

Estos nos dan la oportunidad de trabajar distintas versiones de nuestras librerias, pensemos en la ocasion en que usemos pymongo la version actual de esta libraria es la 4.2 para fast api, pero la misma no esta todavia totalmente intregada con algunas versiones de las librerias en Django entonces debemos usar una version anterior como la 3.2 

## ¿Cómo genero un entorno virtual?

> Si tienes Windows y usas Powershell, deberás habilitar la ejecución de scripts:

```sh
Get-ExecutionPolicy
Set-ExecutionPolicy unrestricted
```

Tanto para Linux, Windows o Mac, proseguimos de la siguiente forma:

```sh
pip install virtualenv # Instalamos la librería

python -m virtualenv venv # Creamos el entorno virtual y la llamamos venv

source venv/bin/activate # Activamos el entorno. En Windows es: venv/Scripts/activate

deactivate # Para desactivar el entorno
```

Dentro del entorno activado, podremos instalar todas las dependencias únicamente en el entorno.
