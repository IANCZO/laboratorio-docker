# Laboratorio Docker

## 1. Creación y comprobación del contenedor
Se creó el contenedor utilizando la imagen oficial de Tomcat, asignando el nombre `servidor_web` y mapeando el puerto 8080:

```bash
docker run -d -p 8080:8080 --name servidor_web tomcat:9.0
docker ps
```

<img width="1150" height="54" alt="comprobacion" src="https://github.com/user-attachments/assets/03c3cb13-6001-464e-b115-1e89fcbb410c" />
<img width="662" height="261" alt="creacion_contenedor" src="https://github.com/user-attachments/assets/585473e4-4e5a-49d0-a506-7c03c38aaf7d" />


## 2. Acceso al servidor web
Acceso exitoso a la interfaz de Apache Tomcat a través del navegador web local:

<img width="1204" height="737" alt="navegador_tomcat" src="https://github.com/user-attachments/assets/097c53bf-50d2-4b6f-934e-ab389a209866" />

## 3. Eliminación del contenedor
Finalización del ciclo de vida del contenedor deteniendo su ejecución y removiendo el recurso del sistema:

```bash
docker stop servidor_web
docker rm servidor_web
```

<img width="395" height="74" alt="limpieza" src="https://github.com/user-attachments/assets/6b5651e0-a7dc-4ba6-a47a-9db93a9190ea" />

