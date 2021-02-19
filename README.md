# Contenedor Docker para proyectos de Data Science

Configuración de un contenedor docker para proyectos de data science. El principal objetivo es tener en un contenedor aislado (con la instalación de Python, los módulos necesarios para el proyecto, y Jupyter) del resto de nuestro equipo, permitiendo diferentes configuraciones para diferentes proyectos.

## Requisitos
Para poder ejecutarlo es necesario tener instalado Docker en el equipo. Las instrucciones de instalación se pueden revisar en la página oficial de [Docker](https://www.docker.com/).

## Instalación

Dirigirnos a la carpeta principal de este proyecto y, a continuación, ejecutar la instrucción `docker-compose up`.

## Contenido
El contenido de cada proyecto será el siguiente:
- `/data`: Carpeta donde se pondrán los datos con los que se quiere trabajar en el proyecto.
- `/notebooks`: Directorio principal de trabajo de Jupyter. Aquí se encontrarán los diferentes notebooks que iremos ejecutando.
- `/jupyter/Dockerfile`: fichero de configuración del contenedor. Aquí especificamos la imagen docker que queremos ejecutar, instalamos módulos extras para el proyecto y especificamos donde se ejecutarán los notebooks.
- `docker-compose.yaml`: fichero para componer la estructura del contenedor. En este fichero podemos modificar donde poner las carpetas locales en nuestro equipo y el puerto para acceder a Jupyter.
