# Imagen base de Node.js
FROM node:18

# Establecer directorio de trabajo
WORKDIR /app

# Copiar archivos y paquetes
COPY package.json package-lock.json ./
RUN npm install

# Copiar el resto del código
COPY . .

# Exponer el puerto
EXPOSE 8080

# Ejecutar el servidor WebSocket
CMD ["npm", "start"]
