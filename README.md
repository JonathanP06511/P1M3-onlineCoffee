# Microservicio de Gestión de Productos

Este proyecto es un microservicio desarrollado con Node.js y Express para gestionar productos mediante una API REST.

## Requisitos

- Node.js
- Docker (opcional, para despliegue con contenedor)

## Instalación

1. Clona este repositorio:
    ```bash
    git clone https://github.com/tu_usuario/tu_repositorio.git
    cd tu_repositorio
    ```

2. Instala las dependencias:
    ```bash
    npm install
    ```

3. Asegúrate de tener un directorio `frontend` en la raíz del proyecto que contenga tu interfaz de usuario.

## Uso

1. Inicia el servidor:
    ```bash
    node server.js
    ```

2. Abre tu navegador y navega a `http://localhost:3000` para interactuar con la interfaz de usuario.

## Uso con Docker

1. Construye la imagen Docker:
    ```bash
    docker build -t product-service .
    ```

2. Inicia un contenedor con la imagen creada:
    ```bash
    docker run -p 3000:3000 -v $(pwd)/frontend:/app/frontend product-service
    ```

3. Abre tu navegador y navega a `http://localhost:3000` para interactuar con la interfaz de usuario.

## Endpoints

- `GET /products`: Obtiene todos los productos.
- `POST /products`: Crea un nuevo producto.
- `GET /products/:id`: Obtiene un producto específico por ID.
- `PUT /products/:id`: Actualiza un producto específico por ID.
- `DELETE /products/:id`: Elimina un producto específico por ID.

## Estructura del Proyecto

