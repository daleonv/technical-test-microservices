# Resolución de prueba técnica

# Introducción
El problema propuesto fue solventado usando springboot orientado a microservicios para el  **backend** y Angular para el **frontend**


# Repositorios
Módulo de dependencias y versiones
[app-gradle.git](https://github.com/daleonv/app-gradle.git)

Módulo para el mapeo de entidades
[app-entities.git](https://github.com/daleonv/app-entities.git)

Microservicios de configuración (Eureka, Api Gateway)
[app-config.git](https://github.com/daleonv/app-config.git)

Microservicios de negocio
[app-person.git](https://github.com/daleonv/app-person.git)
[app-procedure.git](https://github.com/daleonv/app-procedure.git)

Front-End
[app-front.git](https://github.com/daleonv/app-front.git)


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
