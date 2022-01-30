# docker-compose-default

This repository have a little code to docker-compose php with mongo db and mysql. The idea is to increase the repository with codes for different configurations.
## PHP

### Details

- `docker-compose.yml` - php 8.1 (pdo_mysql) needed php-fpm/DockerFile, mysql, nginx:latest, redis. 
- `docker-compose-mongo.yml` - php 7.3 (pdo_mongodb) needed php-fpm-mongo/DockerFile, mongodb, nginx:latest, mongo-express. 

### Files
 - `docker/nginx/site.conf` - change name_folder at line 6 to you name folder config in docker-compose.yml

### Commands
 - `docker-compose up -d` - run the containers in the background.
 - `docker-compose down` - down containers.
 - `docker-compose restart` - restart containers.
 - `docker-compose ps` - this command will list only the containers of the current docker-compose.yml.

 ## Node

 The node configuration is easy, it is only copy `docker-compose.yml` and `Dockerfile` in your project and execute `docker-compose up -d`. It going install node libraries with npm comand.