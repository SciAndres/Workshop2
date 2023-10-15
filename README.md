# Workshop2
Proyecto de Análisis de Datos y Visualización de Premios Grammy y Spotify 
Este proyecto se centra en el análisis de datos relacionados con los premios Grammy utilizando Python, Pandas, Matplotlib y SQLAlchemy. El objetivo es explorar y visualizar la información de los premios Grammy y spotify y combinarla con datos de la plataforma de música Spotify. También se carga el resultado en una base de datos PostgreSQL.

Requisitos Previos:
Asegúrate de tener Python instalado en tu sistema.
Instala las bibliotecas requeridas usando pip install pandas, matplotlib y sqlalchemy seaborn.

Configuración de la Base de Datos:
Se utiliza una base de datos PostgreSQL para almacenar los datos. Asegúrate de tener PostgreSQL instalado en tu máquina y configura la conexión en el archivo Python, por ejemplo:
engine = create_engine('postgresql://postgres:Basesdedatosandres@localhost:5432/WS2')

Análisis de Datos:
El análisis de datos se realiza en varias etapas:

Carga de Datos: Los datos de los premios Grammy se cargan desde la base de datos PostgreSQL y los de spotify se leen directamente desde python, posteriormente a realizar la manipulacion se cargan a la base de datos.

Limpieza de Datos: Se realizan operaciones de limpieza, como la eliminación de valores nulos en las columnas 'artist' y 'workers'.

Exploración de Datos: Se exploran los datos para obtener información como la cantidad de premios por categoría y las categorías más comunes.

Visualización de Datos: Se crea un gráfico de barras que muestra las categorías de premios más comunes.

Combinación de Datos: Se combinan los datos de los premios Grammy con datos de la plataforma de música Spotify y se guarda el resultado en un archivo CSV.

Carga en la Base de Datos: El archivo CSV resultante se carga en la base de datos PostgreSQL con el nombre "Merge1".
