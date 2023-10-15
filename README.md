# Workshop2
# Proyecto de Análisis de Datos y Visualización de Premios Grammy y Spotify

Este proyecto se centra en el análisis de datos relacionados con los premios Grammy y Spotify utilizando Python, Pandas, Matplotlib, Seaborn, y SQLAlchemy. El objetivo es explorar y visualizar información sobre los premios Grammy y datos de canciones de Spotify, y combinarlos en un análisis conjunto. Además, se carga el resultado en una base de datos PostgreSQL.

## Requisitos Previos

- Asegúrate de tener Python instalado en tu sistema.
- Instala las bibliotecas requeridas usando `pip install pandas, matplotlib y sqlalchemy seaborn`.

## Configuración de la Base de Datos

Se utiliza una base de datos PostgreSQL para almacenar los datos. Asegúrate de tener PostgreSQL instalado en tu máquina y configura la conexión en el archivo Python.

```python
engine = create_engine('postgresql://postgres:Basesdedatosandres@localhost:5432/WS2')

## Análisis de Datos de los Premios Grammy:

El análisis de datos de los premios Grammy se realiza en varias etapas:

Carga de Datos: Los datos de los premios Grammy se cargan desde la base de datos PostgreSQL.

Limpieza de Datos: Se realizan operaciones de limpieza, como la eliminación de valores nulos en las columnas 'artist' y 'workers'.

Exploración de Datos: Se exploran los datos para obtener información como la cantidad de premios por categoría y las categorías más comunes.

Visualización de Datos: Se crea un gráfico de barras que muestra las categorías de premios más comunes.

Análisis de Datos de Spotify:
El análisis de datos de Spotify se realiza en varias etapas:

Carga de Datos de Spotify: Los datos de canciones de Spotify se cargan desde un archivo CSV.

Exploración de Datos de Spotify: Se exploran los datos para obtener información como la distribución de popularidad de las canciones y la proporción de canciones explícitas.

Preprocesamiento de Datos de Spotify: Se realizan operaciones de preprocesamiento, como la conversión de tipos de datos, la eliminación de columnas innecesarias y la detección de duplicados.

Carga de Datos en la Base de Datos: Los datos de Spotify se cargan en la base de datos PostgreSQL con el nombre "premioss".

Combinación de Datos
Luego de analizar ambos conjuntos de datos por separado, se realiza una combinación de datos para explorar relaciones entre los datos de los premios Grammy y las canciones de Spotify. El resultado se guarda en un archivo CSV.

Autor
Nombre: Andres Enriquez
Correo Electrónico: andres_alb.enriquez@uao,edu.co 
