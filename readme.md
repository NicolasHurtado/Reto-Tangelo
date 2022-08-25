Versión Python: `3.6`

## Objetivos de la Aplicación

- La aplicacion no hace uso de ningun `framework`

- De https://restcountries.com/ obtenga el nombre del idioma que habla el país y encriptelo con SHA1 

- En la columna Time ponga el tiempo que tardó en armar la fila (debe ser automático)

- La tabla debe ser creada en un DataFrame con la librería PANDAS 

- Con funciones de la librería pandas muestre el tiempo total, el tiempo promedio, el tiempo mínimo y el máximo que tardo en procesar todas las filas de la tabla

- Guarde el resultado en sqlite

- Genere un Json de la tabla creada y guárdelo como data.json


## Base de Datos

La app usa base de datos sqlite creada automaticamente al momento de insertar los datos.


## Crear entorno Virtual

python -m venv venv


## Instale requerimientos

pip install -r requeriments.txt

## Correr server

python main.py

Cuando el servidor esté arriba, debe ir al url  http://127.0.0.1:8000/ y posterior a esa acción obtendrá la respuesta en formato JSON de acuerdo a las especificaciones.


## Correr con docker 

docker build -t tangelo .

docker run --name tangelo_app -p 8000:8000 -d tangelo

