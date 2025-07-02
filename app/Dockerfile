# Usa una imagen base de Python liviana
FROM python:3.10-slim

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia los archivos necesarios
COPY requirements.txt .
COPY app.py .

# Instala las dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Expone el puerto 8000 para Flask
EXPOSE 8000

# Comando para ejecutar la aplicación
CMD ["python", "app.py"]