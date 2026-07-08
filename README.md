# Laboratorio Docker

## 1. Creación y comprobación del contenedor
Se creó el contenedor utilizando la imagen oficial de Tomcat, asignando el nombre `servidor_web` y mapeando el puerto 8080:

```bash
docker run -d -p 8080:8080 --name servidor_web tomcat:9.0
docker ps
```

![Creación del contenedor](captura1.png)

## 2. Acceso al servidor web
Acceso exitoso a la interfaz de Apache Tomcat a través del navegador web local:

![Acceso al navegador](captura2.png)

## 3. Eliminación del contenedor
Finalización del ciclo de vida del contenedor deteniendo su ejecución y removiendo el recurso del sistema:

```bash
docker stop servidor_web
docker rm servidor_web
```

![Eliminación del contenedor](captura3.png)
