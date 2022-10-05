<p align="center"><a href="https://www.docker.com/" target="_blank"><img src="https://www.pinclipart.com/picdir/big/331-3317152_from-docker-images-docker-container-docker-engine-logo.png" width="400"></a></p>
<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

# Laravel-Dockerized
This project is finalized version of dockerized Laravel module in [docker tutorial](https://itsalireza.com/product/%d8%af%d9%88%d8%b1%d9%87-%d8%a7%d9%85%d9%88%d8%b2%d8%b4%db%8c-%d9%81%d8%a7%d8%b1%d8%b3%db%8c-%d8%af%d8%a7%da%a9%d8%b1-%d9%be%d8%b1%d9%88%da%98%d9%87-%d9%85%d8%ad%d9%88%d8%b1/).
including services such as : 
* nginx
* mysql
* php
* artisan
* composer
* npm

## :whale: :whale: :whale: :whale: [link to Docker Tutorial!](https://itsalireza.com/product/%d8%af%d9%88%d8%b1%d9%87-%d8%a7%d9%85%d9%88%d8%b2%d8%b4%db%8c-%d9%81%d8%a7%d8%b1%d8%b3%db%8c-%d8%af%d8%a7%da%a9%d8%b1-%d9%be%d8%b1%d9%88%da%98%d9%87-%d9%85%d8%ad%d9%88%d8%b1/) :whale: :whale: :whale: :whale:

### Runngin Project
1. Clone The Project
2. docker-compose run --rm composer  create-project laravel/laravel .
3. docker-compose up -d server
4. open project in localhost:8000

### Upgrade note
To upgrade the project you need to pull and re-create containers with the latest images.
So you can stop containers and then run docker-composer with this options:

docker-compose up --force-recreate --build -d server
