
# Prueba Técnica 

Este repositorio contiene la solución a la **Prueba Técnica** basada en una **arquitectura de microservicios** para la gestión de clientes, cuentas y movimientos bancarios. La implementación incluye tanto el **Back-End** desarrollado en **Java Spring Boot** como el **Front-End** con **Angular o React**.

## 📌 Tecnologías Utilizadas

### Back-End:
- Java + Spring Boot
- JPA / Hibernate
- Base de Datos Relacional (MySQL)
- Docker
- Eureka (Service Discovery)
- API Gateway
- Pruebas Unitarias con JUnit

### Front-End:
- Angular
- Consumo de APIs REST
- Generación de reportes en formato PDF

## 📂 Estructura del Proyecto

| Módulo | Descripción |
|--------|------------|
| **🔗 [app-gradle.git](https://github.com/daleonv/app-gradle.git)** | Contiene la configuración de dependencias y versiones compartidas entre los microservicios. |
| **📦 [app-entities.git](https://github.com/daleonv/app-entities.git)** | Módulo que define las entidades y modelos de datos utilizados por los microservicios. |
| **⚙️ [app-config.git](https://github.com/daleonv/app-config.git)** | Contiene los microservicios de configuración como **Eureka Service Registry** y **API Gateway** para la gestión y comunicación entre servicios. |
| **🛠️ [app-person.git](https://github.com/daleonv/app-person.git)** | Microservicio responsable de la gestión de personas (usuarios, clientes, etc.). |
| **📑 [app-procedure.git](https://github.com/daleonv/app-procedure.git)** | Microservicio encargado de los procesos administrativos o procedimientos específicos del negocio. |
| **🎨 [app-front.git](https://github.com/daleonv/app-front.git)** | Aplicación **Front-End** desarrollada en **Angular**, encargada de la interfaz de usuario. |

## 🚀 Funcionalidades Implementadas

- **Gestión de Clientes:** CRUD completo para la entidad cliente.
- **Gestión de Cuentas:** Creación, actualización y eliminación de cuentas bancarias.
- **Gestión de Movimientos:** Registro de depósitos y retiros, con validaciones de saldo.
- **Generación de Reportes:** Consulta de movimientos por cliente y rango de fechas, con exportación a PDF y JSON.
### 📝 Nota:
- 📂 **Script SQL:** [BaseDatos.sql](https://github.com/daleonv/app-person/blob/main/script.sql)  
- 📂 **Colección de Postman:** [postman_collection.json](https://github.com/daleonv/app-person/blob/main/API%20Documentation.postman_collection.json)  


