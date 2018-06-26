## Docker-compose for symfony
_**/!\ This setup works on linux, never tried on windows**_
1. Install docker, and docker-compose
2. Run the following commands:
```bash
docker-compose volume create mysqlsymfonydata
docker-compose up -d 
```  
3. Symfony app : http://localhost:8000
4. Adminer (like phpmyadmin) : http://localhost:8080

_The database credentials are :_
```
host: mysqlserver
user: symfony
pass: password
```
