# Especificamos la imagen docker, en este caso la de jupyter
FROM jupyter/datascience-notebook

# Imprimimos la versión de Python
RUN python --version

# Incluimos el fichero requirements.txt
ADD requirements.txt /app/

# Indicamos las librerías adicionales que queremos instalar
RUN pip install --upgrade pip \
    && pip install -r /app/requirements.txt

# Añadimos el volumen /notebooks y lo establecemos como directorio de trabajo
VOLUME /notebooks
WORKDIR /notebooks