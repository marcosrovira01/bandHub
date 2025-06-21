# **BandHub: Gestión de agrupaciones musicales**

Bienvenido al monorepo de BandHub, una aplicación web diseñada para la gestión integral de ensayos y actuaciones de agrupaciones musicales. Este proyecto está construido con Spring Boot y una arquitectura de microservicios, utilizando las últimas tecnologías de Spring Cloud para la orquestación y seguridad.

---

## **Descripción del Proyecto**

BandHub es una plataforma que permite a los administradores de agrupaciones musicales y a los propios músicos gestionar de manera eficiente sus actividades. Las funcionalidades clave incluyen:

- Gestión de Agrupaciones Musicales: Registro y administración de datos de agrupaciones (teléfono, correo, etc.).
- Gestión de Músicos: Añadir, eliminar y actualizar información de los músicos, incluyendo nombre, apellidos, número de hermano e instrumento.
- Gestión de Eventos: Crear y administrar ensayos y actuaciones con detalles como fecha, hora y lugar.
- Control de Asistencia: Registrar la asistencia de los músicos a los eventos para un seguimiento detallado.
- Seguridad y Autenticación: Sistema de login para administradores y músicos, con roles y privilegios diferenciados (administrador puede gestionar todo; músico puede ver sus propios datos y asistencias).
- El objetivo principal de este proyecto es profundizar en el desarrollo de microservicios con Spring Boot, Spring Security y la integración de CI/CD en AWS.

---

## **Arquitectura de microservicios**

El proyecto sigue una arquitectura de microservicios y está organizado en un monorepo, conteniendo los siguientes servicios principales:

- Auth Service: Encargado de la autenticación de usuarios y la gestión de tokens JWT.
- Agrupations Service: Gestiona la información de las agrupaciones musicales.
- Musics Service: Administra los datos de los músicos y su asociación con las agrupaciones.
- Events Service: Maneja los ensayos y actuaciones, incluyendo el registro de asistencia.
- API Gateway: Punto de entrada centralizado para todas las peticiones, gestiona el enrutamiento y la seguridad de borde.
- Eureka Server: Servidor de descubrimiento de servicios que permite a los microservicios encontrarse dinámicamente.
- Config Server: Servidor de configuración centralizado para gestionar las propiedades de todos los microservicios.

---

## **Tecnologías utilizadas**

- Backend: Spring Boot 3.3.x, Java 17
- Microservicios: Spring Cloud (Gateway, Netflix Eureka, Config Server)
- Seguridad: Spring Security (con JWT para autenticación)
- Persistencia: Spring Data JPA / Hibernate
- Base de Datos: PostgreSQL
- Gestión de Proyectos: Apache Maven (monorepo multi-módulo)