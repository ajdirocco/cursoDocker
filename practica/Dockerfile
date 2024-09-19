# Usamos la imagen base de Alpine Linux
FROM alpine:latest

# Establecemos el directorio de trabajo
WORKDIR /app

# Copiamos los archivos del proyecto al contenedor
COPY . .

# Actualizamos los paquetes e instalamos Node.js y Yarn directamente desde los repositorios oficiales
# && Instalamos las dependencias del proyect
RUN apk add --no-cache nodejs yarn && yarn install --production

# Exponemos el puerto de la aplicación (ejemplo: 3000)
EXPOSE 3000

# Comando por defecto para ejecutar la aplicación
CMD ["node", "src/index.js"]
