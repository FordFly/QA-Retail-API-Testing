# QA-Retail-API-Testing - Portfolio Project
Este repositorio contiene un proyecto práctico de **Quality Assurance (QA)** enfocado en pruebas de API para el sector Retail / E-commerce, utilizando **Postman**. 

El objetivo de este proyecto es demostrar la capacidad para validar endpoints, analizar estructuras de datos complejas y automatizar pruebas básicas de backend.

## Tecnologías y Herramientas utilizadas
* **Herramienta principal:** Postman
* **Formatos de datos:** JSON
* **API de pruebas:** [Fake Store API](https://fakestoreapi.com/) (Simulación de backend de e-commerce)
* **Validaciones:** Librería Chai (pm.test) integrada en Postman Scripts.

## Casos de Prueba Implementados

Se ha diseñado una colección de Postman que cubre operaciones CRUD básicas de una tienda online:

1. **GET All Products (Catálogo):**
   - Validación de Status Code `200 OK`.
   - Prueba de rendimiento (Response time < 800ms).
   - Verificación de la estructura del **JSON** devuelto (Validación de que es un Array y contiene las propiedades clave: `id`, `title`, `price`).

2. **POST New Product (Añadir artículo):**
   - Envío de un payload en formato JSON simulando la creación de un nuevo producto.
   - Validación de la correcta creación en el servidor.

## Cómo ejecutar estas pruebas
1. Clona este repositorio o descarga el archivo `.json`.
2. Abre Postman.
3. Ve a `File` > `Import` y selecciona el archivo `.json`.
4. Ejecuta las peticiones y revisa la pestaña de `Test Results` (Scripts > Post-response).
