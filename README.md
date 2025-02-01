# Resolución de prueba técnica

# Introducción
El problema propuesto fue solventado usando springboot orientado a microservicios para el  **backend** y Angular para el **frontend**


## Estructura del Proyecto  

| Módulo | Descripción |
|--------|------------|
| **🔗 [app-gradle.git](https://github.com/daleonv/app-gradle.git)** | Contiene la configuración de dependencias y versiones compartidas entre los microservicios. |
| **📦 [app-entities.git](https://github.com/daleonv/app-entities.git)** | Módulo que define las entidades y modelos de datos utilizados por los microservicios. |
| **⚙️ [app-config.git](https://github.com/daleonv/app-config.git)** | Contiene los microservicios de configuración como **Eureka Service Registry** y **API Gateway** para la gestión y comunicación entre servicios. |
| **🛠️ [app-person.git](https://github.com/daleonv/app-person.git)** | Microservicio responsable de la gestión de personas (usuarios, clientes, etc.). |
| **📑 [app-procedure.git](https://github.com/daleonv/app-procedure.git)** | Microservicio encargado de los procesos administrativos o procedimientos específicos del negocio. |
| **🎨 [app-front.git](https://github.com/daleonv/app-front.git)** | Aplicación **Front-End** desarrollada en **Angular**, encargada de la interfaz de usuario. |



## Instrucciones

Para levantar el proyecto en un servidor local se deben seguir los siguientes pasos:

Los microservicios deben estar en el mismo directorio donde se descargue el proyecto app-gradle, porque dependen de él para administrar las versiones y las dependencias.

El proyecto app-entities debe ser el primero en compilarse, porque es una dependencia de los demás.
En el directorio raíz de **app-gradle** se ejecuta el comando 
> gradle clean build 

Lo siguiente es levantar los microservicios de **app-config**, basta con ejecutar, en la raíz de cada microservicio.
> gradle clean build 

y posteriormente se ejecuta
> gradle gradle bootRun

El siguiente paso es aplicar los mismos comandos en cada uno de los microservicios de negocio **app-person** y **app-procedure**.

> gradle clean build 

y posteriormente se ejecuta
> gradle gradle bootRun
