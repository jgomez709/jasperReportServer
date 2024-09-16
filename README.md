# Instalación de JasperReportServer usando Docker

Este repositorio contiene las configuraciones necesarias para instalar JasperReportServer utilizando contenedores Docker. Las herramientas instaladas son las siguientes:

## Herramientas Instaladas

1. **Base de Datos PostgreSQL (15):** 
   Modifica las siguientes variables según tus necesidades:
   - `POSTGRES_USER=jasperreports`
   - `POSTGRES_PASSWORD=jasperreportspass`
   - `POSTGRES_DB=jasperreports`

2. **Administrador de Base de Datos (PgAdmin):** 
   Ajusta las siguientes variables según tus preferencias:
   - `PGADMIN_DEFAULT_EMAIL=admin@example.com`
   - `PGADMIN_DEFAULT_PASSWORD=adminpassword`

3. **JasperReportServer:** 
   Configura las siguientes variables según tus necesidades:
   - `JASPERREPORTS_DATABASE_NAME=jasperreports`
   - `JASPERREPORTS_DATABASE_USER=jasperreports`
   - `JASPERREPORTS_DATABASE_PASSWORD=jasperreportspass`
   - `JASPERREPORTS_USERNAME=jasperadmin`
   - `JASPERREPORTS_PASSWORD=jasperadmin`

## Instalación

Para instalar JasperReportServer, sigue estos pasos:

1. Abre "WSL" usando la consola de comandos.
2. Navega a una carpeta local en Linux, por ejemplo: `/home/<usuario>/jasperserver`.
3. Clona el repositorio con el siguiente comando:
   ```bash
   sudo git clone https://github.com/jgomez709/jasperReportServer.git .
