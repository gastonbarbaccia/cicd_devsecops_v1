# CI/CD DevOps
## Gitleaks + PHP Stan + PHP Lint + SonarCloud + Dependency Check + Mysql Deploy + Deploy Staging Hostinger

### Crear las siguientes variables como secrets dentro del settings del proyecto:

TOKEN_GITHUB es un token de github que se puede crear con otro nombre de ser necesario, recordar colocar el nombre en el main.yml  
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
El codigo de la aplicacion debera estar dentro de la carepta DEPLOY

### Sonarcloud properties  
El codigo de esta configuracion la da el propio sonarcloud al configurar un nuevo proyecto  

### Script.sql  
Dentro de este script se debera colocar el codigo sql que debera realizar las siguientes operaciones:  
- drop database   
- create database  
- use database  
- create table  
- insert into table  

### Credenciales del RDS
Servidor: database-1-ohio.capjeqwtb4vf.us-east-2.rds.amazonaws.com  
Puerto: 3306  
Usuario: admin  
Contraseña: Inicio1234.  

### Credenciales del hosting
Servidor: ftp.devops-dev.ga
Usuario: u666073011.devops
Contraseña: Inicio1234. (con la primera i en mayuscula y con el punto al final)

### Carpeta DEPLOY
Modificar la cadena de conexion del archivo conexiondb.php para apuntar a la base de datos de aws


### Links

[filezilla](https://filezilla-project.org/download.php?type=client)  
[heidi sql](https://www.heidisql.com/download.php)

## Author: Gaston Barbaccia
