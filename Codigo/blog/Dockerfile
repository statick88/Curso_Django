# Usamos la imagen base de Python para Django
FROM python:3.11

# Establecemos el directorio de trabajo en /app
WORKDIR /app

# Copiamos el archivo de requerimientos al contenedor
COPY requirements.txt .

# Instalamos las dependencias de Django
RUN pip install --no-cache-dir -r requirements.txt

# Copiamos el contenido del proyecto Django al contenedor
COPY . .

# Exponemos el puerto 8000 para acceder al servidor web de Django
EXPOSE 8000

# Comando para iniciar el servidor web de Django
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
