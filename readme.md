# Elecciones 26J

Proyecto para extraer y analizar los datos de las elecciones celebradas el 26 de junio de 2016 en España. El proyecto sirve de excusa para practicar con Python algunas tareas como:

* El _scraping_ de webs usando [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)
* El análisis de datos con [Pandas](http://pandas.pydata.org/)
* La visualización de datos con distintas librerías.

El código está creado usando [IPython Jupiter Notebook](http://jupyter.org/).

Los datos completos de las elecciones están en formato JSON en el archivo [resultados.json](https://github.com/GuilleUCM/elecciones26J/blob/master/resultados.json). Este archivo contiene una lista de diccionarios con el siguiente formato:

* `circunscripcion`: Nombre de la circunscripción
* `url`: URL de la web de la que se han extraido los datos
* `escanyos`: número de escaños que se reparten en la circunscripción
* `votosTotales`: Número total de votos contados
* `abstencion`: Número de abstenciones
* `votosNulos`: Número de votos nulos
* `votosEnBlanco`: Número de votos en blanco
* `resultados`: Lista con la distribución de los votos. Cada elemento de la lista es un diccionario con:
    * `partido`: Nombre del partido político
    * `votos`: número de votos obtenidos
    * `diputados`: número de diputados conseguido