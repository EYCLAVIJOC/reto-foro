# Desafío: Construyendo tu propio Foro con Java y Spring Boot

¡Bienvenidos y bienvenidas a este nuevo desafío! En esta oportunidad, pondremos en práctica los conocimientos adquiridos en **Java** y **Spring Boot** para construir nuestra propia **API REST** con la temática de un foro.

## 🎯 Objetivo del Desafío
El objetivo es crear un foro donde las personas puedan:
- Crear tópicos con dudas o sugerencias.
- Responder e interactuar dentro de la comunidad.
- Gestionar los tópicos de forma segura utilizando autenticación con **JWT (JSON Web Tokens)**.

## 🔧 Herramientas a Utilizar
- **Backend:** Java + Spring Boot
- **Base de datos:** A elección (MySQL, PostgreSQL, SQL Server, etc.)
- **Cliente para pruebas:** Insomnia o Postman
- **Gestión de tareas:** Trello (opcional, para organizar el proyecto)

## 📌 Funcionalidades
1. **Listar Tópicos**
   - Endpoint: `GET /topicos`
   - Retorna todos los tópicos creados.
   - Código de respuesta: `200 OK`

2. **Crear Tópico**
   - Endpoint: `POST /topicos`
   - Campos recomendados:
     - `idUsuario`
     - `titulo`
     - `mensaje`
     - `curso` (opcional)
   - Requiere **autenticación** mediante JWT.
   - Código de respuesta: `201 Created`

3. **Eliminar Tópico**
   - Endpoint: `DELETE /topicos/{id}`
   - Requiere **autenticación**.
   - Código de respuesta: `200 OK`

4. **Autenticación**
   - Endpoint: `POST /auth/login`
   - Campos: `email` y `password`
   - Retorna un **Bearer Token** que se utilizará en los endpoints protegidos.

## 🔐 Seguridad
- Los endpoints de creación, eliminación y actualización de tópicos requieren autenticación.
- Implementación mediante **JWT (JSON Web Tokens)**.
- Usuarios deben estar registrados en la base de datos para autenticarse.

## 🚀 Cómo Probar
1. Registrar un usuario en la base de datos.
2. Autenticarse para obtener el token JWT.
3. Utilizar el token como **Bearer Token** en Insomnia o Postman.
4. Probar los endpoints de creación, listado y eliminación de tópicos.

## 🖌 Personalización
Este proyecto es tuyo, así que puedes:
- Añadir más funcionalidades como comentarios o likes.
- Personalizar los campos de los tópicos.
- Integrar un **frontend** en el futuro.

## 🌟 Recomendaciones
- Divide el proyecto en tareas pequeñas y usa Trello para organizarte.
- Comparte tu proceso en la comunidad de Discord para recibir apoyo.
- Dale tu toque personal al proyecto y hazlo tuyo.

---

¡Manos a la obra! Construyamos juntos nuestra propia versión de un foro y disfrutemos del proceso.  

