<p align="center"><a href="https://www.docker.com/" target="_blank"><img src="https://www.pinclipart.com/picdir/big/331-3317152_from-docker-images-docker-container-docker-engine-logo.png" width="400"></a></p>
<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

# Laravel-Dockerized
This is a simple boilerplate to dockerize a Laravel project including services such as : 
* nginx
* mysql
* php
* artisan
* composer
* npm

### Runngin Project
1. Clone The Project
2. docker-compose run --rm composer  create-project laravel/laravel .
3. docker-compose up -d server
4. open project in localhost:8000

### Upgrade note
To upgrade the project you need to pull and re-create containers with the latest images.
So you can stop containers and then run docker-composer with this options:

docker-compose up --force-recreate --build -d server

### Services Guide
#### PhpMyadmin
To run this service simply use this command:
  ```sh
  docker-compose up -d phpmyadmin
  ```
Then you can open 192.168.10.80 to see phpmyadmin login page.
Mysql user definition is in service/mysql/mysql.env you can use them to log in.
To change the ip or port you can simply edit docker-compose.yml and phpmyadmin service. 
