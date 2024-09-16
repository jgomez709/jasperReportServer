# Instalación de JasperReportServer usando Docker

Este repositorio contiene las configuraciones necesarias para instalar JasperReportServer utilizando contenedores Docker.

## Herramientas instaladas

### 1. Base de Datos PostgreSQL (15)

Configuración de variables (ajustar según necesidades):

```
POSTGRES_USER=jasperreports
POSTGRES_PASSWORD=jasperreportspass
POSTGRES_DB=jasperreports
```

### 2. Administrador de la Base de Datos (PgAdmin)

Configuración de variables (ajustar según necesidades):

```
PGADMIN_DEFAULT_EMAIL=admin@example.com
PGADMIN_DEFAULT_PASSWORD=adminpassword
```

### 3. JasperReportServer

Configuración de variables (ajustar según necesidades):

```
JASPERREPORTS_DATABASE_NAME=jasperreports
JASPERREPORTS_DATABASE_USER=jasperreports
JASPERREPORTS_DATABASE_PASSWORD=jasperreportspass
JASPERREPORTS_USERNAME=jasperadmin
JASPERREPORTS_PASSWORD=jasperadmin
```

## Instalación

Siga estos pasos para instalar JasperReport Server:

1. Acceda a "wsl" usando la consola de comandos.
2. Diríjase a una carpeta local de Linux según su usuario: `/home/<usuario>/jasperserver`.
3. Clone el repositorio usando el siguiente comando:
   ```
   sudo git clone https://github.com/jgomez709/jasperReportServer.git .
   ```
4. Ejecute el siguiente comando para descargar las imágenes especificadas, levantar los contenedores, crear y montar los volúmenes definidos y conectar los contenedores a la red:
   ```
   docker-compose up
   ```
5. Acceda a JasperReportServer usando la URL: `http://localhost:8080/jasperserver`
6. Administre la base de datos desde PgAdmin, accediendo a la URL: `http://localhost:5050/browser/`

Siéntase libre de usar este repositorio para la instalación. Esperamos que le sea de mucha ayuda.
