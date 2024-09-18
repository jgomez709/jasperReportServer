# JasperReportServer 8.1.0 Installation using Docker

This repository contains the necessary configurations to install JasperReportServer using Docker containers.

## Installed Tools

### 1. PostgreSQL Database (15)

Variable configuration (adjust as needed):

```
POSTGRES_USER=jasperreports
POSTGRES_PASSWORD=jasperreportspass
POSTGRES_DB=jasperreports
```

### 2. Database Administrator (PgAdmin)

Variable configuration (adjust as needed):

```
PGADMIN_DEFAULT_EMAIL=admin@example.com
PGADMIN_DEFAULT_PASSWORD=adminpassword
```

### 3. JasperReportServer (8.1.0)

Variable configuration (adjust as needed):

```
JASPERREPORTS_DATABASE_NAME=jasperreports
JASPERREPORTS_DATABASE_USER=jasperreports
JASPERREPORTS_DATABASE_PASSWORD=jasperreportspass
JASPERREPORTS_USERNAME=jasperadmin
JASPERREPORTS_PASSWORD=jasperadmin
```

## Installation

Follow these steps to install JasperReport Server:

1. Access "wsl" using the command console.
2. Navigate to a local Linux folder according to your user: `/home/<user>/jasperserver`.
3. Clone the repository using the following command:
   ```
   sudo git clone https://github.com/jgomez709/jasperReportServer.git .
   ```
4. Run the following command to download the specified images, start the containers, create and mount the defined volumes, and connect the containers to the network:
   ```
   docker-compose up
   ```
5. Access JasperReportServer using the URL: `http://localhost:8080/jasperserver`
6. Manage the database from PgAdmin by accessing the URL: `http://localhost:5050/browser/`

Feel free to use this repository for installation. We hope it will be very helpful to you.
