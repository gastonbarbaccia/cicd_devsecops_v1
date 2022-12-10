# CI/CD DevOps
## Gitleaks + PHP Stan + PHP Lint + SonarCloud + Dependency Check + Mysql Deploy + Deploy Staging Hostinger

### Crear las siguientes variables como secrets dentro del settings del proyecto:

GITHUB_TOKEN es un token de github que se puede crear con otro nombre de ser necesario, recordar colocar el nombre en el main.yml  
SONAR_TOKEN es un token que se genera en sonarcloud  

### Secrets FTP  
FTP_SERVER servidor de hostinger  
FTP_USERNAME usuario de ftp de hostinger  
FTP_PASSWORD contraseña del usuario de ftp   

### Secrets Base de datos  
DATABASE_HOST nombre o IP del servidor donde se encuentra la base de datos  
DATABASE_PORT puerto de mysql, por defecto se debe configurar el 3306. Ej: DATABASE_PORT = 3306  
DATABASE_NAME nombre de la base de datos  
DATABASE_USERNAME usuario de la base de datos  
DATABASE_PASSWORD contraseña de la base de datos  
DATABASE_SCRIPT  nombre del archivo .sql que se desea importar en la base de datos. Ej.  script.sql

### Codigo PHP  
El codigo de la aplicacion debera estar dentro de la carepta src en la raiz del proyecto

## Author: Gaston Barbaccia
