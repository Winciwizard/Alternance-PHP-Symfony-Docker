## Docker-compose for symfony
_**/!\ This setup works on linux, never tried on windows**_
1. Install docker, and docker-compose
2. Create a symfony project or take an existing project and add the config/docker folder AND docker-compose.yml to the project
3. Run the following commands:
```bash
docker volume create mysqlsymfonydata
docker-compose up -d 
```  
4. Symfony app : http://localhost:8000
5. Adminer (like phpmyadmin) : http://localhost:8080

_The database credentials are :_
```
host: mysqlserver
user: symfony
pass: password
```
_To run a composer command_
```
docker-compose run composer MY_COMMAND
```

_To run a php command_
```
docker-compose run fpm MY_COMMAND
```
for example : 
```
docker-compose run fpm bin/console MY_COMMAND
```
