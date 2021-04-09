# Description ?
:whale2: A Symfony-ready docker environment :whale2:


# Stack 
* Debian stretch
* Apache 2
* MySQL 5
* PHP 7.4.16-fpm
* Maildev


# How to ?
Build services : `docker-compose build`

Create/start containers : `docker-compose up -d`

bash access to php_sf container : `docker exec -it -u dev php_sf bash`

Compose project :
`cd /home/wwwroot/sf`

`composer create-project symfony/website-skeleton my-project-name`

Go to `http://localhost:8042` and let's go :rocket:


# Useful docker & docker-compose commands

## List containers (from docker compose folder)
`docker-compose ps`

## Restart services (apache, mysql, php, phpmyadmin, maildev)
`docker-compose restart`

## Stop containers
`docker container stop phpmyadmin_sf maildev_sf mysql_sf php_sf apache_sf`

## Remove containers
`docker-compose rm`
